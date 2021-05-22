---
title: Linux Problems
date: 2021-05-22
categories:
- Linux
---
### Gnome have to switch tty twice to start gdm
```bash
sudo systemctl edit gdm
```
And append
```bash
[Service]
Type=idle
ExecStartPre=/bin/sleep 1
```
