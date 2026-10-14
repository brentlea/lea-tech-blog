---
title: "ProFTP on Ubuntu Server"
date: 2009-02-10
categories: 
  - "linux"
---

Installing the ProFTP 1.3.1 server on Ubuntu Server 8.10 is a pretty straight forward process. I won't go into the whole thing here, but a standard apt-get works just fine.

I started running into problems when a user noticed that after uploading a file to the server, the time stamp on the file was six hours ahead. That corresponds with the six hour offset from GMT for Central Standard Time. The confusing thing was that the problem was only visible through an FTP login. If I connected to the server through an SSH session, all of the date information on the files was correctly showing CST time.

<!--more-->

When troubleshooting started, the first thing I found was an option in the proftpd.conf file that lets you turn on and off reporting of date information using GMT. I turned the option off and restarted the daemon. No joy.

Finally, after much name calling and gnashing of teeth, I found an article that talked about the way linux handles the various time zones. It seems that the ProFTPd server looks for CST when trying to use Central Standard Time. The Ubuntu server I was working on did not have an entry for CST in /usr/share/zoneinfo. I ended up creating a symlink for CST that points to CST6CDT, which is how this linux system looks for Central Standard Time. After a quick restart of the proftpd daemon, time information was displaying correctly through an FTP login.

I have confirmed that the /usr/share/zoneinfo folder structure looks the same on both SuSE and Ubuntu. I can't vouch for other distributions, so your mileage may vary.
