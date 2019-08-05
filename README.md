# GSuiteSkillet
Skillet for securing Google G Suite with the Palo Alto Networks Security Operating Platform.  

### Overview
This Skillet implements the configuration steps listed in the [Deployment Guide for Securing Google G Suite](https://www.paloaltonetworks.com/resources/guides/securing-google-g-suite-deployment-guide).  There are three operations available:
1. Sanction Google G Suite which creates security rules that inspect G Suite application traffic such as Gmail and Google Hangouts.
2. Limit login access to specific G Suite enterprise instances and block access to all other G Suite enterprise and consumer accounts.
3. Block uploads to G Suite for items such as attaching files to Gmail and uploading to Google Docs.

### Assumptions and Prerequisites

- The PAN-OS version tested with this Skillet is 8.1
- Firewalls must be operational. This Skillet only covers the policy specific to G Suite and not the
deployment of the firewalls.
- For optimal results SSL Decryption should be configured.
