# test-asset-nessus-windows-credentialed-scan

### Sample Windows Credentialed Scan

Sample asset for a Nessus credentialed scan against a Windows target.
This asset is not designed to work out of the box, you must download 
it and add your own credentials.

This asset is designed to run a sample credentialed Nessus scan against
a Windows host.  To use this sample, either download it and make it your 
own by editing the credentials in the `scripts/nessus-credentials.txt` file.

For a detailed description of Nessus scan assets, see the sample Nessus Test 
Asset [here on Github](https://github.com/cons3rt/test-asset-nessus-security-scan).

## Usage

* Ensure the admin user's credentials are set properly on the Windows target 
* Clone or download this project locally
* Edit the `scripts/nessus-credentials.txt` files with your desired Windows administrator username/password

```
credential_type=WINDOWS_PASSWORD
username={REPLACE_WINDOWS_ADMIN_USERNAME}
password={REPLACE_WINDOWS_ADMIN_PASSWORD}
```

* Update the `name` and `description` to the `asset.properties` file
* Create a zip file and import your Test Asset under the "Tests" category in CONS3RT
* For launching a deployment with your Nessus Test asset, see [here](https://github.com/cons3rt/test-asset-nessus-security-scan#launch-a-nessus-scan)
* For setting `nessus.targets` and other customer properties, see [here](https://github.com/cons3rt/test-asset-nessus-security-scan#custom-properties)
* For test results, see [here](https://github.com/cons3rt/test-asset-nessus-security-scan#custom-properties)
