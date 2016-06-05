# NoroBot

**An advanced and powerful administration bot based on [yagop/telegram-bot](https://github.com/yagop/telegram-bot) licensed under the [GNU General Public License](https://github.com/NoroTeam/NoroBot/blob/master/LICENSE)**.

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

