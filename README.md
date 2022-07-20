# UEM Managed Goldmaster Scripts

Samples to prove management of Horizon Gold Masters with UEM.

The install_syncml.xml and remove_syncml.xml files are custom CSPs for setting the Windows Update settings. Place these in a profile in UEM, and modify the target version as needed.

Example run of the script:
``` powershell
powershell.exe -ExecutionPolicy Bypass -file .\GoldMasterEnrollmentPoc.ps1 -ApiUsername administrator -ApiPassword verysecurepassword -UemUrl https://apiauemurl.com -TenantCode uY18y+prmK3Sbob0O5Ljb6ZNldSrvqerB99/3skKTls= -EnrollmentUrl https://dsauemurl.com -EnrollmentUsername enrollinguser -EnrollmentPassword verysecurepassword -EnrollmentOG gldmstr -AgentMsiPath C:\Recovery\OEM\AirwatchAgent.msi
```