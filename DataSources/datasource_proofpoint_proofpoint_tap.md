Vendor: Proofpoint
==================
Product: Proofpoint TAP
-----------------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   1   |   1    |     1      |      2      |    2    |

|                                 Use-Case                                  | Activity Types                             | Event Types/Parsers                                                                                                                                                                                                                                                                                                    | MITRE TTP                  | Content                   |
|:-------------------------------------------------------------------------:| ------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------- | ------------------------- |
| [Compromised Credentials](../UseCases/usecase_compromised_credentials.md) | <ul><li>Critical System Activity</li></ul> |  dlp-email-alert-in<br> ↳ [s-proofpoint-email-in](../Parsers/parserContent_s-proofpoint-email-in.md)<br><br> dlp-email-alert-in-failed<br> ↳ [s-proofpoint-email-alert-3](../Parsers/parserContent_s-proofpoint-email-alert-3.md)<br> ↳ [s-proofpoint-email-in](../Parsers/parserContent_s-proofpoint-email-in.md)<br> | T1078 - Valid Accounts<br> | <ul><li>1 Rules</li></ul> |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                      | Execution | Persistence                                                         | Privilege Escalation                                                | Defense Evasion                                                     | Credential Access | Discovery | Lateral Movement | Collection | Command and Control | Exfiltration | Impact |
| ------------------------------------------------------------------- | --------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------- | ---------------- | ---------- | ------------------- | ------------ | ------ |
| [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |           | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |                   |           |                  |            |                     |              |        |