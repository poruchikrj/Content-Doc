Vendor: Mimecast
================
Product: Mimecast Email Security
--------------------------------
|                                 Use-Case                                  | Activity Types                                                                                                                                                                                         | Event Types/Parsers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | MITRE TTP                                                                                                                                                                                                                                                                                                                            | Content                    |
|:-------------------------------------------------------------------------:| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------- |
| [Compromised Credentials](../UseCases/usecase_compromised_credentials.md) | - Activity Time  and Type<br>- Application Activity<br>- Asset Logon and Access<br>- Critical System Activity<br>- Email Activity<br>- Network zones and Location Access<br>- Service Account Activity |  app-activity<br> -- [s-mimecast-app-activity](../Parsers/parserContent_s-mimecast-app-activity.md)<br><br> app-login<br> -- [s-mimecast-app-login](../Parsers/parserContent_s-mimecast-app-login.md)<br><br> dlp-email-alert-in<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-in-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-out<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> dlp-email-alert-out-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> failed-app-login<br> -- [cef-mimecast-failed-app-login](../Parsers/parserContent_cef-mimecast-failed-app-login.md)<br> | T1078 - Valid Accounts<br>T1098.002 - Account Manipulation: Exchange Email Delegate Permissions<br>T1133 - External Remote Services<br>                                                                                                                                                                                              |  - 42 Rules<br> - 5 Models |
|       [Data Exfiltration](../UseCases/usecase_data_exfiltration.md)       | - Email Activity                                                                                                                                                                                       |  app-activity<br> -- [s-mimecast-app-activity](../Parsers/parserContent_s-mimecast-app-activity.md)<br><br> app-login<br> -- [s-mimecast-app-login](../Parsers/parserContent_s-mimecast-app-login.md)<br><br> dlp-email-alert-in<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-in-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-out<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> dlp-email-alert-out-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> failed-app-login<br> -- [cef-mimecast-failed-app-login](../Parsers/parserContent_cef-mimecast-failed-app-login.md)<br> | T1020 - Automated Exfiltration<br>T1048 - Exfiltration Over Alternative Protocol<br>T1048.003 - Exfiltration Over Alternative Protocol: Exfiltration Over Unencrypted/Obfuscated Non-C2 Protocol<br>T1098.002 - Account Manipulation: Exchange Email Delegate Permissions<br>T1114.003 - Email Collection: Email Forwarding Rule<br> |  - 40 Rules<br> - 9 Models |
|          [Internal Fraud](../UseCases/usecase_internal_fraud.md)          | - Application Activity                                                                                                                                                                                 |  app-activity<br> -- [s-mimecast-app-activity](../Parsers/parserContent_s-mimecast-app-activity.md)<br><br> app-login<br> -- [s-mimecast-app-login](../Parsers/parserContent_s-mimecast-app-login.md)<br><br> dlp-email-alert-in<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-in-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-out<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> dlp-email-alert-out-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> failed-app-login<br> -- [cef-mimecast-failed-app-login](../Parsers/parserContent_cef-mimecast-failed-app-login.md)<br> | T1078 - Valid Accounts<br>                                                                                                                                                                                                                                                                                                           |  - 13 Rules<br> - 1 Models |
|        [Lateral Movement](../UseCases/usecase_lateral_movement.md)        | - Activity Time  and Type<br>- Application Activity<br>- Network zones and Location Access                                                                                                             |  app-activity<br> -- [s-mimecast-app-activity](../Parsers/parserContent_s-mimecast-app-activity.md)<br><br> app-login<br> -- [s-mimecast-app-login](../Parsers/parserContent_s-mimecast-app-login.md)<br><br> dlp-email-alert-in<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-in-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-out<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> dlp-email-alert-out-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> failed-app-login<br> -- [cef-mimecast-failed-app-login](../Parsers/parserContent_cef-mimecast-failed-app-login.md)<br> | T1078 - Valid Accounts<br>T1133 - External Remote Services<br>                                                                                                                                                                                                                                                                       |  - 7 Rules<br> - 1 Models  |
|       [Malware Detection](../UseCases/usecase_malware_detection.md)       | - Asset Logon and Access                                                                                                                                                                               |  app-activity<br> -- [s-mimecast-app-activity](../Parsers/parserContent_s-mimecast-app-activity.md)<br><br> app-login<br> -- [s-mimecast-app-login](../Parsers/parserContent_s-mimecast-app-login.md)<br><br> dlp-email-alert-in<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-in-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-out<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> dlp-email-alert-out-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> failed-app-login<br> -- [cef-mimecast-failed-app-login](../Parsers/parserContent_cef-mimecast-failed-app-login.md)<br> | T1078 - Valid Accounts<br>T1090.003 - Proxy: Multi-hop Proxy<br>                                                                                                                                                                                                                                                                     |  - 6 Rules<br>             |
|                [Phishing](../UseCases/usecase_phishing.md)                | - Email Activity                                                                                                                                                                                       |  app-activity<br> -- [s-mimecast-app-activity](../Parsers/parserContent_s-mimecast-app-activity.md)<br><br> app-login<br> -- [s-mimecast-app-login](../Parsers/parserContent_s-mimecast-app-login.md)<br><br> dlp-email-alert-in<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-in-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-out<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> dlp-email-alert-out-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> failed-app-login<br> -- [cef-mimecast-failed-app-login](../Parsers/parserContent_cef-mimecast-failed-app-login.md)<br> | T1048 - Exfiltration Over Alternative Protocol<br>T1048.003 - Exfiltration Over Alternative Protocol: Exfiltration Over Unencrypted/Obfuscated Non-C2 Protocol<br>                                                                                                                                                                   |  - 7 Rules<br> - 2 Models  |
|     [Privileged Activity](../UseCases/usecase_privileged_activity.md)     | - Application Activity<br>- Email Activity<br>- Service Account Activity                                                                                                                               |  app-activity<br> -- [s-mimecast-app-activity](../Parsers/parserContent_s-mimecast-app-activity.md)<br><br> app-login<br> -- [s-mimecast-app-login](../Parsers/parserContent_s-mimecast-app-login.md)<br><br> dlp-email-alert-in<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-in-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-out<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> dlp-email-alert-out-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> failed-app-login<br> -- [cef-mimecast-failed-app-login](../Parsers/parserContent_cef-mimecast-failed-app-login.md)<br> | T1078 - Valid Accounts<br>T1098.002 - Account Manipulation: Exchange Email Delegate Permissions<br>                                                                                                                                                                                                                                  |  - 5 Rules<br> - 1 Models  |
|    [Ransomware Detection](../UseCases/usecase_ransomware_detection.md)    | - Asset Logon and Access                                                                                                                                                                               |  app-activity<br> -- [s-mimecast-app-activity](../Parsers/parserContent_s-mimecast-app-activity.md)<br><br> app-login<br> -- [s-mimecast-app-login](../Parsers/parserContent_s-mimecast-app-login.md)<br><br> dlp-email-alert-in<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-in-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br> -- [cef-mimecast-security-alert](../Parsers/parserContent_cef-mimecast-security-alert.md)<br> -- [cef-mimecast-email-alert-1](../Parsers/parserContent_cef-mimecast-email-alert-1.md)<br> -- [cef-mimecast-email-alert](../Parsers/parserContent_cef-mimecast-email-alert.md)<br><br> dlp-email-alert-out<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> dlp-email-alert-out-failed<br> -- [s-mimecast-dlp-email](../Parsers/parserContent_s-mimecast-dlp-email.md)<br><br> failed-app-login<br> -- [cef-mimecast-failed-app-login](../Parsers/parserContent_cef-mimecast-failed-app-login.md)<br> | T1078 - Valid Accounts<br>T1090.003 - Proxy: Multi-hop Proxy<br>                                                                                                                                                                                                                                                                     |  - 6 Rules<br>             |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                                                                                                   | Execution | Persistence                                                                                                                                                                                                                                                                                                                                 | Privilage escalation                                                | Defense evasion                                                     | Credential Access | Discovery | Lateral Movement | Collection                                                                                                                                                            | Command and Control                                                                                                                       | Exfiltration                                                                                                                                                                                                                                                                                                                    | Impact |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------- | ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------ |
| [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |           | [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br>[Account Manipulation](https://attack.mitre.org/techniques/T1098)<br><br>[Account Manipulation: Exchange Email Delegate Permissions](https://attack.mitre.org/techniques/T1098/002)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |                   |           |                  | [Email Collection](https://attack.mitre.org/techniques/T1114)<br><br>[Email Collection: Email Forwarding Rule](https://attack.mitre.org/techniques/T1114/003)<br><br> | [Proxy: Multi-hop Proxy](https://attack.mitre.org/techniques/T1090/003)<br><br>[Proxy](https://attack.mitre.org/techniques/T1090)<br><br> | [Exfiltration Over Alternative Protocol](https://attack.mitre.org/techniques/T1048)<br><br>[Exfiltration Over Alternative Protocol: Exfiltration Over Unencrypted/Obfuscated Non-C2 Protocol](https://attack.mitre.org/techniques/T1048/003)<br><br>[Automated Exfiltration](https://attack.mitre.org/techniques/T1020)<br><br> |        |