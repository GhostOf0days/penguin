A cli tool to browse and watch TV shows and movies, Korean Dramas (and, in the future, Chinese Dramas), and anime. You can also browse and read manga. Uses versions of ani-cli and dra-cli containing modifications, bug fixes, and improvements. Uses base version of [lobster](https://github.com/justchokingaround/lobster) for TV show and movie support. Uses base version of [mangal](https://github.com/metafates/mangal) for manga support.

## Table of Contents
- [Terminal Command](#Terminal-Command)
- [Install](#Install)
  - [Linux &amp; macOS Installation](#Linux--macOS-Installation)
- [Uninstall](#Uninstall)
  - [Uninstall on Linux &amp; macOS](#Uninstall-on-Linux--macOS)
- [Dependencies](#Dependencies)
- [A Note on ani-skip for Anime](#A-Note-on-ani-skip-for-Anime)
- [Disclaimer](#Disclaimer)
  - [DMCA &amp; Copyright Infrigements](#DMCA--Copyright-Infrigements)

## Terminal Command
```penguin```

## Install

### Linux &amp; macOS Installation

Install [dependencies](#Dependencies) before installing penguin.

```sh
cd ~
sudo curl -sL https://raw.githubusercontent.com/GhostOf0days/penguin/main/lobster-cli.sh > lobster-cli
sudo curl -sL https://raw.githubusercontent.com/GhostOf0days/penguin/main/drama-cli.sh > drama-cli
sudo curl -sL https://raw.githubusercontent.com/GhostOf0days/penguin/main/anime-cli.sh > anime-cli
sudo curl -sL https://raw.githubusercontent.com/GhostOf0days/penguin/main/penguin.sh > penguin
chmod +x lobster-cli
chmod +x drama-cli
chmod +x anime-cli
chmod +x penguin
sudo mv lobster-cli /usr/local/bin/lobster-cli
sudo mv drama-cli /usr/local/bin/drama-cli
sudo mv anime-cli /usr/local/bin/anime-cli
sudo mv penguin /usr/local/bin/penguin
PATH=/usr/local/bin:$PATH
```

## Uninstall

### Uninstall on Linux &amp; macOS

 ```sh
sudo rm /usr/local/bin/lobster-cli /usr/local/bin/drama-cli /usr/local/bin/anime-cli /usr/local/bin/penguin
```

## Dependencies

- grep
- sed
- curl
- openssl
- mpv - Video Player
- vlc - Video Player
- iina - mpv replacement for MacOS
- aria2 - Download manager
- yt-dlp - m3u8 Downloader
- ffmpeg - m3u8 Downloader
- fzf - User interface
- ani-skip (optional, but recommended)

## A Note on ani-skip for Anime
ani-skip is a script to automatically skip anime opening sequences, making it easier to watch your favorite anime without having to manually skip the intros each time (from the original [README](https://github.com/synacktraa/ani-skip/tree/master#a-script-to-automatically-skip-anime-opening-sequences-making-it-easier-to-watch-your-favorite-shows-without-having-to-manually-skip-the-intros-each-time)).

For install instructions visit [ani-skip](https://github.com/synacktraa/ani-skip).

ani-skip uses the external lua script function of mpv. Therefore, it only works with mpv for now.

Warning: For now, ani-skip does not seem to work under Windows.

Note: ani-skip may not know the anime you're trying to watch. Try using the --skip-title <title> command line argument. (It uses the [ani-skip API](https://github.com/lexesjan/typescript-aniskip-extension/tree/main/src/api/aniskip-http-client) and you can contribute missing anime or ask for including it in the database on their [Discord server](https://discord.com/invite/UqT55CbrbE).

## Disclaimer
The core aim of this project is to co-relate automation and efficiency to extract what is provided to an user on the internet. Every content available in the project is hosted by external non-affiliated sources.

Any content served through this project is publicly accessible. If your site is listed in this project, the code is pretty much public. Take necessary measures to counter the exploits used to extract content in your site.

Think of this project as your normal browser, but a bit more straight-forward and specific. While an average browser makes hundreds of requests to get everything from a site, this project goes on to make requests associated with only getting the content served by the sites.

This project is to be used at the user's own risk, based on their government and laws.

This project has no control on the content it is serving, using copyrighted content from the providers is not going to be accounted for by the developer. It is the user's own risk.

## DMCA &amp; Copyright Infrigements
A browser is a tool, and the maliciousness of the tool is directly based on the user.

This project uses client-side content access mechanisms. Hence, the copyright infrigements or DMCA in this project's regards are to be forwarded to the associated site by the associated notifier of any such claims.