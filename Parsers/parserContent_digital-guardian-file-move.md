#### Parser Content
```Java
{
Name = digital-guardian-file-move
  Product = Digital Guardian Endpoint Protection
  DataType = "file-write"
  Conditions = [ """ Agent_Local_Time="""", """ User_Name="""", """ Operation="12"""" ]
  Fields = ${DGParserTemplates.digital-guardian-activity.Fields}[
  ]
}
```