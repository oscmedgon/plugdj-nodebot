plugdj-nodebot
==============

A [Plug.dj](https://plug.dj/) bot which allow you to do multiple moderations actions faster. It also moderate the room when no admins are here. It is open-source so you can edit it like you want.

##How to use it ?
* The bot needs [Node.js](http://nodejs.org/) to work.
* The bot uses [PlugAPI](https://github.com/plugCubed/plugAPI) so you'll need it before running the bot.
* After it, you need to download the bot. The entire bot is in the nodebot.js
* Now, open the nodebot.js file and add the name of your room (only the name __without the /__ ), the email of the bot account and it password.
* The bot should now be connected to your room and will detect commands starting by __!__

___Note___: If you want to automatically restart the bot on crash, you can use [forever](https://github.com/indexzero/forever) or [pm2](https://github.com/Unitech/pm2).

##List of commands
* __!ban__ _(username[,time,reason])_: Ban an user. __Time__ should only be __h__ _for an hour (60minutes)_, __d__ _for a day (24hours)_ or __f__ _forever (Long long time)_. __Reason__ should only be __spam/troll/abuse/offensive/badsong/badtheme/negative__. Default time is Forever and default reason is Spam/Troll. (___Manager to Host___).
* __!commands__: Show a link to this readme.
* __!link__: Send the link of the current song in the chat (___Current DJ or Resident DJ to Host___).
* __!restart__: Restart the bot (Don't work if the bot crashed). (___Manager to Host___).
* __!skip__: Forceskip the song if your rank is highest than Resident DJ or if you're DJ (___Current DJ or Bouncer to Host___). If you're not, it start a vote to skip (___None to Resident DJ___).
* __!unban__ _(username)_: Unban an user. (___Manager to Host___).

_New commands are coming soon, let me know if you want another command._

##License
_This bot is under GNU GENERAL PUBLIC LICENSE, more informations [here](https://github.com/Moutard3/plugdj-nodebot/blob/master/LICENSE)_
