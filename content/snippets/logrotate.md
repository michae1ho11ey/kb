---
title: "Logrotate Basics"
date: 2018-04-12T06:55:36-06:00
draft: true
tags: ['linux', 'cli', 'foundation', 'logrotate']
---

# Logrotate
> <Intro to logrotate>

## Important Locations
* `/etc/logrotate.conf` // Basic logrotate config
* `/etc/logrotate.d/` // Where app specific logrotate files are stored
* `/etc/cron.daily/logrotate` // Cron job to control when logrotate runs

## Useful Commands
* `logrotate -vf /etc/logrotate.d/service` // Manually force logrotate to run and be verbose

## Examples
**MongoDB:**
```
/var/log/mongodb/mongod.log {
    weekly
    rotate 5
    missingok
    notifempty
    copytruncate
}
```

### Resources
* [Manage Linux log files with Logrotate](http://www.techrepublic.com/article/manage-linux-log-files-with-logrotate/) // List all options
* [Understanding logrotate utility](https://support.rackspace.com/how-to/understanding-logrotate-utility/) //Explanation and examples

+linux+ +cli+ +foundation+ +logrotate+
