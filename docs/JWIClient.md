# JWIClient
Get [information about JWIPacket](https://github.com/theFFPS/jwi/blob/main/docs/JWIPacket.md)

Creating your own JWIClient
==================
1. Create TCP client application
2. Create packet builder (if you want to make sending packets easier)
3. Get port from "HOME_DIR/.jwi_servers" by parsing JSON and getting port for JWIServer with name of JWIServer. (Use if  server is localhost)
4. Create parser for packets from JWIServer by parsing JSON.
5. Send security packet with security key. 
6. Parse security response.
7. Save jwiID from response.
------
Security packet
==================
```json
{
  "function": "security",
  "arguments": ["$KEY"]
}
```
------
Security response
==================
```json
{
  "jwi_id": "$JWI_ID"
}
```
------
Security values
==================
`Security Key` is key required to get `jwiID`
```sh
```
`jwiID` is required for security of Java application that uses JWI (Generated on server start)