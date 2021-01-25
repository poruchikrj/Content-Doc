Vendor: Check Point
===================
Product: Check Point NGFW
-------------------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|  151  |   31   |     15     |      9      |    9    |

|               Use-Case                | Activity Types                                                                                                                                                                                                                                                                                                                                                                                                                                | Event Types/Parsers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | MITRE TTP                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                | Content                                                |
|:-------------------------------------:| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------ |
| [Other](../UseCases/usecase_other.md) | <ul><li>Activity Time  and Type</li><li>Application Activity</li><li>Asset Logon and Access</li><li>Credential Switch Activity</li><li>Critical System Activity</li><li>Data Loss Prevention</li><li>Email Activity</li><li>Endpoint Activity</li><li>Network</li><li>Network Alert</li><li>Network zones and Location Access</li><li>Process Activity</li><li>Security Alert</li><li>Service Account Activity</li><li>Web Activity</li></ul> |  app-login<br> ↳ [smartdashboard-app-login](../Parsers/parserContent_smartdashboard-app-login.md)<br> ↳ [syslog-checkpoint-app-login-1](../Parsers/parserContent_syslog-checkpoint-app-login-1.md)<br> ↳ [syslog-checkpoint-app-login](../Parsers/parserContent_syslog-checkpoint-app-login.md)<br><br> dlp-email-alert-in<br> ↳ [checkpoint-dlp-email-alert](../Parsers/parserContent_checkpoint-dlp-email-alert.md)<br><br> dlp-email-alert-out<br> ↳ [checkpoint-dlp-alert-out](../Parsers/parserContent_checkpoint-dlp-alert-out.md)<br><br> local-logon<br> ↳ [checkpoint-local-logon](../Parsers/parserContent_checkpoint-local-logon.md)<br><br> network-alert<br> ↳ [checkpoint-network-alert-3](../Parsers/parserContent_checkpoint-network-alert-3.md)<br> ↳ [checkpoint-vpn-firewall](../Parsers/parserContent_checkpoint-vpn-firewall.md)<br><br> network-connection-failed<br> ↳ [checkpoint-firewall-drop](../Parsers/parserContent_checkpoint-firewall-drop.md)<br> ↳ [checkpoint-firewall-network-connection-drop](../Parsers/parserContent_checkpoint-firewall-network-connection-drop.md)<br> ↳ [s-checkpoint-firewall-drop](../Parsers/parserContent_s-checkpoint-firewall-drop.md)<br><br> network-connection-successful<br> ↳ [checkpoint-firewall-accept](../Parsers/parserContent_checkpoint-firewall-accept.md)<br> ↳ [checkpoint-5599-network-connection](../Parsers/parserContent_checkpoint-5599-network-connection.md)<br> ↳ [raw-checkpoint-firewall-allow](../Parsers/parserContent_raw-checkpoint-firewall-allow.md)<br> ↳ [s-checkpoint-firewall-accept](../Parsers/parserContent_s-checkpoint-firewall-accept.md)<br> ↳ [checkpoint-firewall-network-connection-accept](../Parsers/parserContent_checkpoint-firewall-network-connection-accept.md)<br><br> web-activity-allowed<br> ↳ [s-checkpoint-proxy](../Parsers/parserContent_s-checkpoint-proxy.md)<br> ↳ [checkpoint-url-filtering](../Parsers/parserContent_checkpoint-url-filtering.md)<br> ↳ [checkpoint-proxy](../Parsers/parserContent_checkpoint-proxy.md)<br> ↳ [checkpoint-proxy-2](../Parsers/parserContent_checkpoint-proxy-2.md)<br> ↳ [checkpoint-firewall-allow-2](../Parsers/parserContent_checkpoint-firewall-allow-2.md)<br> ↳ [checkpoint-proxy-1](../Parsers/parserContent_checkpoint-proxy-1.md)<br> ↳ [checkpoint-web-activity](../Parsers/parserContent_checkpoint-web-activity.md)<br><br> web-activity-denied<br> ↳ [s-checkpoint-proxy](../Parsers/parserContent_s-checkpoint-proxy.md)<br> ↳ [checkpoint-url-filtering](../Parsers/parserContent_checkpoint-url-filtering.md)<br> ↳ [checkpoint-proxy](../Parsers/parserContent_checkpoint-proxy.md)<br> ↳ [checkpoint-proxy-2](../Parsers/parserContent_checkpoint-proxy-2.md)<br> ↳ [checkpoint-proxy-1](../Parsers/parserContent_checkpoint-proxy-1.md)<br> ↳ [checkpoint-web-activity](../Parsers/parserContent_checkpoint-web-activity.md)<br> | T1003 - OS Credential Dumping<br>T1033 - System Owner/User Discovery<br>T1041 - Exfiltration Over C2 Channel<br>T1048 - Exfiltration Over Alternative Protocol<br>T1065 - T1065<br>T1066 - T1066<br>T1068 - Exploitation for Privilege Escalation<br>T1071 - Application Layer Protocol<br>T1078 - Valid Accounts<br>T1102 - Web Service<br>T1133 - External Remote Services<br>T1188 - T1188<br>T1189 - Drive-by Compromise<br>T1204 - User Execution<br>T1213 - Data from Information Repositories<br> | <ul><li>151 Rules</li></ul><ul><li>31 Models</li></ul> |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                                                                                                                                                                           | Execution                                                           | Persistence                                                                                                                                      | Privilege Escalation                                                                                                                                          | Defense Evasion                                                     | Credential Access                                                          | Discovery                                                                        | Lateral Movement | Collection                                                                              | Command and Control                                                                                                                             | Exfiltration                                                                                                                                                                 | Impact |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------------- | ---------------- | --------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------ |
| [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br>[Drive-by Compromise](https://attack.mitre.org/techniques/T1189)<br><br> | [User Execution](https://attack.mitre.org/techniques/T1204)<br><br> | [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br>[Exploitation for Privilege Escalation](https://attack.mitre.org/techniques/T1068)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [OS Credential Dumping](https://attack.mitre.org/techniques/T1003)<br><br> | [System Owner/User Discovery](https://attack.mitre.org/techniques/T1033)<br><br> |                  | [Data from Information Repositories](https://attack.mitre.org/techniques/T1213)<br><br> | [Web Service](https://attack.mitre.org/techniques/T1102)<br><br>[Application Layer Protocol](https://attack.mitre.org/techniques/T1071)<br><br> | [Exfiltration Over Alternative Protocol](https://attack.mitre.org/techniques/T1048)<br><br>[Exfiltration Over C2 Channel](https://attack.mitre.org/techniques/T1041)<br><br> |        |