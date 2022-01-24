---
title: 'How I Built my MVP as a (relatively) shit Programmer'
date: 2022-01-11 00:00:00
featured_image: '/images/demo/hodlernews_featured.jpg'
excerpt: If this project taught me anything, it’s how far you can get by just starting small, and adding things one by one.
---

![]({{ site.baseurl }}/images/demo/hodlernews_featured.jpg)

#### TL;DR
* I started with the programming language and framework I was most familiar with, which in my case is Ruby on Rails. Sounds obvious, but a lot of people go out and try to learn the hot, new technology out there. 
* I followed tutorials like Build A Clone of X in rails. If you can, start with something like this. Find the tutorial that is closest to what you want to build. 
* I used gems and external libraries to help me build the more fancy features


#### Rails
I love programming in Ruby. It’s the first programming language I learned and I loved it so much, I decided to go and get a job where I can do some programming. After I started working in tech, I realised that having to look at Java code is quite different to programming in rails, and I found this much less fun than I expected. 


#### Build a Reddit Clone Tutorial
At its core, the product I wanted to build was a forum. So I found a reddit clone tutorial on YouTube and followed it step by step. This turned out to be very useful because the tutorial included bits of code that I would have never been able to add myself. For example, this snippet of code deals with ranking posts on the homepage. While I’m sure I would’ve got around to this, I’m not sure I would have had this kind of system ready for the MVP, had I not come across this great tutorial.

![]({{ site.baseurl }}/images/demo/hot-score.jpg)


#### Build a Job Board
The next thing I wanted to build was a jobs board. In terms of implementation, this was pretty similar to implementing the normal posts. 


#### The Front End
I realised that using HTML tables made laying out my job board page much, much easier. I then used sites like coolors.co. I took inspiration from the indie hackers website and decided that darker = better. 

![]({{ site.baseurl }}/images/demo/indie-hackers.jpg)




### The Fancier Stuff

#### Nested Comments
The first challenge I had was trying to implement nested comments into my app. A nested comment is where a user can reply to a comment and can create threads of nested comments that way. This was a situation where it took me much longer than expected. 

![]({{ site.baseurl }}/images/demo/nested-comments.jpg)

#### Rich Text
Rich text allows users to format the text when they’re writing on your site. This is meant to be very simple in rails. Action Text comes as standard, and you can just enable it. Except that no matter how hard I tried, I couldn’t make this work. Instead, I had to use an alternative called TinyMCE. 

![]({{ site.baseurl }}/images/demo/rich-text.jpg)

#### Stripe
Finally, there was the issue of collecting payments. Initially, I went with Paddle instead of Stripe to take care of payments. My reasoning was that Paddle also takes care of tax issues, which is a big plus. But I found it quite hard to integrate Paddle, and there was just far less documentation available when compared to Stripe. And mid-way through, I also realised that Stripe has recently launched Stripe Tax, which means they take care of tax issues too! So at this point, I gave up on Paddle and switched. And after a lot of struggle with webhooks, I managed to implement Stripe.

![]({{ site.baseurl }}/images/demo/stripe.jpg)


#### Getting Ready for Launch
There were a few extra things I needed to add to get my site ready for launch. The first thing I did was add analytics. I’m using segment.io and google analytics for this. Google analytics gives me a high level overview of how many people are on my site in real time, and how many people have visited for the day. Segment allows me to track behaviours. It allows me to see when someone has signed up.  The next thing I did was load testing my website. I wanted to know how much traffic I could handle, in case the launch went really well (a guy can dream). Finally, I signed up for the 14 day trial of helpcrunch, so I could add a feedback box to my homepage. This allows users to report any bugs or things they don’t like, and means I can resolve these much quicker. 

![]({{ site.baseurl }}/images/demo/analytics.jpg)

#### Putting it in the Hands of Users
After doing all of this, I plucked up the courage to post about my new project on Hacker News. For those that don't know, Hacker News is a forum where nerds hang out. After posting on here, I was able to get some really valuable feedback from lots of different people. The Hacker News crowd tends to have a lot of technical expertise. 

![]({{ site.baseurl }}/images/demo/hn_feedback.jpg)


#### Conclusion - Building Brick by Brick
If this project taught me anything, it’s how far you can get by just starting small, and adding things one by one. Now that the MVP is built - it’s time to put it out into the world. Let's see how it goes!

If you're curious - here's a link to the MVP I've been talking about so much!

<a href="https://www.hodlernews.io/" class="button button--large">My MVP</a>