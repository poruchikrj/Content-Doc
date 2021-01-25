Vendor: F5
==========
Product: Big-IP
---------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|  92   |   17   |     15     |      7      |    7    |

|               Use-Case                | Activity Types                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              | Event Types/Parsers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          | MITRE TTP                                                                                                                                                                                                                                                                                                                                                                                                                                               | Content                                               |
|:-------------------------------------:| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------- |
| [Other](../UseCases/usecase_other.md) | <ul><li>Activity Time  and Type</li><li>Application Activity</li><li>Asset Logon and Access</li><li>Credential Switch Activity</li><li>Data Loss Prevention</li><li>Email Activity</li><li>Endpoint Activity</li><li>Executives</li><li>Failed Logon and Account Lockout</li><li>Network zones and Location Access</li><li>Pass The Hash and Golden Ticket</li><li>Privileged Activity</li><li>Process Activity</li><li>Security Operations</li><li>Service Account Activity</li><li>VPN Activity</li></ul> |  <br> ↳ [f5-vpn-policy](../Parsers/parserContent_f5-vpn-policy.md)<br> ↳ [f5-vpn-additional-info](../Parsers/parserContent_f5-vpn-additional-info.md)<br> ↳ [f5-vpn-user-agent](../Parsers/parserContent_f5-vpn-user-agent.md)<br> ↳ [f5-vpn-username](../Parsers/parserContent_f5-vpn-username.md)<br> ↳ [f5-vpn-policy](../Parsers/parserContent_f5-vpn-policy.md)<br> ↳ [f5-vpn-additional-info](../Parsers/parserContent_f5-vpn-additional-info.md)<br> ↳ [f5-vpn-user-agent](../Parsers/parserContent_f5-vpn-user-agent.md)<br> ↳ [f5-vpn-username](../Parsers/parserContent_f5-vpn-username.md)<br><br> authentication-failed<br> ↳ [f5-vpn-auth-failed](../Parsers/parserContent_f5-vpn-auth-failed.md)<br><br> failed-logon<br> ↳ [f5-ssh-failed-logon](../Parsers/parserContent_f5-ssh-failed-logon.md)<br><br> failed-vpn-login<br> ↳ [f5-vpn-login-failed](../Parsers/parserContent_f5-vpn-login-failed.md)<br><br> remote-logon<br> ↳ [f5-ssh-login-successful](../Parsers/parserContent_f5-ssh-login-successful.md)<br><br> vpn-login<br> ↳ [f5-vpn-assign-ip](../Parsers/parserContent_f5-vpn-assign-ip.md)<br> ↳ [f5-vpn-session-start](../Parsers/parserContent_f5-vpn-session-start.md)<br> ↳ [cef-f5-vpn-start-1](../Parsers/parserContent_cef-f5-vpn-start-1.md)<br> ↳ [f5-vpn-session-start](../Parsers/parserContent_f5-vpn-session-start.md)<br><br> vpn-logout<br> ↳ [cef-f5-vpn-end](../Parsers/parserContent_cef-f5-vpn-end.md)<br> | T1003 - OS Credential Dumping<br>T1021 - Remote Services<br>T1033 - System Owner/User Discovery<br>T1048 - Exfiltration Over Alternative Protocol<br>T1052 - Exfiltration Over Physical Medium<br>T1068 - Exploitation for Privilege Escalation<br>T1075 - T1075<br>T1076 - T1076<br>T1078 - Valid Accounts<br>T1097 - T1097<br>T1110 - Brute Force<br>T1133 - External Remote Services<br>T1188 - T1188<br>T1204 - User Execution<br>T1208 - T1208<br> | <ul><li>92 Rules</li></ul><ul><li>17 Models</li></ul> |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                                                                                                   | Execution                                                           | Persistence                                                                                                                                      | Privilege Escalation                                                                                                                                          | Defense Evasion                                                     | Credential Access                                                                                                                          | Discovery                                                                        | Lateral Movement                                                     | Collection | Command and Control | Exfiltration                                                                                                                                                                      | Impact |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------- | -------------------------------------------------------------------- | ---------- | ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------ |
| [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [User Execution](https://attack.mitre.org/techniques/T1204)<br><br> | [External Remote Services](https://attack.mitre.org/techniques/T1133)<br><br>[Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br>[Exploitation for Privilege Escalation](https://attack.mitre.org/techniques/T1068)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [OS Credential Dumping](https://attack.mitre.org/techniques/T1003)<br><br>[Brute Force](https://attack.mitre.org/techniques/T1110)<br><br> | [System Owner/User Discovery](https://attack.mitre.org/techniques/T1033)<br><br> | [Remote Services](https://attack.mitre.org/techniques/T1021)<br><br> |            |                     | [Exfiltration Over Alternative Protocol](https://attack.mitre.org/techniques/T1048)<br><br>[Exfiltration Over Physical Medium](https://attack.mitre.org/techniques/T1052)<br><br> |        |