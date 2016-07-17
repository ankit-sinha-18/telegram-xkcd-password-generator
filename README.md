# <p align="center">  Readable Passwords Generator for Telegram #

This bot allows you to generate readable passwords directly from Telegram without necessity to open external utilities such as KeePass. An inspiration for this bot came from famous [XKCD 936](http://xkcd.com/936/) strip.  
Try it now: https://telegram.me/passgenbot

### Features 
* Presets of different complexity
* Ability to generate customized password  
* Inline mode with colored complexity
* No personal data is collected!  

### Used modules
* [pyTelegramBotAPI](https://github.com/eternnoir/pyTelegramBotAPI) – Awesome Telegram API wrapper
* [TinyDB](https://github.com/msiemens/tinydb) – Simple and pretty fast document-oriented DB
* [XKCD-password-generator](https://github.com/redacted/XKCD-password-generator) – It goes without saying :)
* [Botan](https://github.com/botanio/sdk) – Yandex.Appmetrica bot analytics
* [CherryPy](https://github.com/cherrypy/cherrypy) – Web-Server for using with Webhooks  

### Presets
 ![Presets](https://pp.vk.me/c636824/v636824512/19583/hJgaGSvCn8c.jpg)

`/generate_weak` – 2 words, no separators between words  
`/generate_normal` – 3 words, no separators between words, second word is CAPITALIZED  
`/generate_strong` – 3 words, random CAPITALIZATION, random number as separator between words   
`/generate_stronger` – Same as "strong", but using 4 words    
`/generate_insane` – 4 words, second one CAPITALIZED, separators, prefixes and suffixes  

### Customized Passwords

![Customized Passwords](https://pp.vk.me/c636824/v636824512/1958b/6X8h64GqpaA.jpg)  

With `/settings` command you can customize generated passwords. Currently supported settings are number of words (2 to 8), prefixes and suffices in the beginning and in the end of password and separators between words in password. Then just use `/generate` command to create password based on your settings.

### Inline mode

![Inline mode](https://pp.vk.me/c636824/v636824512/1959c/Y3f8VXAWOdw.jpg)

You can also use this bot in inline mode. An indicator on the left shows rough password complexity (green is good, red is not).


### Botan analytics

I'm using [Botan](http://botan.io/) in my bot to collect anonymous stats for most used commands. Here you can see screenshot of Botan's web interface. Notice I'm using stubs to get rid of user ID's or other user-specific data.  

![Botan web interface](https://pp.vk.me/c636824/v636824512/195a5/QwSq4wC3KiU.jpg)



### My other projects
* [Telegram-RSS-Generation](https://github.com/Kondra007/telegram-rss-generation) – A concept for creating an RSS feed for your own channel
* [Telegram Proxy Bot](https://bitbucket.org/master_groosha/telegram-proxy-bot) – A "virtual" bot account for chatting with other people without telling your real username (one bot for one person)   