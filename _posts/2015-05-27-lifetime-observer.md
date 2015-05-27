---
layout: post
title: "Lifetime Observer"
tags: code
---

I've been enjoying the recent run of [Inessential][inessential] posts on How Not to Crash. Brent Simmons has been at this a long time, and these sound like hard learned lessons. In particular the [one on NSNotification][inessential-notification] piqued my interest. The two simplifying rules he suggests are that you should send notifications from the main thread, and your observers should observe for their entire lifetime. Both sound good to me.

The bit that I don't like is having to remember to remove the observer. If you're always going to be removing the observer in `dealloc`, why not automate it? Brent urges against using `-[NSNotificationCenter addObserverForName:​object:​queue:​usingBlock:]` because it makes for more housekeeping. But the housekeeping it requires is quite straightforward. I've added a category on `NSNotificationCenter` that wraps it and calls `-[NSNotificationCenter removeObserver:]` appropriately on deallocation (of an object you can specify as a parameter).

I'm not totally happy with the name, but I'm happy with the result, one call and you're done. The block is nicely tied to the registration, and clean up happens automatically.

I should knock my ‘Standard Kit’ in to a good enough shape that I feel okay having it public on github, but in the absence of that, I've added this [category as a gist][gist]. Curious to hear if I'm missing something, because it sort of seems too easy.

[inessential]:http://inessential.com
[inessential-notification]:http://inessential.com/2015/05/21/how_not_to_crash_3_nsnotification
[gist]:https://gist.github.com/blackp/d60c2f85392d139a95ee
