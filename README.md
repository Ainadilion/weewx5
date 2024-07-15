# weewx5
weewx auf Raspi5

Import WsWin
https://www.pc-wetterstation.de/forum/viewtopic.php?f=26&t=10329
bitte csv-wswin5.conf beachten
Ordner etc/weewx/import für conf-Datei und Datendatei wswin.csv

sudo wget https://wischewetter.info/wswin.csv

sudo weectl import --config=/etc/weewx/weewx.conf --import-config=/etc/weewx/import/csv-wswin5.conf

sudo weectl database calc-missing --config=/etc/weewx/weewx.conf

dwd-wget in usr/bin/local
DWPG Land Brandenburg für Vorhersage VHDL50 bis 54

sudo systemctl start weewx
sudo systemctl stop weewx

sudo journalctl -u weewx --lines 500

Treiber
sudo weectl station reconfigure --driver=weewx.drivers.simulator
sudo weectl station reconfigure --driver=user.interceptor
