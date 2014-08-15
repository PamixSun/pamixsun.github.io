---
layout: post
title:  "Gigabit Broadband"
date:   2014-07-02 23:15:11
categories: tech
---

I'm lucky enough to live in an apartment complex in London's Docklands that's recently had [Hyperoptic][ho] installed. As I run the Residents' Association for my complex, and got into a bit of a Twitter conversation with their head of marketing (following them picking up on the fact that I was slagging off Sky Broadband!), I managed to set myself up to be their "Hyperoptic Champion" for my development. This essentially means that I help them to market their services to the residents, and in return I get their services for free. It got activated in the middle of May.

After having issues with my previous broadband provider I'd forked out a fair amount of cash for a [Billion 7800DXL][billion], a router that allows you to modify pretty much any setting you could ever think of in order to get the maximum possible performance from your ADSL connection. One of the things that attracted me to this router was that it supported ADSL and a WAN connection (which is what Hyperoptic provide), so knowing that I'd be getting Hyperoptic at some point in the future I'd be reasonably 'futureproofed'. Wrong!

After Hyperoptic was switched on, I did what every tech geek would do and ran a speed test:

~~~
Testing from Hyperoptic Ltd (154.xxx.xxx.xxx)...
Selecting best server based on ping...
Hosted by Vodafone UK (London) [0.96 km]: 26.941 ms
Testing download speed........................................
Download: 301.22 Mbits/s
Testing upload speed..................................................
Upload: 136.64 Mbits/s
~~~

Huh? After a bit of digging it became apparent that my (rather expensive) router was the bottleneck for my spangly new gigabit broadband. I'd always thought that my internet connection would always be the cap on everything, and now it was the hardware in my own LAN causing the problems! Again, as any tech geek would do - this now became "Mission Remove Bottlenecks".



[ho]: http://www.hyperoptic.com
[billion]: http://www.amazon.co.uk/gp/product/B00HDK4GAK/ref=as_li_ss_tl?ie=UTF8&camp=1634&creative=19450&creativeASIN=B00HDK4GAK&linkCode=as2&tag=slocooclu-21
