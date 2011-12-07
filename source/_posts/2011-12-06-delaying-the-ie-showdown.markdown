---
layout: post
title: "Delaying the IE Showdown"
date: 2011-12-06 20:27
comments: true
categories: development
---

<script src="http://storify.com/olivierlacan/how-do-you-deal-with-internet-explorer.js"></script><noscript><a href="http://storify.com/olivierlacan/how-do-you-deal-with-internet-explorer" target="_blank">View the story "How do you deal with Internet Explorer?" on Storify</a>]</noscript>

To conclude almost every single response presented an approach where styles are written in a standards-compliant environment (today that would be Chrome or Safari, more so than Firefox) then adjusted for IE's obsolete ways.

Keep this in mind, because a production process tied by IE-compatibility from the get-go is likely to create frustrations and creative limitations very early on. It doesn't mean one shouldn't consider IE before the end-stages of a project (as Nick pointed out, the demographic matters a lot) but be weary of efforts towards graceful degradation that may be rendered unnecessary by late design decisions.

Project managers are rarely as cautious with CSS since it doesn't directly impact business logic (back-end), which means they are more likely to propose modifications to styles later on in a project than they would with controller-logic that could cause functionality breakage.

Managers also often expect websites to [look the same in every browser](http://dowebsitesneedtolookexactlythesameineverybrowser.com/). If you catch any flak when adopting such a process, don't hesitate to point out that many web professionals adopt a similar technique because it is the most efficient use of their time. Going and back and forth between standard CSS and IE fallbacks after each design iteration is a waste of your time and their money.

If managers or clients somehow insist of having fully IE compatible sites after each iteration, several people have suggested introducing an IE tax to give everyone a clear picture of the [true cost of obsolete browsers](http://www.informationweek.com/news/windows/microsoft_news/229401795) on development schedules.

I highly recommend Andy Clarke's thorough [breakdown of his Canny Bill redesign](http://stuffandnonsense.co.uk/blog/about/what_does_browser_testing_mean_today/) across progressively less advanced browsers and his benchmark browser approach.

Finally, one of the best tools to further the cause of graceful degradation (a much more logical moniker than "progressive enhancement") is [Modernizr](http://www.modernizr.com/), spearheaded by [Faruk Ateş](http://farukat.es/), [Paul Irish](http://paulirish.com) and [Alex Sexton](http://alexsexton.com/).