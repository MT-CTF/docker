FROM webd97/minetestserver:0.4.17.1

RUN apk update
RUN apk add git
RUN cd /minetest/games && git clone https://github.com/MT-CTF/capturetheflag --recursive
RUN cd /minetest/mods && git clone https://github.com/MT-CTF/servermods
RUN cd /minetest/mods && git clone https://github.com/MT-CTF/rules
RUN cd /minetest/mods && git clone https://github.com/shivajiva101/sauth
RUN cd /minetest/mods && git clone https://github.com/shivajiva101/sban
RUN cd /minetest/mods && git clone https://github.com/minetest-mods/irc
RUN cd /minetest/mods && git clone https://github.com/rubenwardy/prometheus
RUN cd /minetest/mods && git clone https://github.com/minetest-mods/filter
RUN cd /minetest/mods && git clone https://github.com/ClobberXD/hud_notify
RUN cd /minetest/mods && git clone https://github.com/MT-CTF/minetest-irc_commands -b host_logins
RUN cd /minetest/mods && wget https://forum.minetest.net/download/file.php?id=177 -O no_guests.zip && unzip no_guests.zip
