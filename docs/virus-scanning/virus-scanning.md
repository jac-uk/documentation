
## Malware Scanner Service Documentation

#### Overview
___
This service scans documents uploaded to Google Cloud Storage (GCS) for malware using ClamAV. The service is built on Google App Engine Flex and operates within a Docker container. When a file is uploaded to a specified GCS bucket, a Cloud Function triggers the service to download the file, scan it, and then handle it based on the scan results.

  ## Quickstart

1.  **Clone the Repository**
    `git clone https://github.com/GoogleCloudPlatform/docker-clamav-malware-scanner.git` 
    
2.  **Configure Google Cloud**
    
    Follow the setup instructions in the [tutorial](https://cloud.google.com/solutions/automating-malware-scanning-for-documents-uploaded-to-cloud-storage) to configure your Google Cloud project.
    
3.  **Deploy to App Engine**
    
    Navigate to the directory containing your App Engine configuration files and run one of the following commands based on your environment:
    
    -   **Development**:
        `gcloud app deploy` 
        
    -   **Staging**
        `gcloud app deploy app-staging.yaml --project=digital-platform-staging` 
        
    -   **Production**:
        `gcloud app deploy app-production.yaml --project=platform-production-9207d`

#### Components
___
1. **Dockerfile**
The Dockerfile describes how to build the Docker image for this service. It starts from a Node.js base image, installs necessary packages, and sets up ClamAV for malware scanning.

	**Key Points:**
	**Base Image:** node:10.15-stretch
	**Packages:** Includes net-tools, dos2unix, and clamav-daemon.
	**Command:** Runs bootstrap.sh which updates ClamAV definitions, reloads services, and starts the Node.js application.

___

2. **bootstrap.sh**

	This shell script initialises ClamAV and starts the Node.js application.
	
	**Steps**:
	**Update Definitions:** Runs freshclam to get the latest virus definitions.
	**Reload Services:** Reloads ClamAV services to apply updates.
**Start Application:** Runs the Node.js application using npm start.

___

3. **server.js**

	The main server file for handling HTTP requests and interacting with GCS and ClamAV.
	
	**Features:**
	**Express Server:** Listens on port 8080.
	**Rate Limiting:** Uses express-rate-limit to prevent abuse and limit cost.
**GCS Integration:** Downloads files from GCS for scanning within server.
**Malware Scanning:** Uses clamdjs to scan the downloaded file.
**Metadata:** Adds scan results as metadata to the file in GCS.
**Error Handling:** Logs errors and handles file clean-up.

___

4. **app.yaml, app-production.yaml, app-staging.yaml**

	These configuration files define how the service is deployed to Google App Engine. They specify the runtime environment, scaling settings, and environment variables.

	**Common Configurations:**
	
	**Runtime:** Custom runtime on App Engine Flex.

	**Scaling:** Different settings for development, staging, and production environments.

	**Environment Variables:** PROJECT_ID for identifying the GCS bucket.

___

## Setup
Cloning the repository, configuring Google Cloud, and deploying the service.

**Deployment:** Steps to deploy the service to different environments (development, staging, production) using gcloud.

**Debugging:** Tips for restarting the ClamAV service and viewing logs.

### Setup and Deployment

Clone Repository:

```
git clone https://github.com/GoogleCloudPlatform/docker-clamav-malware-scanner.git
```
or (for our implementation)

navigate to `digital-platform/google-app-engine/virus-scanning-node`

**Configure gcloud:**

Set up different configurations for development, staging, and production environments.

**Deploy to App Engine:**

**Development:** gcloud app deploy

**Staging:** gcloud app deploy app-staging.yaml --project=digital-platform-staging

**Production:** gcloud app deploy app-production.yaml --project=platform-production-9207d

## **Troubleshooting**
If ClamAV is not running after deployment, follow these steps to manually restart the service:

-  **Connect to the App Engine VM via SSH**:

`gcloud app browse`

-  **List Docker containers**:

`docker container ls`

-  **Access the Docker container**:

`docker exec -it gaeapp /bin/bash`

-  **Check listening ports**:

`netstat -plnt`

-  **Restart ClamAV**:

`service clamav-daemon force-reload`

-  **Verify ClamAV is listening**:

`netstat -plnt`