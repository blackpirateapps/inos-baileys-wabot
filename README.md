# inos-baileys-wabot
> WhatsApp Bot Using Baileys Library By InosID!

<p align="center">
<img src="https://gpvc.arturio.dev/InoxID" />
<p/>
<p align="center">
<a href="https://github.com/CxD9-Teams/cxd9-bot/stargazers/"><img title="Stars" src="https://img.shields.io/github/stars/CxD9-Teams/cxd9-bot?&style=flat-square"></a>
<a href="https://github.com/CxD9-Teams/cxd9-bot/network/members"><img title="Fork" src="https://img.shields.io/github/forks/CxD9-Teams/cxd9-bot?style=flat-square"></a>
<a href="https://github.com/CxD9-Teams/cxd9-bot/watchers"><img title="Watching" src="https://img.shields.io/github/watchers/CxD9-Teams/cxd9-bot?label=Watching&style=flat-square"></a>
<a href="https://github.com/CxD9-Teams/cxd9-bot/watchers"><img title="Contributor" src="https://img.shields.io/github/contributors/CxD9-Teams/cxd9-bot?logo=github&style=flat-square"></a>
</p>
<p align="center">
<a href="https://github.com/CxD9-Teams/cxd9-bot"><img src="https://img.shields.io/github/repo-size/CxD9-Teams/cxd9-bot?label=Repo%20size&style=flat-square"></a>
</p>

- [x] **HEROKU APP**

> Heroku Deploy **Beta**

**First deploy bot**, Click the deploy icon below !

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/blackpirateapps/inos-baileys-wabot)

Then click view web.
After that, scan the qr, Done.

- [x] **RDP/VPS USER**

**First download tools**, Click icon to download !

<a href="https://git-scm.com/downloads"><img src="http://img.shields.io/badge/-Git-F1502F?style=flat&logo=git&logoColor=FFFFFF"></a>
<a href="https://nodejs.org/en/download"><img
src="https://img.shields.io/badge/-Node.js-3C873A?style=flat&logo=Node.js&logoColor=white"></a>
<a href="https://ffmpeg.org/download.html"><img src="http://img.shields.io/badge/-Ffmpeg-000000?style=flat&logo=ffmpeg&logoColor=green"></a>
<a href="https://notepad-plus-plus.org/downloads/v8.1.9"><img src="http://img.shields.io/badge/-Notepad++-orange?style=flat"></a>

## Termux/Ubuntu/Linux User
Make sure everything is in good condition

First, install
```bash
• apt install git -y
• apt install ffmpeg -y
• apt install nodejs -y
```

If everything has been confirmed to be safe and installed, continue with the clone repo
```bash
• git clone https://github.com/InosID/inos-baileys-wabot
• mv inos-baileys-wabot inosbot
• cd inosbot
• npm i
• npm start
```
For all questions in the installation just select y 
the second step is to just change the number of the owner of the bot and finally scan the qr code

**Powered By**
<p align="center">
  <a href="https://github.com/InosID">
    <img src="https://github.com/InosID.png?size=100">
  </a>
</p>

***
[![moo-d](https://github.com/moo-d.png)](https://github.com/moo-d) | [![mrfzvx12](https://github.com/mrfzvx12.png)](https://github.com/mrfzvx12) | [![YourAlfabet](https://github.com/youralfabet.png)](https://github.com/YourAlfabet)
--------|--------|--------|
[![Fxc7](https://github.com/fxc7.png)](https://github.com/fxc7) | [![Hadi-Api](https://github.com/hadi-api.png)](https://github.com/hadi-api) | [![Ahmadzakix](https://github.com/Ahmadzakix.png)](https://github.com/Ahmadzakix)
[![Finox999](https://github.com/Finox999.png)](https://github.com/Finox999) | [![Fauzy-Rahadian](https://github.com/fauzy-rahadian.png)](https://github.com/Fauzy-Rahadian) | [![Arifi Razzaq](https://github.com/arifirazzaq2001.png)](https://github.com/arifirazzaq2001)
[![Caliph91](https://github.com/Caliph91.png)](https:github.com/caliph) | [![AffisJunianto](https://github.com/affisjunianto.png)](https://github.com/affisjunianto) | [![Monxnl](https://github.com/Monxnl.png)](https://github.com/Monxnl)

## Group WhatsApp

[Click Here](https://chat.whatsapp.com/KXxyPFoIpRDCbyQWRYVu8G)

## Send Message

#### Send Text Message

```js
let Baileys = require('@adiwajshing/baileys')

// Get message type from Baileys
let { text } = Baileys.MessageType

// Send text
CXD.sendText(from, "Hello World!")

// Send text with reply
CXD.reply("Hello World!")
```

#### Send Image Message

```js
let Baileys = require('@adiwajshing/baileys')
let fs = require('fs')

// Get type from Baileys
let {
  text,
  image
} = Baileys.MessageType

let locationImg = fs.readFileSync('./lib/emror.jpeg')

// Send image
CXD.sendImage(from, locationImg, "This is caption.", false)
/**
 * If you wan't without reply, change the true to false.
 */

// Send image in website
let website = "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQKTvqbVbQdjSx7J6IvfQpk-8iNopG_Ox7UCg&usqp=CAU"

CXD.sendImage(from, website, "This is caption.", true)
/**
 * If you wan't without reply, change the true to false.
 */
```

#### Send File Message

```js
let Baileys = require('@adiwajshing/baileys')

// Get message type from Baileys
let {
  text,
  image,
  document,
  audio,
  video
} = Baileys.MessageType

// Location file
let locationFile = './views/favicon.png'

// Send file
CXD.sendFile(from, locationFile, 'this is caption', true)
/**
 * If you wan't without reply, change the true to false.
 */
```

#### Send File From Url Message

```js
let Baileys = require('@adiwajshing/baileys')

// Get message type from Baileys
let {
  text,
  image,
  document,
  audio,
  video
} = Baileys.MessageType

// Url
urls = 'https://website.com'

// Send file from url
CXD.sendFileFromUrl(from, urls, 'image', "This is caption", true)
/**
 * If you wan't without reply, change the true to false.
 * If the file type is document, change 'image' to 'document' etc.
 */
```

#### Send Button Message

```js
CXD.sendButton(from, "content", "footer", [
  {
    buttonId: `row`
    buttonText: {
      displayText: 'button',
    },
    type: 1,
  },
], { quoted: msg })
```

# Note
> If this script has an error, you can report it via issue.
