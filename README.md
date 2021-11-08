# Telegram VCVideoPlayBot

- An Telegram Bot By [@shukurenai007](https://t.me/shukurenai007) To Stream Videos in Telegram Voice Chat.

---

## NOTE:

- Make sure you have started a VoiceChat in your Group/Channel before deploying.

---

## Features

<details>
  <summary><b>Show the Features</b></summary>
<br/>

- Playlist, queue.
- Supports Video Recording.
- Supports Scheduling voicechats.
- Cool UI for controling the player.
- Customizabe to audio or video.
- Custom quality for video chats.
- Supports Play from Youtube Playlist.
- Change VoiceChat title to current playing song name.
- Supports Live streaming from youtube
- Play from telegram file supported.
- Starts Radio after if no songs in playlist.
- Automatic restart even if heroku restarts. (Configurable)
- Support exporting and importing playlist.

</details>

---

## Variables
<details>
  <summary><b>See Variables</b></summary>
<br/>

<b>Mandatory Vars</b>
1. `API_ID` : Get From [my.telegram.org](https://my.telegram.org/)
2. `API_HASH` : Get from [my.telegram.org](https://my.telegram.org)
3. `BOT_TOKEN` : [@Botfather](https://telegram.dog/BotFather)
4. `SESSION_STRING` : Generate From here [![GenerateStringName](https://img.shields.io/badge/repl.it-generateStringName-yellowgreen)](https://replit.com/@shukurenaibotcr/GenerateStringSession-1)
5. `CHAT` : ID of Channel/Group where the bot plays Music.

<b>Recommended Optional Vars</b>
1. `DATABASE_URI`: MongoDB database Url, get from [mongodb](https://cloud.mongodb.com). This is an optional var, but it is recomonded to use this to experiance the full features.
2. `HEROKU_API_KEY`: Your heroku api key. Get one from [here](https://dashboard.heroku.com/account/applications/authorizations/new)
3. `HEROKU_APP_NAME`: Your heroku apps name.

<b>Optional Vars</b>
1. `LOG_GROUP` : Group to send Playlist, if CHAT is a Group()
2. `ADMINS` : ID of users who can use admin commands.
3. `STARTUP_STREAM` : This will be streamed on startups and restarts of bot. You can use either any STREAM_URL or a direct link of any video or a Youtube Live link. You can also use YouTube Playlist.Find a Telegram Link for your playlist from [PlayList Dumb](https://telegram.dog/DumpPlaylist) or get a PlayList from [PlayList Extract](https://telegram.dog/GetAPlaylistbot). The PlayList link should in form `https://t.me/DumpPlaylist/xxx`.
4. `REPLY_MESSAGE` : A reply to those who message the USER account in PM. Leave it blank if you do not need this feature. (Configurable through bot if mongodb added.)
5. `ADMIN_ONLY` : Pass `True` If you want to make /play command only for admins of `CHAT`. By default /play is available for all.(Configurable through bot if mongodb added.)
6. `DATABASE_NAME`: Database name for your mongodb database.
7. `SHUFFLE` : Make it `False` if you dont want to shuffle playlists. (Configurable through bot if mongodb added.)
8. `EDIT_TITLE` : Make it `False` if you do not want the bot to edit video chat title according to playing song. (Configurable through bot if mongodb added.)
9. `RECORDING_DUMP` : A Channel ID with the USER account as admin, to dump video chat recordings.
10. `RECORDING_TITLE`: A custom title for your videochat recordings.
11. `TIME_ZONE` : Time Zone of your country, by default IST
12. `IS_VIDEO_RECORD` : Make it `False` if you do not want to record video, and only audio will be recorded.(Configurable through bot if mongodb added.)
13. `IS_LOOP` ; Make it `False` if you do not want 24 / 7 Video Chat. (Configurable through bot if mongodb added.)
14. `IS_VIDEO` : Make it `False` if you want to use the player as a musicplayer without video. (Configurable through bot if mongodb added.)
15. `PORTRAIT`: Make it `True` if you want the video recording in portrait mode. (Configurable through bot if mongodb added.)
16. `DELAY` : Choose the time limit for commands deletion. 10 sec by default.
18. `QUALITY` : Customize the quality of video chat, use one of `high`, `medium`, `low` . 
19. `BITRATE` : Bitrate of audio (Not recommended to change).
20. `FPS` : Fps of video to be played (Not recommended to change.)

</details>

---

## Deploy Now

<details><summary><b>Deploy to Heroku</b></summary>
<p>
<br>
<a href="https://heroku.com/deploy?template=https://github.com/shukurenaibotcreate/VCVideoPlayerBot">
  <img src="https://www.herokucdn.com/deploy/button.svg" alt="Deploy">
</a>
</p>
</details>

<details>
  <summary><b>Deploy to Railway</b></summary>
<br/>

<p align="left">
<a href="https://railway.app/new/template?template=https%3A%2F%2Fgithub.com%2Fshukurenaibotcreate%2FVCVideoPlayerBot"
">
     <img height="30px" src="https://railway.app/button.svg">
  </a>
</p>

</a>
</p>

</details>

<details>
  <summary><b>Deploy in your VPS</b></summary>
<br/>

```sh
$ git clone https://github.com/shukurenaibotcreate/VCVideoPlayerBot.git
$ cd VCVideoPlayerBot
$ sudo apt-get install python3-pip ffmpeg
$ pip3 install -U pip
$ pip3 install -U -r requirements.txt
# <Create Variables appropriately (.env [optional])>
$ python3 main.py
```

</details>

---

## Requirements
- Python 3.6 or Higher.
- [Telegram API key](https://docs.pyrogram.org/intro/quickstart#enjoy-the-api).
- Latest [FFmpeg Python](https://www.ffmpeg.org/).
- Pyrogram [String Session](https://replit.com/@shukurenaibotcr/GenerateStringSession-1) of the account.
- The User Account Needs To Be An Admin In The Channel/Group.

---
