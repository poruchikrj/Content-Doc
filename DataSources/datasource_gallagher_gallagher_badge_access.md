Vendor: Gallagher
=================
Product: Gallagher Badge Access
-------------------------------
| Rules | Models | MITRE TTPs | Event Types | Parsers |
|:-----:|:------:|:----------:|:-----------:|:-------:|
|   2   |   1    |     1      |      2      |    2    |

|               Use-Case                | Activity Types                                                 | Event Types/Parsers                                                                                                                                                                                                                     | MITRE TTP                  | Content                                             |
|:-------------------------------------:| -------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------- | --------------------------------------------------- |
| [Other](../UseCases/usecase_other.md) | <ul><li>Activity Time  and Type</li><li>Badge Access</li></ul> |  failed-physical-access<br> ↳ [gallagher-badge-access-denied](../Parsers/parserContent_gallagher-badge-access-denied.md)<br><br> physical-access<br> ↳ [gallagher-badge-access](../Parsers/parserContent_gallagher-badge-access.md)<br> | T1078 - Valid Accounts<br> | <ul><li>2 Rules</li></ul><ul><li>1 Models</li></ul> |

ATT&CK Matrix for Enterprise
----------------------------
| Initial Access                                                      | Execution | Persistence                                                         | Privilege Escalation                                                | Defense Evasion                                                     | Credential Access | Discovery | Lateral Movement | Collection | Command and Control | Exfiltration | Impact |
| ------------------------------------------------------------------- | --------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------- | ---------------- | ---------- | ------------------- | ------------ | ------ |
| [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |           | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> | [Valid Accounts](https://attack.mitre.org/techniques/T1078)<br><br> |                   |           |                  |            |                     |              |        |