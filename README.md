# Updatecheck
- Version 1.0.0
.
- The idea is simpel, it checks the mod.json file on github
- after reading the mod.json files version and reason string
- it reads the version.lua on the server and compares the version tag
- if there is a change it spams the version and reason string and post it in the console.
- THIS part works as it should be.
- This can be false or true
- This extended version has a option that should be useable ingame by invoke the !mod command
- And should post the same output in the chat screen.
- 

- Cooking it in your own mod:
- open your __init file and add this line: 
- -- Check if there is a new version
- require('__shared/UpdateCheck')   
-
- Copy UpdateCheck.lua and version in your shared folder
-
- What is do:
- This wil check if the current version is the same as on github
- 
-These things you need to change in the updatecheck.lua
-
- This contains the string that send out in the console that there is no change in the mod
s_current = ("VU-Pixels_updatecheck seems to be up2date")

- This line contains the message if the mod.json is the difrent on github ,as is the version.lua localy on your server
- s_update = ("VU-Pixels_updatecheck seems to be out of date!")
-
- Make sure this point on github to your mod.json file !
- Example: s_githublink = ("https://raw.githubusercontent.com/-username-/-modname-/main/mod.json")
-
- s_githublink = ("https://raw.githubusercontent.com/-username-/-modname-/main/mod.json")
-
- if you want to know the link to past here
- click on mod.json on github
- click the raw link, and copy that line, and past in s_githublink
-
- Also,, change the @mod check to what u want
- when using this in game, it reply the currect version the server readed on startup
-
- Todo: checking if it send globaly in chat, or to the player
- Todo: Make it so that only admins can use this
