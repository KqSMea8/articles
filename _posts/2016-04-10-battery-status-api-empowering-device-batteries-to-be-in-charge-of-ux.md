---

title: 'Battery Status API: Empowering device batteries to be in charge of UX'
layout: post

---
Let me set the scene: you’re in an unfamiliar city and you’re on the move. Through a series of travel delays and general unpreparedness, you are about to be late to interview for your dream job. Frantically, you try to continue to make progress on foot while not knowing the actual address of the place. Your phone’s map app doesn’t recognize the business’s name, so you need to search for their address in your smartphone’s browser.

Sadly, a day of travel and data roaming has also sapped your phone’s battery, leaving you with just 5% left. Google results show the place’s homepage in the results, but not their physical address, so you have to click into their site—a modern site with huge graphics, a testimonials carousel, and even background video showing the hustle and bustle of their office on an average day, much like today.

You frantically try to thumb-scroll to the footer, where every sensible business has their physical address (or at least a “Contact Us” link to that info) but as the browser tries loading all the snazzier assets further up the DOM, your battery tanks further and further until it blinks out of existence and you’re left like an unfrozen caveman, unsure of where to go or how to navigate the concrete jungle.

Even those of us that are battery charging obsessive could find ourselves in a similar situation. I’ve <a href="https://twitter.com/_ragozzine/status/702203645069283333">previously scoffed</a> at the “mobile users are constantly sprinting around the world with no time for ANYTHING” zip-zip mantra of web development. Often, this manner of thinking results in engineers choosing absolutes, cut along the Mobile-Desktop / Mason-Dixon Line (M-D for both? Coincidence?!). The resulting “<a href="https://twitter.com/_ragozzine/status/675319601757036544">hide on mobile</a>” atrocity is not the answer; the decision can be far more nuanced than that.

<img src="/images/battery-life.png" />

You can push your mobile strategy further by leveraging the <a href="https://w3c.github.io/battery/">Battery Status API</a>. While <a href="http://caniuse.com/#feat=battery-status">not 100% supported</a> yet, I feel this type of useful tool will soon be universally available. With it, you can detect whether a device’s battery is high or low, charging or de-charging, and use that information to determine how much data downloading the device can handle.

In the case above, the device’s extremely low battery could be detected and used to inform the site presentation. With only 5% battery left, the basic content of the site could be loaded first, with the splashy design elements being delayed or, more likely, jettisoned completely. Yes, this could result in “hide on mobile,” but at least it would be a conscious, informed decision based on real-time data, not engineer assumptions.

The opposite can be true as well. If the battery is charging, you know that the user is likely stationary (near a wall outlet) and casually browsing your site. That said, you don’t need to hold back on the eye-catching features of the “full” site; you can have at it with all the power-zapping fluff you want!

<a href="http://blog.teamtreehouse.com/exploring-battery-status-api">Treehouse has a nice Battery Status API demo</a> you can play around with, to expand your user friendly web dev arsenal a bit more. From mobile sites to native apps, sniffing out as much about your users’ states as you can will help you take your code to the next UX level.
