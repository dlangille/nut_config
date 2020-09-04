Goal: allow host to shutdown when needed.

THIS is not a working configuration. I'm still testing.  This won't actually shutdown the host.

shutdown commands have not been added, this is initial testing.

Each host is monitored via the Nagios check_ups plugin.

Running on each host is:

$ ps auwwx | grep ups
uucp    71970    0.0  0.0     11668   2944  -  Ss   00:39        0:30.57 /usr/local/libexec/nut/dummy-ups -a ups02
uucp    71972    0.0  0.0    257460   2936  -  Ss   00:39        0:01.16 /usr/local/sbin/upsd

