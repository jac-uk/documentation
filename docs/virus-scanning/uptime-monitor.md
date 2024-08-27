# Uptime Monitor

## Overview

The Uptime Monitor is designed to verify and maintain the health of file upload and virus scanning processes within your application. This includes monitoring the functionality of file uploads, ensuring proper virus scanning, and validating the integrity of files.

## Key Functionalities

### 1. Virus Scanner Health Check

#### Purpose
The `runScannerTest` function is used to test the functionality of the virus scanner by running predefined test files. It checks whether the virus scanner correctly identifies a known virus (EICAR test file) and a clean file.

#### Implementation Details

- **Test Files**:
  - **EICAR Test File**: A known test file used to verify that the virus scanner detects it as a threat.
  - **Clean Test File**: A file that should be recognized as clean by the virus scanner.

- **Process**:
  1. The `runScannerTest` function invokes the `scanFile` method with paths to the test files.
  2. It retrieves and compares scan results against expected outcomes (clean vs. error).
  3. The results are logged and stored in Firestore under `settings/candidateSettings`.
  4. If the test fails, it logs an error but no alerting or monitoring process is currently implemented.

### 2. File Upload Component

#### Purpose
The file upload component allows users to upload files, ensuring they meet specified criteria and are processed correctly.

#### Key Features

- **File Upload**: Handles file selection, validation, and uploading to Firebase Storage.
- **File Validation**: Checks file type, size, and ensures it does not exceed a defined limit.
- **Error Handling**: Provides feedback if the file upload fails due to invalid type, size, or other issues.
- **File Replacement**: Allows users to replace an existing file if needed.

#### Implementation Details

- **File Constraints**:
  - **Size Limit**: Files are limited to 2 MB.
  - **Type Constraints**: Acceptable file types include `.pdf`, `.docx`, `.doc`, `.odt`, `.txt`, `.fodt`.

- **Process**:
  1. Users select a file through the file input.
  2. The file is validated based on type and size constraints.
  3. If valid, the file is uploaded to Firebase Storage.
  4. Existing files can be replaced if the `enableDelete` option is set to `true`.
