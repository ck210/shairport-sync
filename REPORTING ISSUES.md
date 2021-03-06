
Reporting Issues and Making Pull Requests
====

Pull Requests
----
If you would like to contribute to the development of Shairport Sync, please make you changes to the `development` branch and make a pull request.

Changes and additions in the development branch make their way eventually to the `master` branch.

Issue Reports
----
Issue reports are welcome, but before you report an issue, please have a look though the existing [issues](https://github.com/mikebrady/shairport-sync/issues), both open and closed, and check for hints in the [TROUBLESHOOTING](TROUBLESHOOTING.md) page. It would be great to give some details of the device and version of Linux or FreeBSD in use along with the version of Shairport Sync you are using (use `$ shairport-sync -V` to get this). Then, if possible, some diagnostic information from the log or logfile would be useful.

If your system uses `systemd`, as most recent Linuxes do, try using:
```
$ sudo systemctl status shairport-sync
```
You might get something lke this:
```
● shairport-sync.service - Shairport Sync - AirPlay Audio Receiver
   Loaded: loaded (/lib/systemd/system/shairport-sync.service; disabled; vendor preset: enabled)
   Active: active (running) since Fri 2019-11-29 08:52:47 GMT; 3s ago
 Main PID: 19812 (shairport-sync)
    Tasks: 10 (limit: 4915)
   Memory: 2.0M
   CGroup: /system.slice/shairport-sync.service
           └─19812 /usr/local/bin/shairport-sync

```

If so, please paste it in as code (see below) the output into your message.

In general, a log verbosity of 2 is adequate (`-vv`, or the relevant entry in the configuration file), and it's usually helpful if statistics have been enabled (`--statistics` on the command line, or the relevant entry in the configuration file).

If you are pasting in code or a log file, format it as code by preceding it and following it with a line containing exactly three backquotes and nothing else ([see here](https://guides.github.com/features/mastering-markdown/) for more on formatting): 

\`\`\`
```
code or log file entries
```
\`\`\`

