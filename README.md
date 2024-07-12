# weewx5
weewx auf Raspi5

Import WsWin
https://www.pc-wetterstation.de/forum/viewtopic.php?f=26&t=10329
bitte csv-wswin5.conf beachten
Ordner etc/weewx/import für conf-Datei und Datendatei wswin.csv

sudo wget https://wischewetter.info/wswin.csv

sudo weectl import --config=/etc/weewx/weewx.conf --import-config=/etc/weewx/import/csv-wswin5.conf

Using configuration file /etc/weewx/weewx.conf
Starting weectl import...
**** Unable to parse source-to-WeeWX field map.
**** No units specified for source field 'Date' in /etc/weewx/import/csv-wswin5.conf.
**** Nothing done, exiting.

