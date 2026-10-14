---
title: "Dreamhost saved my bacon"
date: 2008-04-08
categories: 
  - "hosting"
  - "linux"
---

Kudos to Dreamhost for outsmarting my attempt to delete critical data.

<!--more-->

I was cleaning up some sites over the weekend and in the process I was deleting MySQL databases that were no longer needed. I noticed last night that one of my Joomla based sites wasn't working. I was getting a message saying that the site was offline and that I should contact my administrator, which would be me. I had a moment of panic, when I also noticed in the fine print at the bottom of that message, that the site could not connect to the database.

Yikes! I must have deleted it when I was cleaning up! Oh noes!

OK. After the initial panic passed, I decided to go and see if there was any kind of recycle bin that I could get my poor discarded database back from. I'm sure you can imagine my excitement when I found that their MySQL management site includes just that functionality.

I dug into the recycle bin and, sure enough, there was my missing database. I selected it from the list and told the system to please put it back. Almost immediately, the database was back. I then noticed that the site still didn't work. Same error.

Guh...

OK, so maybe the recycle bin only restored the database structure and not the data. Let's go looking for a backup/restore utility. (Not that I had ever actually backed it up, mind you.) Sure enough, I clicked on the option to restore a backup and found that Dream host had a complete history of about five versions that I could choose from. I restored the most recent one and... viola! The site was back online.

Thanks, DreamHost, for watching my back.
