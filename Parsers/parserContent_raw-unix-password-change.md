#### Parser Content
```Java
{
Name = raw-unix-password-change
  Vendor = Unix
  Product = Unix
  Lms = Direct
  DataType = "password-change"
  TimeFormat = "yyyy-MM-dd HH:mm:ss"
  Conditions = [ """pam_unix(passwd:chauthtok):""", "password changed for" ]
  Fields = [
    """exabeam_time=({time}\d\d\d\d-\d\d-\d\d \d\d:\d\d:\d\d)""",
    """exabeam_host=({host}[\w.\-]+)""",
    """\d\d:\d\d:\d\d ({host}[\w.\-]+)""",
    """password changed for ({target_user}.+?)\s$""",
  ]
  DupFields = [ "host->dest_host" ]
}
```