## Quick start

## What it is

RESTful-API for Dedicated Serverfiles, Mods and Addons generates your informationen on the fly.

## Features

- Simple and lightweight
- Support for Linux Dedicated Gameserver
- Useful informationen
- Stay smart up-to-date
- Completely encrypted

## Requirements Web Server
 
- TekBASE 8.6.16 (no support for PHP 8)
- PHP version 7.4
- PHP-Extension cURL
- PHP-Extension Zip 
- PHP-Extension [ionCube Loader 14.4.0](https://ioncube.com/lw) stable
- HTTPS support (Free: [Let's Encrpyt free certificate](https://letsencrypt.org/de/) via [Certbot](https://certbot.eff.org/) or [Plesk Extension](https://www.plesk.com/extensions/letsencrypt/))

## Recommendation TekBASE

- GameQv3 - Fix Online Status [download](https://github.com/celltek/game.protocol/archive/refs/heads/main.zip)

## Requirements Service Server

**!! NO SUPPORT FOR DEBIAN OR OTHER LINUX DISTRIBUTIONEN !!**

**Dependencies**
- OS: Ubuntu 24.04.1 LTS (Noble Numbat)
- [Shell Script Compiler](https://github.com/neurobin/shc)
- [jq](https://stedolan.github.io/jq/)
- [cURL](https://wiki.ubuntuusers.de/cURL/)
- [xmlstarlet](https://xmlstar.sourceforge.net/)
- Java 8, Java 11,Java 17, Java 21

**If you are using a 64-bit machine, you will need to add multiverse**
```ssh
sudo add-apt-repository multiverse
sudo apt install software-properties-common
sudo dpkg --add-architecture i386
```

**Dont forget to update, if you add multiverse before installing**
```ssh
sudo apt update
```

**SteamCMD**
```ssh
sudo apt install lib32gcc-s1 steamcmd
**agree steam license**
```

**Dependencies install**
```ssh
sudo apt update && sudo apt install openjdk-8-jdk-headless openjdk-11-jdk-headless openjdk-17-jdk-headless \
openjdk-21-jdk-headless mailutils postfix wget file bzip2 gzip unzip bsdmainutils python3 util-linux \
ca-certificates binutils xmlstarlet tmux nano shc jq curl bc libxml2-utils \
lib32gcc-s1 libstdc++6 libstdc++6:i386 libcurl3-gnutls:i386 \
libsdl2-2.0-0:i386 psmisc libfontconfig1 libpangocairo-1.0-0 libnss3 libxi6 \
libxcursor1 libxss1 libxcomposite1 libxdamage1 libxtst6 libatk1.0-0 libxrandr2 -y
```

**Change Java default version with**
```ssh
sudo update-alternatives --config java
```

## Community

Users and the development team are usually in the [Discord chat room](https://celltek.de/discord).