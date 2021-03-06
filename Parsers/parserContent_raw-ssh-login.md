#### Parser Content
```Java
{
Name = raw-ssh-login
  Vendor = Unix
  Product = Unix
  Lms = Direct
  DataType = "ssh-login"
  TimeFormat = "yyyy-MM-dd HH:mm:ss"
  Conditions = [ """ssh""", """Accepted """, """ for """, """ from """ ]
  Fields = [
    """exabeam_time=({time}\d\d\d\d-\d\d-\d\d \d\d:\d\d:\d\d)""",
    """exabeam_host=([^=]+@\s*)?(::ffff:)?({host}[^\s]+)""",
    """exabeam_host=([^=]+@\s*)?(::ffff:)?(({dest_ip}\d{1,3}.\d{1,3}.\d{1,3}.\d{1,3})|({dest_host}[^\s]+))""",
    """<({time}\d+\s+\w+\s+\d+\s+\d+:\d+:\d+)\s""",
    """\d\d:\d\d:\d\d \d\d\d\d ({host}[^\s]+)""",
    """\d\d:\d\d:\d\d \d\d\d\d ({dest_host}[^\s]+)""",
    """\s(::ffff:)?(({dest_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})|({dest_host}[\w\.-]+)):?\s+sshd\[""",
    """\d{2}:\d{2}:\d{2}\s+(::ffff:)?({dest_host}[\w\.-]+)\s+auth\|""",
    """Accepted ({auth}\S+) for (({domain}[^\\:]+)\\+)?({user}[\w.'\-\\$]+)(\s|$)""",
    """\s+from\s+(::ffff:)?({src_ip}[:0-9a-fA-F\.]+)""",
    """\s+from\s+(::[\w]+:)?({src_ip}\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})""",
    """(::ffff:)?({host}[\w.\-]+) sshd ({logon_id}\d+)""",
    """(::ffff:)?({host}[\w\.\-]+):\s+sshd\[""",
    """sshd\[({logon_id}\d+)""",
    """({event_code}ssh)""",
    """\d+\s+\w+\s+\d+\s+\d+:\d+:\d+\s+\w+>\s+<(::ffff:)?({dest_host}[\w\-.]+)""",
  ]
  DupFields = ["dest_host->original_dest_host"]
}
```