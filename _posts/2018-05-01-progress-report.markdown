---
layout: post
title:  "Progress report 18.04"
date:   2018-04-01 20:45:11 +0100
categories: news
---

March has been a busy month. We got the application back up on the Play Store, reicast.com & gamedb.reicast.com were migrated to new infrastructure, there was major progress in modernizing the Android tooling as well as Android UI bug fixing.

Over 1 million Android downloads
---
nullDC was released in April 1st 2007 as a reverse April fool's joke. That's 11 years ago, to the day. Reicast, which is derived from nullDC, has crossed the 1 milion downloads in the Android store this month. It's been a great ride, and we hope you've managed to relive childhood memories using these projects :)

Bye bye ant & eclipse
---
Thanks to @tolis764 who kept pushing for Android Studio support, we started working on it! Android Studio & Gradle are the modern tools that Google provides for building apps, and this migration was a prerequisite for further work.

Hello Jekyll and GitHub pages
---
Picking on the momentum, I decided to migrate the reicast.com to GitHub Pages + Jekyll. The old site was some ruby on rails code I had hacked together over a weekend and was an unmaintainable mess. The new design and tooling are very minimalistic, allowing us to focus on content.

Welcome back, Play Store listing
---
With the site updated we re-submitted to play store and got green-lighted within a few hours! Reicast was taken down because the old site did not have a privacy policy, which is now mandatory.

Nice to meet you, bug fixes
---
While I was working on the site, @tolis764 started migrating the Android codebase to use newer libraries and such. Shortly after @LoungeKatt joined in and continued from where @tolis764 left off, leading to many Android UI fixes, and even a branch with backported retroarch changes. Android 7.0 support is almost there now! These changes have not yet landed to master, but should do so before the end of the month.

So long, older Android versions
---
We decided to drop support for Android versions 2.x, 3.x and 4.0.x. While very few users use these OSes, we'll be nice and upload the last 2.2 compatible version as "Reicast Lite" to the store.

That's it for now,

~skmp
