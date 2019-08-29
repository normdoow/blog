---
layout: post
title:  "What it's like Building a Startup in 24 Hours...LIVE!"
date:   2019-8-26
description: At 6am, on August 10th 2019, my buddy Drew and I clicked the "Start Streaming" button to go live on Twitch! We were attempting to do quite the task - build a startup in 24 hours. We had seen some other indie makers do similar things such as @thepatwalls or @levelsio. The plan was to try out a business idea and validate it as quickly as possible. Doing this in public would force us to actually make it happen and keep us accountable.
---

<p class="intro"><span class="dropcap">A</span>t 6am, on August 10th 2019, my buddy Drew and I clicked the "Start Streaming" button to go live on Twitch! We were attempting to do quite the task - build a startup in 24 hours. We had seen some other indie makers do similar things such as @thepatwalls or @levelsio. The plan was to try out a business idea and validate it as quickly as possible. Doing this in public would force us to actually make it happen and keep us accountable.</p>

Limiting ourselves to 24 hours would force us to make a prototype as fast as possible to validate the idea. I think limiting yourself in this way is a really good practice. Why build tons of custom code and spend loads of time on an idea that may not even fly?!

I had a great setup for the stream. I was actually in my brother-in-law's basement so that I would be in a quiet place where I wouldn't be too loud and distract my family, especially overnight! I had my laptop, mic, second monitor, comfy chair, food and water - everything you need for 24 hours of coding! 

<center><img src="/assets/img/setup_tweet.png" alt="" /></center>

And with that, we were off to the races! I began by making a tweet to announce the start of the stream.

<center><img src="/assets/img/startup_tweet.png" alt="" /></center>

