---
title: "MS08-067 and VNC"
date: 2008-10-28
categories: 
  - "linkedin"
  - "microsoft"
---

Well, I've finally done some testing and it appears that the MS08-067 patch doesn't break VNC. I have been testing with an XP SP3 system and the latest version of Tight VNC.

I started with the XP system and no patch. I installed and configured VNC as a service and tested it. I was able to take remote control with no problems, which I would expect.

After installing MS08-067 on the XP system, I rebooted as required. Everything seemed to come up fine and I noticed that the VNC icon was in the system tray. Again, this is as would be expected. I fired up my VNC client and took remote control of the XP system without hesitation. All works well.

Keep in mind, this is one system. There may be other problems with other scenarios. Next, I need to do some more definitive testing with GenControl.
