#### Parser Content
```Java
{
Name = trend-micro-alert-5
  Vendor = Trend Micro
  Product = OfficeScan
  Lms = Direct
  DataType = "alert"
  TimeFormat = "yyyy-MM-dd HH:mm:ss"
  Conditions = [ """ WFBSS-SVC-AC [LogSpyware""", """Spyware/Grayware""" ]
  Fields = [
    """({host}\S+) WFBSS-SVC-AC""",
    """\d+ ({time}\d\d\d\d\-\d\d\-\d\d \d\d:\d\d:\d\d) \d+\.\d+\.\d+\.\d+""",
    """Device name="({src_host}[^"]+)""",
    """User="({user}[^"]+)""",
    """Spyware="({alert_name}[^"]+)""",
    """Risk Level="({alert_severity}[^"]+)""",
    """Infected Resource="({malware_url}[^"]+)""",
    """\[({alert_type}[^@]+)""",
  ]
}
```