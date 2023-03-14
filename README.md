⚠️ UNMAINTAINED / DEPRECATED ⚠️
============
### NoroBot

**An advanced and powerful administration bot based on [yagop/telegram-bot](https://github.com/yagop/telegram-bot) licensed under the [GNU General Public License](https://github.com/NoroTeam/NoroBot/blob/master/LICENSE)**.

### Features

* **A powerful antispam system with custom sensitivity for each group**
* **Multiple realms (admin groups)**
* **Recalcitrant to any kind of spamming (X/Y bots, name/photo changers, etc.)**
* **Global banning**
* **Broadcast to all groups**
* **Group and  links**
* **Kick, ban and unban by reply**
* **Groups, ban and global ban list**
* **Logging anything that happens in a group**
* **Invitation by username**
* **Group administration via private messages**
* **Only mods, owner and admin can add bots in groups**
* **Arabic lock**
* **Lock TgService**
* **Chat list**
* **And more!**

### Ranks 

| Rank | Description |
|:------|:------------|
| Banned | Cannot enter the group(s). |
| User | Default rank. |
| Moderator | Can set settings and kick/ban/unban users from a group. Can unmute users. |
| Owner | Can mute users. Can promote/demote moderators. Can set SuperGroup admins. |
| Support | Can globally unban users. Acts as owner of all groups. |
| Administrator | Can globally ban/unban users. Can promote/demote owners. |
| Sudo | Can add[#!/]remove groups. Can broadcast. Can promote/demote administrators. |

Each higher status inherits the privileges of the lower status.

**You can use "#", "!", or "/" to begin all commands

# Installation

```sh
# Install dependencies.
# Tested on Ubuntu 14.04. For other OSs, check out https://github.com/yagop/telegram-bot/wiki/Installation
sudo apt-get install libreadline-dev libconfig-dev libssl-dev lua5.2 liblua5.2-dev lua-socket lua-sec lua-expat libevent-dev make unzip git redis-server autoconf g++ libjansson-dev libpython-dev expat libexpat1-dev

# Let's install the bot.
open new Teminal

git clone https://github.com/NoroTeam/NoroBot.git
cd NoroBot
chmod +x Noro.sh
./Noro.sh install
./Noro.sh # Enter a phone number & confirmation code.
```
### One command
To install everything in one command (useful for VPS deployment) on Debian-based distros, use:
```sh
sudo apt-get update; sudo apt-get upgrade -y --force-yes; sudo apt-get dist-upgrade -y --force-yes; sudo apt-get install libreadline-dev libconfig-dev libssl-dev lua5.2 liblua5.2-dev lua-socket lua-sec lua-expat libevent-dev libjansson* libpython-dev make unzip git redis-server g++ autoconf -y --force-yes && git clone https://github.com/NoroTeam/NoroBot.git && cd NoroBot && chmod +x Noro.sh && ./Noro.sh install && ./Noro.sh
```

* * *

### Realm configuration

After you run the bot for first time, send it `!id`. Get your ID and stop the bot.

Open ./data/NoroBot.lua and add your ID to the "sudo_users" section in the following format:
```
  sudo_users = {Yourid}
```
If you are some guys following this format:
```
  sudo_users = {id1,id2,id3,....,idx}
```

