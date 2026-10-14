---
title: "I just love Micro$oft..."
date: 2008-10-27
categories: 
  - "linkedin"
  - "microsoft"
---

Hmmm... well maybe not so much. I've been caught up in the latest "emergency" patch deployment.

I'm thankful that we have made so much progress in our patch deployment processes. I believe we have over 800 workstations in our patch management system. Many of our servers are also in that system, but we still have to connect to each one and allow the patches to be installed.

<!--more-->

We have noticed a gotcha. One of the utilities that our PC Support group uses is GenControl. It is a VNC based remote control program that pushes out the server portion on demand. When you are done with that connection, it removes the server component so that there are no additional, unnecessary services running. This patch appears to break GenControl. I haven't tested a basic VNC connection yet, but Iâ€™d bet that it is broken as well. I'll try to remember to post my findings on that later.

I also heard of some possible reboot problems, but I don't have any detail on that yet.

At any rate, we are chugging along with this deployment. I would have gotten more done this weekend, but my internet connection has not been performing well. I guess I'll hit it early in the morning and see how many systems I can get done before people start the work week.
