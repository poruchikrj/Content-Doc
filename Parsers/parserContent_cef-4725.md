#### Parser Content
```Java
{
Name = cef-4725
    Vendor = Microsoft
    Product = Microsoft Windows
    Lms = ArcSight
    DataType = "windows-account-disabled"
    TimeFormat = "epoch"
    Conditions = [ """|Microsoft|Microsoft Windows|""","""|Microsoft-Windows-Security-Auditing:4725|""" ]
    Fields = [ """exabeam_EventTime=({eventtime}\d+)""",
      """({event_name}A user account was disabled)""",
      """\sexternalId=({event_code}\d+)""",
      """\srt=({time}\d+)""",
      """\sdvc=({host}[a-fA-F:\d.]+)""",
      """\sdvchost=({host}[^\s]+)""",
      """\sdhost=({dest_host}[^\s]+)""",
      """\sdst=({dest_ip}[a-fA-F:\d.]+)""",
      """\ssuser=({user}.+?)\s+\w+=""",
      """\ssntdom=({domain}.+?)\s\w+=""",
      """\ssuid=({logon_id}[^\s]+)""",
      """\sduser=({target_user}.+?)\s+\w+=""",
      """\sdntdom=({target_domain}.+?)\s\w+=""",
      """Security_,ID=({target_user_sid}[^\s]+)"""
    ]
  }
```