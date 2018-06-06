---
title: "Wipe a File Without Deleting It"
date: 2018-04-12T06:55:36-06:00
draft: true
tags: ['linux', 'cli', 'foundation', 'file-management']
---

> On occasion there are files that get really big (often logs) and due to their size it's too difficult to edit the file down or use logrotate. If the data isn't needed a quick way to clear the contents of the file without removing the file and creating a new one (great for apps that have a file lock on the file) is by using /dev/null.

## Useful Commands
* `/dev/null > /path/to/big/file.log`
* `> /path/to/big/file.log` // Short cut for the above file

### Resources
* [5 Ways to Empty or Delete a Large File Content in Linux](https://www.tecmint.com/empty-delete-file-content-linux/)
