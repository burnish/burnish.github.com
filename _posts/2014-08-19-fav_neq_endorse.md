---
title: Star &#x2260; Endorsement
layout: post
category: twitter casterly
tags: []
description: Why it might not be so bad that Twitter sometimes surfaces tweets based on who stars them.
---

Twitter has made some changes recently where tweets are occasionally promoted just because they have been starred by people in your network. Understandably, people have been [airing][codinghorror] [their][cabel] [dissatisfaction][monkbent] with this change. I tried to [point out][blackp] how maybe it's not so bad, but 140 characters didn't seem quite enough. 

This topic is of interest to me because it plays a part in how [Casterly][casterly] works: a podcast might turn up in your episode stream, annotated with "starred by @user_you_follow". I've felt slightly uneasy about this ever since implementing it late last year. Activity on twitter is and always has been public[^1], but sometimes bringing public activity to attention can be uncomfortable.

Any recommendation algorithm comes with false positives, which might range from the odd to the awkward. The question is whether the useful recommendations are good enough to overlook those that miss. In my experience with Casterly so far, it's a worthwhile trade off[^2].

Everyone is entitled to a different interpretation of how Twitter should work. As a regular user with friend, follower, tweet, and favourite counts in the low hundreds; my perspective is quite different to most of those complaining (who tend to have numbers in the tens of thousands). My gut feeling is that the net effect of this change will be for the positive.

There are all sorts of ways I would like to improve the algorithms that drive Casterly's episode recommendations. I look forward to a day when those slightly awkward false positives are better culled. I bet Twitter is a long way ahead of me in getting there too. It's still likely that occasional tweets will surface where the star was not intended as endorsement. But really, what's the harm? Give a bit of credit to the follower to work that out in context.

[^1]: With the exception of protected accounts.
[^2]: There have been other strategies where the trade off has not been worthwhile. Given the sparsity of podcast episode links in some user's timelines there are various other ways I've tried to reach further into a user's Twitter network of activity. The "starred by" is the only one so far that I'm mostly comfortable with.

[codinghorror]: https://twitter.com/codinghorror/status/501507338394554368
[monkbent]: https://twitter.com/monkbent/status/501524491625705472
[cabel]: https://twitter.com/cabel/status/501284443399536640
[blackp]: https://twitter.com/blackp/status/501288943686410240
[nudge]: https://twitter.com/michaelhoney/status/475848843246829569

[casterly]: http://www.casterly.net
[app-store]: https://itunes.apple.com/us/app/casterly/id705700170?ls=1&mt=8
