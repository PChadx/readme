https://github.com/PChadx/NewWorld/blob/main/README.md

##What the bot does

##Important 
When the bot is added to a group, when he's added he will create his own settings for that group, and
also will mark that group as Home. Home is used for the place where the bot looks, this is where
he finds all the chats he was added in [useful for raid, thor and mthor].


Bot reacts to the following commands:
Conditions: One must be an admin to trigger these three. 

#In groups:

`!raid` - turns raid value on and off. when on everyone will be banned from entering the group.
Users are banned for 60 seconds, everytime group members send messages to the chat , the bot listents to messages it also checks the banned under raid list; if > 60 seconds then it unbans specific users. 

If a banned user would try to enter the chat again under raid ( after being unbanned ), he will be banned again and clock resets for him. Representation: 🛡️⚔️

`!thor` - reply to a user's message and ban him from all the chats where the bot lives.
There is no automatic unban from this. Has no timer.

Representation: Thor⚡️ `thor power aka ban` 🔥 `burned in all chats, like spies do` 🔨 `hammer`

`!loki` - reply to a user's message with mute him in all the chats where the bot lives.
Extra nice consequence: if he happens to enter a chat where he wasn't part of when you used this command
then he is muted there because BOT was living there, when bot presents him with captcha 
he won't be able to complete it and will be banned. Can take a timer, if not it will mute for over 643k days.

Representation 🙊 `mute` 🔥 `burned in all chats, like spies do` 🔨 `hammer`
Example of command : `!loki 1 month now go ahead and think about what you were saying`

`!captcha Normal` - THis sets the captcha to normal old one.

`!captcha Hexagons` - This sets the captcha to the Hexagons one.

`!captcha NONE` - This will make the bot ignore newcomers and not show them captcha nor add them in candidates list. useful for when other bots do that. (default)

When a user enters the chat, it wil be presented with a captcha to resolve. If captcha resolved succesfully does not happen in 60 seconds user will be banned. If resolved succesfully captcha message will be deleted and user greeted. 

`#report` reply to a users message and it will forward the message and create a report card in the logs group 
that is tied to the main group.
example of command `#report you should not say that` or `you should not say that, i am #reporting you`

`#warn` reply to a users message and it will warn them. 3 warnings and user gets banned and warning count reset. this will also forward the msg to replied to. if you want to make a note withm more info you coul use it this way `#warn You should not say this , this the the 3rd time in a row bro` or `ok f**** this shit, you get a #warn for being an asshole again`

`#dwarn` reply to a users message and it will take decrement 1 warn

`#clear` reply to a users message and it will clear warnings

You'll also see `FullWarnings` in bot announcements, this represents how many times the user got to 3 warnings,
for example `[FullWarnings 2]` means user go a total of 3 warnings twice; it is similar to level resets in MMOPRG's

#In Private:
- sending a forwarded message will get you the user's ID subject to his security/privacy settings.

`!setlogs IDchat1 IDchat2` - where IDchat2 repesents the ID of the chat where the logs whould be sent and IDchat1 is the group from where the bot gets his actions.
    If the bot is not admin in `IDchat1` he won't go forward.
    If you are not admin of `IDchat1` he won't go forward.
    If he is not a member of `IDchat2` he will go forward but will remind you to make him one.
IDchat1 and IDchat2 are the numerical values of the chats and start wuth -100

`!HEX` - JUST TESTING captcha 

Note that commands are not case sensitive.

Quick steps: 
1. add bot to group
2. make bot admin
3. set logs by going in private message with the bot ( no need for this anymore , defaults to HEXterminator Actions grup id)

Nice to have in the future: 
`!setRHgroup` - command that will make the group known to the bot as a RH one. will only be possible to set 
if the admin is an admin in one of the RH groups. as an initial seed:
```
// -1001258350810 @PulseChainCom
// -1001637711044 @PulseXCom
// -1001281663801 @HEXSecurity
// -1001232515634 @HEXTrading
// -1001213498543 @HEXcrypto
```  

Notes:
Enable the mongod service to start automatically on boot by running the following command:
`sudo systemctl enable mongod`

Install pm2 
`npm install pm2 -g`

Enable PM2 watch mode, which restarts webhook-vps.js automatically when changes are made to its source code
`pm2 start webhook-vps.js -i 1 --watch`

Enable automatic restarts if the Node.js app errors out, run:
`pm2 startup`
[PM2] Freeze a process list on reboot via:
$ `pm2 save`

[PM2] Remove init script via:
$ `pm2 unstartup systemd`
