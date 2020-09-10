#### Parser Content
```Java
{
Name = xml-microsoft-dns-query
  Vendor = Microsoft
  Product = Microsoft Windows DNSServer
  Lms = Direct
  DataType = "dns-query"
  IsHVF = true
  TimeFormat = "yyyy-MM-dd'T'HH:mm:ss.SSSSSSSSSZ"
  Conditions = [ """<Data Name='QNAME'>""", """<Data Name='QTYPE'>""", """<Data Name='Flags'>""" ]
  Fields = [
    """<TimeCreated SystemTime='({time}\d\d\d\d-\d\d-\d\dT\d\d:\d\d:\d\d\.\d{9}Z)""",
    """<Computer>({host}.+?)<\/Computer>""",
    """<EventID>({event_code}\d+)<\/EventID>""",
    """<Execution ProcessID='({pid}\d+)""",
    """<Data Name='XID'>({query_id}\d+)""",
    """ThreadID='({thread_id}[^\']+)""",
    """<Data Name='InterfaceIP'>({dest_ip}[A-Fa-f:\d.]+)""",
    """<Data Name='Source'>({src_ip}[A-Fa-f:\d.]+)""",
    """<Data Name='Port'>({src_port}\d+)""",
    """<Data Name='QNAME'>({query}.+?({top_query}\w+.(?i)(com|net|info|edu|org|gov|co|jp|ru|de|ir|it|in|fr|info|pl|nl|es|gr|cz|eu|tv|me|jp|ca|cn|uk|my|cc|id|us|nz|biz|club|io|gg|fi|au|st|tw|asia|sg|ie|li|za)\.))<\/Data>""",
    """<Data Name='QTYPE'>({query_type}.+?)<\/Data>""",
    """<Data Name='Flags'>({query_flags}.+?)<\/Data>""",
    """<Data Name='BufferSize'>({bytes}\d+)<\/Data>""",
  ]
}
```