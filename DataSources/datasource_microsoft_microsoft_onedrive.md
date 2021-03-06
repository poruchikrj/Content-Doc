Vendor: Microsoft
=================
Product: Microsoft OneDrive
---------------------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   4   |   3    |     2      |      1      |    1    |

|                                 Use-Case                                  | Activity Types                                                   | Event Types/Parsers                                                                                       | MITRE TTP                                                          | Content                                             |
|:-------------------------------------------------------------------------:| ---------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ | --------------------------------------------------- |
| [Compromised Credentials](../UseCases/usecase_compromised_credentials.md) | <ul><li>Critical System Activity</li><li>File Activity</li></ul> |  file-read<br> ↳ [cef-onedrive-file-activity](../Parsers/parserContent_cef-onedrive-file-activity.md)<br> | T1078 - Valid Accounts<br>T1083 - File and Directory Discovery<br> | <ul><li>3 Rules</li></ul><ul><li>2 Models</li></ul> |
|       [Data Exfiltration](../UseCases/usecase_data_exfiltration.md)       | <ul><li>File Activity</li></ul>                                  |  file-read<br> ↳ [cef-onedrive-file-activity](../Parsers/parserContent_cef-onedrive-file-activity.md)<br> | T1083 - File and Directory Discovery<br>                           | <ul><li>3 Rules</li></ul><ul><li>3 Models</li></ul> |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                      | Execution | Persistence                                                         | Privilege Escalation                                                | Defense Evasion                                                     | Credential Access | Discovery                                                                         | Lateral Movement | Collection | Command and Control | Exfiltration | Impact |
| ------------------------------------------------------------------- | --------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------------------------------------------------------------------------------- | ---------------- | ---------- | ------------------- | ------------ | ------ |
| [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |           | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |                   | [File and Directory Discovery](https://attack.mitre.org/techniques/T1083)<br><br> |                  |            |                     |              |        |