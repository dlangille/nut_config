Goal: allow host to shutdown when needed.

THIS is not a working configuration. I'm still testing.  This won't actually shutdown the host.

shutdown commands have not been added, this is initial testing.

Each host is monitored via the Nagios check_ups plugin.

Running on each host is:

```
[dan@slocum:~] $ ps auwwx | grep ups   
root      46270    0.0  0.0   11332    2868  -  Ss   19:49        0:00.00 /usr/local/sbin/upsmon localhost
uucp      46271    0.0  0.0   11596    2896  -  S    19:49        0:00.00 /usr/local/sbin/upsmon localhost
uucp      56305    0.0  0.0   11668    2952  -  Ss   20:07        1:05.11 /usr/local/libexec/nut/dummy-ups -a repeater
uucp      75564    0.0  0.0   11668    2952  -  Ss   20:14        1:02.33 /usr/local/libexec/nut/dummy-ups -a ups02
uucp      75566    0.0  0.0  110004    2936  -  Ss   20:14        0:02.01 /usr/local/sbin/upsd
dan       46603    0.0  0.0   11292    2760  3  S+   19:50        0:00.00 grep ups
[dan@slocum:~] $ 
```
