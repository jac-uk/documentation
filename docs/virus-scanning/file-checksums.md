# Scanned File Checksums

## Overview
Part of the malware scanning system includes a checksum stored in Firebase Storage, validating files before download to ensure file integrity, preventing manipulation or corruption whilst in storage. The system uses a Cloud Function to compare the current checksum of a file with a pre-stored checksum in Firestore (checksums > [storage file path]).

## Features

1. Checksum Creation: `createChecksum`, `addChecksumToFirestore`, `scanFileAndCreateChecksum`
Checksums are generated using a SHA-256 hash of the file content (digital-platform/functions/actions/malware-scanning/createChecksum.js), then stored (digital-platform/functions/actions/malware-scanning/addChecksumToFirestore.js) for comparison upon download. These are batched into an action `scanFileAndCreateChecksum` which is an end to end action including all steps for scanning a file, creating a checksum based on the result and storing it in firestore.

2. Cloud Function: `verifyFileChecksum`
A callable Cloud Function named verifyFileChecksum is implemented to handle checksum validation. When invoked, it:

Retrieves the expected checksum from Firestore.
Downloads the file from Firebase Storage.
Computes the checksum of the downloaded file.
Compares the computed checksum with the expected checksum.
Returns a validation result indicating whether the file's integrity is intact.

>{ valid: bool, message: [error.message || 'checksum mismatch'] }

4. Frontend Integration
Using the callable function `verifyFileChecksum` prior to download, file integrity is ensured prior to download, and prevented in the case of change. This functionality is all managed within the `DownloadLink` component, which also includes a feature flag for disabling of the checksums functionality. (intended to allow the feature to be rolled out and then for checksums to be created for preexisting files within our storage)

Display a download link if the file passes the checksum validation.
Provide feedback to the user if the file fails validation or if an error occurs during the process.

## Usage

Uploading Files: When files are uploaded, their checksums should be generated and stored in Firestore under a document corresponding to the file path.

Validating Files: Before a file is downloaded, the frontend should invoke the verifyFileChecksum Cloud Function to ensure the file has not been tampered with.

Handling Errors: If the checksum validation fails or if any errors occur, the frontend should handle these, ensuring that the file is not downloaded if its integrity cannot be confirmed.

Key Endpoints
Cloud Function: verifyFileChecksum
Request: { filePath: string }
Response: { valid: boolean, message?: string }