# time-track-simply
Simple CLI tool to track what you have done over day and have an overview.

It's written in pure bash together with standard UNIX utilities. Tested primarily on Cygwin environment.

# Usage
To create new record just call `timetrack` script and write what you just did until now. You will probably use this several times per day.

### timetrack
**It records time when you fill activity and hit [Enter]**. (The timestamp at beginning of line is just time when you invoke `timetrack` - probably not so useful.)
```console
$ ./timetrack
(13:24) Just finished activity: updated README of time-track-simply
```


### day-overview
```console
$ ./day-overview 2024-12-05
--:-- - 10:53    09:53: stanup, finishing documentation
10:53 - 11:59    01:06: helping Michal with configuration
11:59 - 12:20    00:21: reading news at root.cz
12:20 - 13:06    00:46: lunch
13:06 - 13:20    00:14: code review timetrack patch
13:20 - 14:23    01:03: refactoring day-overview script
```

### day-overview-yesterday
Same like `day-overview` with implicit previous day
