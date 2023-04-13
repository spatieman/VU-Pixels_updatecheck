# Updatecheck
- Version 1.0.0
.
- This is a test version, not a release.
- The idea is simpel, it checks the mod.json file
- for changes in the Version string
- after reading the local version.lua file, what contains the local version it compares it.
- if there is a change it reads the Reason string and post it in the console.
- THIS part works as it should be.
- .
- This extended version should be useable ingame by invoke the !mod command
- And should post the same output in the chat screen.
- SHOULD,so this mod is a Work in progress mod.
-- DO NOT YET USE UNLESS YOU DONT CARE ABOUT THE CHAT FUNCTION --

- This is how a mod.json can look like
- 
- {
-     "Name": "Pixels Updatecheck",
-     "Description": "checks the Version on github and compares it with the local version",
-     "Version": "1.0.0",
-     "Reason": "TEST VERSION", 
-     "Authors": [ "iamadeadpixel" ],
-     "HasVeniceEXT": true,
-     "Dependencies": {
-         "veniceext": "^1.0.0"
-      }
- }
- 
- Or edit this mod.json file
