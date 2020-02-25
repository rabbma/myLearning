# Linux Tips

Mount nsf
mkdir /data2
mount -t nfs 192.168.100.54:/data2 /data2

rsync
nohup rsync -a mydir /data2 &

crontab
2 0 * * * /usr/local/work/vmstat.sh > /dev/null 2>&1

MIN HOUR DOM MON DOW CMD

Field    Description    Allowed Value
MIN      Minute field    0 to 59
HOUR     Hour field      0 to 23
DOM      Day of Month    1-31
MON      Month field     1-12
DOW      Day Of Week     0-6
CMD      Command         Any command to be executed.


