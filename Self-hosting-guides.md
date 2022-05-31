# Katsushika Self-hosting Guide

## 📉 Prerequisites

- [Git](https://git-scm.com/)

- [Node.JS](https://nodejs.org/en/)

- [WebP](https://developers.google.com/speed/webp/download)

- [FFMpeg](https://ffmpeg.org/download.html)

- [ImageMagick-Legacy](https://imagemagick.org/index.php)

## 🗂 Installation

Run the following code to clone the repo

```SH

> git clone https://github.com/Issa2001/Katsushika

> cd Katsushika

```

Run this to install the depencencies

```SH

> npm i && npm i -D

```

or

```SH

> npm ci

```

## 🏷 Configuration

Create a file named `.env` then add the following fields

```env

PREFIX=:,#/$&-!?

SESSION=add any name that you won't forget.

MONGO_URI=mongodb://addYourUrl

MODS=[]

GOOGLE_API_KEY=addYourKey

CRON=null

CHAT_BOT_URL=yourUrl

TENOR_API_KEY=yourApi

GENIUS_KEY=yourLyricsKey

MAL_USERNAME=yourUsername

MAL_PASSWORD=yourPassword

```

`PREFIX` The Prefix of the Bot <br>

`SESSION` A string to keep track of your session.

`MODS` The phone numbers of users wo you want to be the bot's Admins separated by a comma and must the numbers must be in the following format: `[cc][number]`. eg: `1615******`<br>

`GOOGLE_API` An API key for google.

`CRON` Used for clearing chats.(Not recommended)

`CHAT_BOT_URL` Your chat bot url.

`TENOR_API` Your API key for searching gifs.

`GENIUS_KEY` Your API key for fetching lyrics.

`MAL_USERNAME` Username for your myanimelist account.

`MAL_PASSWORD` Password for your myanimelist account.

`MONGO_URI` is the Connection URL to your DB

To get the connection URL there are two ways

#1 [Mongo Atlas](http://mongodb.com/cloud/atlas) and create an account \

After you set up your account create a new Cluster \

Then copy the connection url to your cluster

([Mongo-Atlas-Guide](https://github.com/Issa2001/Katsushika-guides/blob/main/Mongo-Atlas-guide.md))

a#2 If you don't want to use Mongo Atlas you can install MongoDB in your system and use the URI provided in `.env.example`

Follow the instructions [here](https://docs.mongodb.com/manual/installation/) to install MongoDB in your system

`EIF` is the main endpoint of the [Express-is-fun APIs](https://express-is-fun.herokuapp.com/api). \

If you want the chatbot functionality add this url there: `https://express-is-fun.herokuapp.com`. Leave it empty if you don't want the chatbot functionality

`ADMIN_GROUP_JID` If this field is provided, the members of this group will automatically become admins (use the command `id` to get the jid)

## ⌨ Building

Run `npm run build` and the Compiled JS files, Deceleration Files, Maps and Declaration Maps with their folder will appear in the `dist` folder

## 💻 Running

```SH

npm start

```

Running the above command will start the bot. 

To authenticate scan the QR which shows up in the terminal or the link which is logged when the QR event fires using the WA-Web Scanner on your WhatsApp.

Now you're on your own. Good Luck!

## Don't want to do the hassle of setting up on your own PC?

[Set it up on Heroku](https://github.com/Issa2001/AsunaBotto-guides/blob/main/Heroku-Deploy-Guide.md)

