#### Parser Content
```Java
{
Name = pulsesecure-account-deleted
  Vendor = Juniper Networks
  Product = Juniper Networks Pulse Secure
  Lms = Direct
  DataType = "account-deleted"
  TimeFormat = "yyyy-MM-dd HH:mm:ss"
  Conditions = [ """PulseSecure:""", """User Accounts modified.""" ]
  Fields = [
    """PulseSecure:.+?({time}\d\d\d\d-\d\d-\d\d \d\d:\d\d:\d\d) - (::ffff:)?({host}\S+) - \[(::ffff:)?({src_ip}[A-Fa-f:\d.]+)\] (({domain}[^\\]+)\\)?(System|({user}[^\\\/\s\(]+))""", 
    """Removed username (({target_domain}[^\\]+)\\)?({target_user}[^\\\s]+)""",
  ]
  DupFields = [ "target_user->account_name" , "host->dest_host"]
}
```