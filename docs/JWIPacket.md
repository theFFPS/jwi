# JWIPacket
JWIPacket Structure
===================
JWIPacket is JSON stored fields. 
JWIPacket example:
```json
{
  "function": "PrintStream/println", 
  "jwi_id": "$jwiID",
  "arguments": [
    "Hello World!"
  ]
}
```
------
JWIPacket fields
===================
`function` is field that contains function to execute. `String`
```sh
```
`arguments` is field that contains arguments for `function`. `List`