The tweet actually did pretty well! [Pieter Levels](https://twitter.com/levelsio) retweeted it, allowing it to go somewhat viral (at least for me). It ended up getting 10,500 impressions, which is the most I have ever gotten on a tweet. This is the kind of hype we were hoping for. This helped get my stream off to a great start.

[Drew](https://twitter.com/DBids35) made a post to the [/r/EntrepreneurRideAlong](https://www.reddit.com/r/EntrepreneurRideAlong/) subreddit. He got a ton of traffic to his separate stream from this. His post ended up being the top for the day and got 60 upvotes.

<center><img src="/assets/img/reddit_post.png" alt="" /></center>

### The Product

I should probably give a little context on what we were building. It is a SMS text messaging app called [SnoozeYouLose](https://snoozeyoulose.io/) that helps you keep accountable to wake up. 

A user would pledge an amount of money and the time that they want to wake up every morning. At their wake up time, we would send them a text with a simple math question. If they woke up and answered it correctly within 5 minutes they were in the clear. Otherwise, if they snoozed, they would have to pay the money that they pledged! Half of the money would go to a [non-profit organization](https://www.charitywater.org/) to provide water for those in third world countries that don't have easy access to it.

It was a fun idea and we thought it may be useful to people to help them in their morning routine.

### The Stream

The stream went really well! At the height of my stream, I had 37 people watching simultaneously. On average, there were 15 people watching at all times. [Drew](https://twitter.com/DBids35)'s stream did even better! He had 30 people watching at all times.

Overall, I had 550 unique people and [Drew](https://twitter.com/DBids35) had 850 come through the stream during the 24 hours. It really helped build hype for what we were building.

It was really exciting to see viewers interested in [SnoozeYouLose](https://snoozeyoulose.io/) and want to interact. We had some viewers that helped us through some road blocks and hard situations.

There is definitely something to be said about having a live audience while you are trying to code. On one hand, it made me more efficient and forced me to move quickly because I knew there were people watching. On the other hand though, it was distracting at times because there was so much going on! Viewers commenting, [Drew](https://twitter.com/DBids35) talking, Twitter notifications coming in. It was crazy!

All in all, I think it definitely helped give us accountability and push us towards our goal of validating an idea quickly.

### The Road Bumps

Everything wasn't all just fine and dandy during the stream. We hit some hard spots! We had done some planning beforehand (which I definitely recommend) to help create some kind of roadmap for how we would build [SnoozeYouLose](https://snoozeyoulose.io/).

But you know how planning goes...things always change! We had planned to use [Typeform](https://www.typeform.com/) to collect user info and credit card information. [Typeform](https://www.typeform.com/) has a nice integration with Stripe, but we found out during the stream that it only allows you to do one-time purchases. We needed it for collecting a credit card that we could charge later (Once a user didn't wake up at the time they specified).

We had to find another solution for this that wouldn't take too long. We didn't want to have to develop the code all ourselves since our time was limited. We found Paperform from a recommendation by a viewer. It's very similar to [Typeform](https://www.typeform.com/), but supposedly had a better integration with [Stripe](https://stripe.com/) (more on this later).

### The Crash

After we got through the [Typeform](https://www.typeform.com/) hiccup, things were going really well! We had finished most of the features by 9pm that evening. We thought we were on track to easily finish it on time.

Then the crash came! By 3am, both of us had gotten really tired and we were up against one of the hardest problems yet to solve: time zones and daylight savings! What made this problem so hard was that our app didn't run on a device. All the code was running from a server. We weren't able to easily grab a user's local time. So instead, we had to take in their time from a form and somehow convert it to UTC time correctly. 

There are a gajillion different timezones and variances. We didn't want the user to have to select through a huge list. So instead, we had the user input their current time locally and then we would just use that as the offset. This wouldn't account for daylight savings, but we figured we could iron out that part later.

This plan would have worked, but since we were so tired, we did some of the conversions incorrectly. We had to fix this a day after the stream finished :(

### The Launch

We finished just about everything by 7am Sunday morning (25 hours after we started). We launched to [Product Hunt](https://www.producthunt.com/) and posted to [Hacker News](https://news.ycombinator.com/) and the [Indie Hackers](https://www.indiehackers.com/) community. It felt good to finally be done. We were ready for a nap!

We had done some testing, but not as much as we would have liked to because of the time crunch. Right after we launched, I went through the entire process of making a [SnoozeYouLose](https://snoozeyoulose.io/) account and trying out the features.

We had put a field within [PaperForm](http://paperform.co]) for the user to enter their credit card in, but clarified that we would not charge them today. We would only use it to charge them later if they snoozed.

<center><img src="/assets/img/paperform_button.png" alt="" /></center>

Well, when I tried this out, it charged my card right away! This was terrible. People would think that [SnoozeYouLose](https://snoozeyoulose.io/) was a complete scam. We had to quickly remove the field where we took credit card information. [PaperForm](http://paperform.co]) was not going to work for this.

We wouldn't be taking anyone's credit card for the launch. We would have to add that feature later. For now, if someone snoozed, we would just tell them that they got a free pass for the day. This was definitely not ideal. Instead of getting someone to sign up and get their credit card information right away, we would have to ask them again later which would most likely make less people fully complete the signup.

Other than this, the launch went pretty well. We got 89 upvotes on [Product Hunt](https://www.producthunt.com/) the first day. We were seventh for the day. I was hoping that we would get in the top 3 spots, but seventh wasn't terrible.

We had 35 people sign up to use [SnoozeYouLose](https://snoozeyoulose.io/). That was pretty decent. I think it showed that this idea could be promising. Time will tell if it proves to be valuable to users and if they will keep using it. At least this was a good starting point!

### The Lessons Learned

1) Starting a startup in 24 hours is very challenging! You need to do a lot of detailed planning beforehand to make sure it goes smoothly. 

2) The scope of the project has to be on the smaller side. Find really quick ways to create and validate the idea. 

3) You can drum up some extra interest through the hype of starting something in 24 hours. The accountability that comes is really amazing. You can make some cool connections with your viewers and they will want to root for you. One way that helped us in adding to the hype was making posts to relevant subreddits and groups online. 

4) Try to figure out the hardest parts of your project first before you get too tired. Our tiredness definitely hurt us the last few hours and probably made our launch not as successful as it could have been.

5) Make sure that you have enough time to make your product solid. If I were to do it again, I would probably take five days so that I could build something more substantial and make sure all of the bugs are squashed before the product was launched.

All in all, it was really exciting to build something live in 24 hours! I'd love to hear your feedback and thoughts, and about your experiences launching your own products. Connect with me on [Twitter](https://twitter.com/noahwbragg)!

If you want to see the the livestream of me building [SnoozeYouLose](https://snoozeyoulose.io/) you can see it [here on YouTube](https://www.youtube.com/watch?v=9enyvhpUuvM&t=3916s)

### Support

Thank you for taking the time to read. If you liked it, sharing the [thread on Twitter](https://twitter.com/noahwbragg/status/1167079814513201158?s=20) is really appreciated!

<center><a href="https://twitter.com/noahwbragg/status/1167079814513201158?s=20"><img style="max-width: 60%;" src="/assets/img/twitter_24_hour_startup.png" alt="" /></a></center>

