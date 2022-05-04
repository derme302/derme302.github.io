---
title: "Cookie - Homepod Mini of Terror"
date: 2022-05-04T18:30:00+10:00
categories:
  - Smart Home
tags:
  - guide
---
I recently picked up a Homepod Mini so that I could compare it against Alexa and Google Home speakers. I had thought that this would be a pretty straight forward endeavour, but I was wrong.

The Homepod decided to utilize 100% of my bandwidth for the first two days and use over 200GB+ of data, which is an impressive effort as it only has 64GB of memory. I was very confused by the whole thing and even after solving it I am not sure I fully understand how this issue occurs.

Luckily, I stumbled on [this Reddit post](https://www.reddit.com/r/HomePod/comments/piloe8/homepods_utilize_100_of_my_internet_bandwidth/) with someone having the same problem. The advice I got there was that if the Homepod has issues with it's software update it'll just infinitely retry the update (which does seems dumb).

So if you've hit the same issue, my steps for resolution:

1. Setup a Content Sharing Service (in System Preferences: Sharing) on a Mac in your local LAN
2. Set the Mac power settings so that it doesn't hibernate or go to sleep while plugged in
3. Reset the Homepod (Can be done by removing it from the Home app)
4. They should start downloading the software update from your Mac (You may need to force this in the Home app)
5. Then you may still need to leave it for ~24 hours as it syncs your iCloud music library

After that it should be sorted, my Homepod is currently using 1.6kbps of download, which is a much more sustainable amount of usage.
