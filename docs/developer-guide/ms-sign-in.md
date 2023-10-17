## Updating Microsoft sign-in certificates
<h1>CERTIFICATE NEXT EXPIRES 1/11/2023 </h1>

### Steps to renew certificate
 - Log-in to [azure portal](https://portal.azure.com) with an account (this will be your microsoft/gov.uk account) which has owner privileges for the JAC azure project.
 - under 'Certificates & Secrets'
 - observe currently active secret 
 - In a new tab/window open the [ DEVELOP ] firebase console
 - under 'Authentication' > 'sign in method' > Microsoft 
 - Compare the viewable sections of the currently active keys.
 - Ensure they match.

- Generate a new key in the azure console
-  The secret is only available for a limited time so be sure to take a note of it asap
- Be sure to copy the 'value' NOT 'secret_id'
 - In firebase update the secret under the microsoft authentication update window.
 
- check the DEVELOP env
- test you can sign in with an MS account
- repeat above steps for each env
- update this document with your new expiry date and any changes to the process 


| Date updated | Expiry |
|--|--|
| 25/06/21 | 25/12/21  |
| 07/12/21 | 01/01/23  |
