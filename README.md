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

- TekBASE 8.6.16
- PHP version 7.3.X or higher (max 7.4.X)
- PHP-Extension cURL
- PHP-Extension Zip 
- PHP-Extension [ionCube Loader 11.0.0](https://ioncube.com/lw) stable
- HTTPS support (Free: [Let's Encrpyt free certificate](https://letsencrypt.org/de/) via [Certbot](https://certbot.eff.org/) or [Plesk Extension](https://www.plesk.com/extensions/letsencrypt/))


## Requirements Service Server

- Recommended: Ubuntu 20.04 LTS or greater
- [Wine](https://www.winehq.org/)
- [Mono](https://www.mono-project.com/download/stable/#download-lin)
- [Shell Script Compiler](https://github.com/neurobin/shc)
- [jq](https://stedolan.github.io/jq/)
- [cURL](https://wiki.ubuntuusers.de/cURL/)
- Xvfb
- Java 17

```ssh
sudo dpkg --add-architecture i386
```

Wine:
[Download](https://wiki.winehq.org/Download)

Mono:
[Download](https://www.mono-project.com/download/stable/#download-lin)

Needed Libs:
```ssh
sudo apt update && sudo apt install --install-recommend openjdk-17-jre-headless mailutils postfix wget file bzip2 gzip unzip bsdmainutils python util-linux \
ca-certificates binutils xvfb winbind tmux nano shc jq htop curl bc jq tmux \
lib32gcc1 libstdc++6 libstdc++6:i386 libsdl2-2.0-0:i386 psmisc libfontconfig1 libpangocairo-1.0-0 libnss3 libgconf-2-4 libxi6 \
libxcursor1 libxss1 libxcomposite1 libasound2 libxdamage1 libxtst6 libatk1.0-0 libxrandr2 -y
```

## Community

Users and the development team are usually in the [Discord chat room](https://celltek.de/discord).
