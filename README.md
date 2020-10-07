## Quick start

## What it is

RESTful-API for Dedicated Serverfiles, Mods and Addons generates your informationen on the fly.


## Features

- Simple and lightweight
- Support for Linux Dedicated
- Useful informationen
- Stay smart up-to-date
- Completely encrypted

## Requirements Web Server

- TekBASE 8.6.16
- PHP version 7.3 or higher
- PHP-Extension cURL 
- PHP-Extension Zip 
- PHP-Extension [ionCube Loader 10.4.4](https://ioncube.com/lw) stable
- HTTPS support (Free: [Let's Encrpyt free certificate](https://letsencrypt.org/de/))


## Requirements Service Server

- Recommended: Ubuntu 20.04 LTS or greater
- [Wine](https://www.winehq.org/)
- [Mono](https://www.mono-project.com/download/stable/#download-lin)
- [Shell Script Compiler](https://github.com/neurobin/shc)
- [jq](https://stedolan.github.io/jq/)
- [cURL](https://wiki.ubuntuusers.de/cURL/)
- Xvfb
- Java

```ssh
sudo dpkg --add-architecture i386
```

Wine:
```ssh
wget -nc https://dl.winehq.org/wine-builds/winehq.key | sudo apt-key add winehq.key
&& sudo apt-add-repository 'deb http://dl.winehq.org/wine-builds/ubuntu/ bionic main'
	
sudo apt install --install-recommends winehq-stable
```

Mono:
```ssh
sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
&& echo "deb https://download.mono-project.com/repo/ubuntu stable-bionic main" | sudo tee /etc/apt/sources.list.d/mono-official-stable.list 

sudo apt install --install-recommends mono-devel mono-complete
```

Needed Libs:
```ssh
sudo apt update && sudo apt install --install-recommends mailutils postfix wget file bzip2 gzip unzip bsdmainutils python util-linux \
ca-certificates binutils xvfb winbind tmux nano shc jq htop curl bc jq tmux default-jre \
lib32gcc1 libstdc++6 libstdc++6:i386 psmisc libfontconfig1 libpangocairo-1.0-0 libnss3 libgconf2-4 libxi6 \
libxcursor1 libxss1 libxcomposite1 libasound2 libxdamage1 libxtst6 libatk1.0-0 libxrandr2 -y
```

## Community

Users and the development team are usually in the [Discord chat room](https://celltek.de/discord).