# JWIPacket
JWIPacket Structure
===================
JWIPacket is JSON stored fields. 
JWIPacket example:
```json
{
  "function": "PrintStream/println", 
  "arguments": [
    "Hello World!"
  ]
}
```
------
JWIPacket fields
===================
`function` is field that contains function to execute. 
------
`arguments` is field that contains arguments for `function`.