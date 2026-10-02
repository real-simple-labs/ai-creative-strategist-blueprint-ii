---
title: "Parker course — Week 6 transcript"
date: 2026-10-01
session: "Week 6 — Landing pages and putting the system together"
source_type: "Uploaded VTT transcript"
source_file_name: "GMT20261001-160133_Recording.cc.vtt"
source_provenance: "File supplied directly by Alex"
---

# Parker course — Week 6 transcript

Verbatim caption export from the October 1, 2026 Parker course session. Captioning errors and timing are preserved.

Transcription artefacts noted for retrieval only: “Cloud Code,” “Claw Code,” and similar variants likely refer to Claude Code; “codes/codecs” to Codex; “Parker/Pocket desktop” to Parker Desktop; “Grooms/Gruens” likely to Grüns; “Avatorel” to advertorial; and “URL love it/you'll love it/EuroLovett” to URLlovett. No corrections were made to the transcript body.

```vtt
WEBVTT

00:00:08.000 --> 00:00:15.000
What's up, peeps? Happy Thursday.

00:00:15.000 --> 00:00:19.000
Who's ready for the last session

00:00:19.000 --> 00:00:24.000
Of this course.

00:00:24.000 --> 00:00:36.000
How are you feeling, guys?

00:00:36.000 --> 00:00:46.000
There we go, we want more session. Might have to charge through if we do more sessions.

00:00:46.000 --> 00:01:02.000
Feeling lazy. It's been awesome, pretty good. Let's go. Hey, you guys are the you guys are the real MVPs. Thank you for joining for six whole weeks. It's a huge commitment. I know we do two. I mean, if you include the Q&A, it's three hours a week, so, like.

00:01:02.000 --> 00:01:24.000
Jimmy and I, from the bottom of our heart, we really do appreciate you. He might be jumping on soon, I also know that he is, at the airport right now, because he was in San Francisco for some things, but I'll be here to talk through landing pages with you guys today. I'm super excited, so, thank you, everyone, again, for joining, and we are so, grateful for each and every one of you who spent the time

00:01:24.000 --> 00:01:47.000
in the lead up to Q4 with us here. First thing I want to say before we get started as an aside, not not around landing pages is guys, I don't know what you guys have been building over 5.5, but it's freaking wild. Like I was doing a lot of my stuff on Astra or like my heavy hitting stuff on Astra until last week, but Astra just eats credits

00:01:47.000 --> 00:02:02.000
I've been building things on Opus 5.5 that I'm like, genuinely, this is an insane step up, and not even for that, like, not even that expensive token-wise. Like, I've still got a good amount of my usage, but I've been absolutely slamming landing pages this week.

00:02:02.000 --> 00:02:12.000
As I was trying to like prepare the chats that are like presentable to show to you guys today. I want to show something super quickly. Again, I'm not

00:02:12.000 --> 00:02:16.000
And we're going to go into landing pages in a second

00:02:16.000 --> 00:02:25.000
Look at this though. And you might have seen people on Twitter sharing this too. I literally asked

00:02:25.000 --> 00:02:40.000
Opus 5.5 to go inside of our like brain, we've got an internal Parker brain just for our company. And it just said, go and look inside our brain and create us a launch video.

00:02:40.000 --> 00:02:55.000
And that was it. Like, I didn't do anything else. I just said, you've got the context. Actually, no, I said, I said, look at my Twitter bookmarks, because I'd bookmarked a load of tweets about a launch video, making a launch video on Opus 5.5, and I was just like, this probably won't work, but go and make a launch video for

00:02:55.000 --> 00:03:25.000
I don't want to decide what feature it is, or what it does, or whatever. Let's just go make a launch video. One shot. And again, I wouldn't post this, but like I was staggered that it was able to do this with zero input from me. This was literally the one shot output.

00:03:41.000 --> 00:04:01.000
I mean, isn't that insane? Like, it literally did that in court. That wasn't like using Higgs field or using any MCP. Like Claude Opus 5.5 made that with no prompting. I could have like I could have said, let me step in and work on the storyboard, or here's what features to look at, or here's the B roll I need you to collect

00:04:01.000 --> 00:04:23.000
But I thought that was like incredible. Yeah, no prompting at all. Like literally one shot. Now, it did take three hours to run, but like, I mean, it was one shot. I literally just put in the prompt and then I just let it go. And then three hours later it came out with that video and I actually now might make a real launch video for us inside of Opus 5.5.

00:04:23.000 --> 00:04:27.000
And it asked, how did you give access to your ex? Remote control?

00:04:27.000 --> 00:04:41.000
Sorry, not remote control, browser control. So I just say go and take over my browser and go through my expert marks. It's not an API, it's not an MCP or anything. It literally just went through my X… like, I saw it scrolling on my X, it went to my bookmarks, and it looked all the tweets.

00:04:41.000 --> 00:04:50.000
resources and recordings are all available. If you go in the Notion, everything's up to date now. All the skills, all of the

00:04:50.000 --> 00:05:00.000
All of the videos, all the transcripts, they're all inside of Notion. Melody will put the link in the chat in a moment, so you can see,

00:05:00.000 --> 00:05:10.000
So you can see everything from this course. Also, we'll be putting out a GitHub if anyone's interested with access to everything from the course too. So I mean, that's coming your way too.

00:05:10.000 --> 00:05:15.000
So let's talk about landing pages. I actually think today's one is going to go the

00:05:15.000 --> 00:05:34.000
full hour, it might not. If we do, we can just fit in with some Q&A, and I have a special guest for you guys, coming in in the back half of the session, and I think you're gonna like who it is. So I'm going to cover landing pages, I'm gonna do some other landing page stuff. I want to show you guys how I've been building landing pages in Claude Code

00:05:34.000 --> 00:05:38.000
I do most of auditing pages in Claude Code now

00:05:38.000 --> 00:05:48.000
For the brands that we work with, and I'm just going to share the process. And for those of you who are here two weeks ago for the,

00:05:48.000 --> 00:05:50.000
For the

00:05:50.000 --> 00:05:57.000
Static building session. It's a very similar process to that.

00:05:57.000 --> 00:06:06.000
So I'm going to walk you through it. First thing I want to show, as this is the last session, is like, I just want to circle back to the

00:06:06.000 --> 00:06:22.000
Figma diagram that we showed at the beginning of this course. And I mean, it's just been so interesting throughout this course to see how like more and more of this stuff now could be done through agents. You know, we looked at research at the start, research and ideation. Jimmy talked through skills

00:06:22.000 --> 00:06:38.000
And the idea of building a brain that can research. We talked through last week creator management and the creator sourcing, how to do that agentically, video editing we looked at last week as well. We did a session on statics, and then that could easily be applied to video as well.

00:06:38.000 --> 00:06:41.000
And then if anyone was here on

00:06:41.000 --> 00:06:43.000
on

00:06:43.000 --> 00:06:55.000
Tuesday for Andre's session, he talked about media buying and basically how he's got this entire system automated, which if you haven't seen that session yet, I would highly recommend it. It was really good, pretty advanced, but it was really good.

00:06:55.000 --> 00:07:10.000
So, it's just crazy now how, like, with enough elbow grease, like, the one-person creative team is… it is real, it's a thing. And if you can spend enough time to actually, explain the processes that you have and build into coding codecs, you can

00:07:10.000 --> 00:07:14.000
become a one-person creative team, which is extremely exciting

00:07:14.000 --> 00:07:24.000
Why are landing pages important? Well, as many of you guys know, and you've seen the podcasts and, you know, the content online

00:07:24.000 --> 00:07:41.000
Chad from Gruins literally went on, I can't remember which podcast it was, was it Open Residency or was it MFM? I don't know. And basically just said that like a big part of their creative process has been building specific landing pages for specific personas

00:07:41.000 --> 00:08:03.000
So not just sending, you know, everything to the PDP or not sending everything to collections paid or page, or, or, you know, a specific landing page, but, like, building actual, persona-based landing pages for the different personas. And as we know, Facebook is moving towards or already is in a world where it's all about persona-based advertising. And if you can make an experience that feels

00:08:03.000 --> 00:08:23.000
tailored to the specific persona that you're talking to, then you are going to be more likely to convert than, if you don't have that as a part of your strategy. I did a LinkedIn post on this recently where I just basically… I actually went inside of Parker and… or, like, the Parker MCP, and I said, go and study all of Gruens' pages in their ad library, and

00:08:23.000 --> 00:08:34.000
produce me a report. They've got 47, or they had 47 unique landing pages, running at that time, and 16 of them were persona-based landing pages.

00:08:34.000 --> 00:08:50.000
Which I thought was interesting, and, you know, you might be watching this and going like, well, I don't have, I don't have the team internally to be able to go and spin up that many landing pages to match, you know, the level of creative that we're already putting out, and that's what I'm trying to help you with today. I'm trying to allow people who

00:08:50.000 --> 00:09:05.000
Don't necessarily have the resource to put out a lot more landing pages, on their own using Claude Code, because I literally, I mean, I'm going to show you some examples in a minute, but I ran, like, all of these ran this morning. I created all of these landing pages.

00:09:05.000 --> 00:09:16.000
And we're going to walk through the exact process they use to make them, but like literally all of these made natively inside of Claude Code with Opus 5.5.

00:09:16.000 --> 00:09:20.000
Now, here's what I'll say about this process

00:09:20.000 --> 00:09:38.000
Do I think that should you expect to be able to make flashy, like extremely well designed landing pages like this? Possibly if you have enough elbow grease. But I think it's less likely that that will be the case

00:09:38.000 --> 00:09:56.000
Because there are a lot of, like, elements on this landing page, which is just a very good design. You can maybe get it there if you worked enough, but I worked in it enough, but I actually haven't done, like, tried to push these pages to the limit like this, with these kind of, like, animations and, like, elements like this. I actually find this is, like, a much better use case of what I'm about to show you

00:09:56.000 --> 00:10:13.000
Is making simple landing pages. And the good thing is, simple landing pages convert. Like, we've got many clients internally who have had extremely simple landing pages, and we've run them for years, and if the copy's good enough and the messaging is good enough, and it's paired with the right ad, they can go and spend a lot of money profitably for your brand.

00:10:13.000 --> 00:10:31.000
So, I mean, all of these, I spell out this one, but, like, advertoros, for example, I think this is a great use case for these because they're not like super complex design-wise, like this Gruens one. They're easy to put together. If you have a brand brain and you have the right context, you can have it

00:10:31.000 --> 00:10:43.000
You can have it, like, put out code that's pretty good and ready to go. You can spin out so many of these so quickly. Simple land page like this, this is another one. This was done, this morning with

00:10:43.000 --> 00:10:59.000
with Opus 5.5. Again, like, I had all of the brand assets inside of here, and I was able to spin up this template based, spin up this land page based on one of my templates, and if I wanted to create five different versions of this for 5 different SKUs or five different personas, that's just one prompt, and I can have it done instantly.

00:10:59.000 --> 00:11:06.000
So how do we go about doing that? Let's go into Claude.

00:11:06.000 --> 00:11:18.000
I need to find my artifact. Okay, so you guys remember this? This is from two weeks ago. Hopefully the chat is not in the way for you guys.

00:11:18.000 --> 00:11:29.000
So, this was the statics workflow that I showed you. And if you remember, the principles from this, it was very much like, you know, it was

00:11:29.000 --> 00:11:37.000
built in a way where there's human in the loop, so you get to dictate, like, what statics are built for your brand.

00:11:37.000 --> 00:11:41.000
And I've basically got the same process for

00:11:41.000 --> 00:11:57.000
Landing pages or a similar process, and I've actually got a similar diagram I can show you guys, here. So this is my process for landing pages. Not too different at all, virtually the same, the same graphic that I've used here. So, what we're going to be going through is

00:11:57.000 --> 00:12:16.000
the template, swipe bar, again, like Andre and Ruslan covered this on Tuesday. It seems to be a common theme in pretty much everyone who I know is… who is pumping out a lot on Claude Code or Codex. Like, the idea of having themes or templates or a swipe file, whatever you want to call it, like, of statics, of landing pages.

00:12:16.000 --> 00:12:21.000
Whatever you're building, having that bank of templates to go off of

00:12:21.000 --> 00:12:36.000
It's been something that I've seen like nearly every person that I respect in the space that's doing it, running. That's what Rusline called themes, what I call templates in this white file. We're going to go through building a swipe file together again

00:12:36.000 --> 00:12:49.000
And that's going to be what we are able to pick from when we are creating a new landing page, whether that be for a new persona, whether that be for a new SKU, or whatever it is.

00:12:49.000 --> 00:13:12.000
Research the brand and the copy. That's actually going to be the same as the process from two weeks ago. So I've built in, as I showed you guys, research and context docs onto like how to go about writing copy. I've also done like the similar thing with the document that we created with like, you know, for a landing page, this is what I think about landing page copy. This is how we write it. And then I just basically

00:13:12.000 --> 00:13:15.000
I'm going to show you how we direct the

00:13:15.000 --> 00:13:35.000
skill to just use as much customer… voice of customer language as possible, or influence… have that influence the copy, and I found that the copying landing page has been pretty good. Approve the copy, build the page, check the build. We have a review agent that is going to just go through it on mobile and desktop and make sure that there is nothing that's out of place, nothing that's weird design-wise

00:13:35.000 --> 00:13:55.000
When I first started doing this, I'd get some, like, things that I'm like, oh, this just doesn't make sense. Like, you wouldn't design like this, or there's a big gap here. That's what that review agent's going to do. And then we have the final page. And then we're done. Super simple process. It's also, again, built in a way where we're going to give it feedback. So we're going to give these templates feedback, and then the better

00:13:55.000 --> 00:14:20.000
the more feedback we give it, the better they're gonna get, and then just over time, you're gonna have maybe 5 different landing page templates for your business that you can go spin up 10 of these, and it can be good to go. And, you know, Grooms has 16 across their accounts, so maybe you don't even need that many, but, like, it's just good to be able to put out a bunch of these, really quickly, and to a good standard so that you can test them inside of your ad account

00:14:20.000 --> 00:14:25.000
Okay, so let me just check my notes. I don't have my mods today, so I've got

00:14:25.000 --> 00:14:39.000
Okay, let's start off with, brand assets. Now, we covered this two weeks ago, but I'm gonna cover it again, just for those of you who weren't there. So the first question you may be thinking is, how… how

00:14:39.000 --> 00:14:54.000
How do we make sure that, like, the landing pages that we build have assets that they can build with? Because obviously if you just got a text-based item page, I mean, that's one way you can do it, but like you obviously want to make sure that you have some assets on there

00:14:54.000 --> 00:14:58.000
So, sorry, I have a ton of chats open right now.

00:14:58.000 --> 00:15:01.000
What you can do

00:15:01.000 --> 00:15:02.000
Is

00:15:02.000 --> 00:15:12.000
I'm assuming everyone here or everyone should if you're in this course, have by now a brand brain or client brain set up. Again, I'll show you ours if you are

00:15:12.000 --> 00:15:26.000
If you don't have one set up, or if you're just curious. So this is our brand brain for the perfect gene that has everything about the brand inside of here, all the context pulled in from all our different connectors, as you guys know, because you've been in the course, Slack

00:15:26.000 --> 00:15:38.000
Google Calendar email, ad account, everything pulling into this brand brain updates in real time, shared with the team via the Pocket desktop app. Inside of here

00:15:38.000 --> 00:15:58.000
I've just had it create a folder called brand assets, and basically you can do this in a prompt. You can say, I'm going to be building some landing pages in Claude code for this brand. I want you to look at the landing pages to our active ads, look at our website, look at our statics, and basically just compile a mega folder of all of the assets

00:15:58.000 --> 00:16:00.000
That

00:16:00.000 --> 00:16:17.000
That I need to build my landing page and you're going to create a folder inside of my brand brain called brand assets. And this is what the skill is going to reference. So when we build the skill, we are going to always reference the brand assets folder because then it's going to go in here and it's going to pick

00:16:17.000 --> 00:16:21.000
the relevant, the relevant assets that it wants to use.

00:16:21.000 --> 00:16:34.000
It's a bunch of static ads here. You can even put video ads in here. I think groomers do that a lot on their landing pages. They just put video ads straight into these look like Wistia links, I think.

00:16:34.000 --> 00:16:50.000
But yeah, just collecting all the different assets from everywhere, or everywhere that you've got them. You can have it scrape Google Drive if you want it, or Dropbox, or wherever you've got files, and you just want, like, one master file with all your brand assets in your brand brain, and make sure it is somewhere on your

00:16:50.000 --> 00:17:00.000
Desktop that, like, it's easy to reference, so that's why we just keep it in the brand brain for us, so that now when we build the skill, we'll just say, look inside of this folder.

00:17:00.000 --> 00:17:06.000
And then we're going to build the swiper file. So first of all, let me show you mine.

00:17:06.000 --> 00:17:20.000
I… there's no right way to build this swipe fault. That's not it. This is it. There's no right way to build a swipe file of landing pages. The same thing I said to you guys about ads.

00:17:20.000 --> 00:17:42.000
If you've already got a swipe file of landing pages that you like, and you think are good templates, great, use that. If you don't, I'm going to show you how to make one in a second, but it's really, really simple. These are some swipe… these are some landing pages that I like. I've just got them saved in this artifact here, as you can see. I can scroll down them, and I've categorized them into different templates. So I have a

00:17:42.000 --> 00:17:58.000
a swipe file for… I have a category for listicles. I have a category for founder stories with the long piece of copy advertorials, product page, like style, and then offer based Lambda. Again.

00:17:58.000 --> 00:18:17.000
the actual name, I probably could do a better job at, but, like, these are all the different styles that I like to build mine off, and you don't need that many templates, because at the end of the day, there's not that many different types of, landing page that you can make, but, like, the important thing here is you can get good templates inside of here, that you can easily build off of. If you know that listicles work for you.

00:18:17.000 --> 00:18:22.000
Go and find a bunch of listicles. If you know that advertorals work for you

00:18:22.000 --> 00:18:40.000
And go and put a bunch of them in your swipe file and I can't emphasize this enough, the same thing with static swipe file, the ceiling of the landing pages that you can create is dictated by how good, or is at least partially dictated by how good the swipe file is. So it's worth spending the time to make sure, in the same way that the static swipe file

00:18:40.000 --> 00:18:50.000
We spent a lot of time making that swipe file good. This too, you want to make sure it's good, you don't have to have that many in there, but as long as you like pretty much every single

00:18:50.000 --> 00:18:54.000
Every single one inside of here, then,

00:18:54.000 --> 00:19:03.000
You're in a good spot because this is what we're going to be building the landing pages off of. I'm going to start the skill and the skill is going to go, okay, which template do you want me to select?

00:19:03.000 --> 00:19:11.000
If I choose this one from the perfect gene, then it's going to build a landing page like this for the brand that I say to execute it for.

00:19:11.000 --> 00:19:18.000
So spend a lot of time building your swipe valve. If you don't know where to look for

00:19:18.000 --> 00:19:21.000
If you don't know where to look.

00:19:21.000 --> 00:19:22.000
for

00:19:22.000 --> 00:19:32.000
swipe, full landing pages to put in your swipe file. Here's what you can do. You're gonna have the Parker MCP installed, and you're gonna say something like this.

00:19:32.000 --> 00:19:34.000
I am

00:19:34.000 --> 00:19:40.000
Building a skill where I am building a landing page

00:19:40.000 --> 00:19:53.000
Builder inside of Claude code. Now, to do this, I need a swipe file of landing page templates to base it off of. I want you to look into the following brands that I think do make really good

00:19:53.000 --> 00:20:02.000
Landing pages, and I want you to collect their most successful landing pages by looking at the ads that are performing for them by impressions

00:20:02.000 --> 00:20:11.000
And put them down on an artifact for me to select which ones I want to put into my swap file

00:20:11.000 --> 00:20:23.000
And you can either list the brands that you want, I could say rac, IMA, yada, yada. Or you could just say, go into the Parker database of

00:20:23.000 --> 00:20:35.000
Or after that, go into the Parker database of the millions of ads and find some of the most prominent supplement brands and look at their

00:20:35.000 --> 00:20:46.000
Best landing pages and suggest them to me. I'm not going to take all of the ones that you suggest, but I just want to be able to select the ones that I think are the best and then we'll build the score off the back of that.

00:20:46.000 --> 00:20:58.000
You go and do that, that's going to go and put together an artifact that you can just basically, you know, choose. Like, I want this one, this one, this one, this one, this one, and that's gonna leave you with a

00:20:58.000 --> 00:21:16.000
That's gonna leave you with a page that looks something like this. You've got your landing page swipe file, you now have step one of this process complete. And the reason why this isn't going to take that long is, guys, this is going to be the same process as the static workflow, so if you were here for that session, you know what's going to happen now

00:21:16.000 --> 00:21:24.000
It's going to go through and go through the exact same process. I do see any questions in the chat? Are they

00:21:24.000 --> 00:21:25.000
Okay.

00:21:25.000 --> 00:21:31.000
Okay, the questions come in the chat or the Q&A. I'll get to them at the end.

00:21:31.000 --> 00:21:37.000
So yeah, sorry, I'm trying to, I'm going with Jimmy today, so I'm trying to balance. Okay.

00:21:37.000 --> 00:21:52.000
Research the brand and check the copy. For the sake of time, because I do want to give some time to the person who we have coming on shortly. The process for this is exactly the same as the one I shared two weeks ago. If you go into Notion, you'll see the

00:21:52.000 --> 00:22:07.000
recording from the static workflow. And I want you to I had a look at what I did there. I mean, there's not too much different than I do here, really. I just I gave it some context about

00:22:07.000 --> 00:22:25.000
about the research process for a research and copy process. For landing pages, but I've actually found it to do a pretty good job, even without much of it. If you give it a good swipe file, and a good template to go off of, and then it has all of the information already in the,

00:22:25.000 --> 00:22:42.000
In the brand brain, then I just direct it, and I said, now I want you to build the skill itself. Here is the process that I want you to follow. Make sure when you're doing the research and the copy, you always take inspiration from customer reviews and comments and any other voice of customer we

00:22:42.000 --> 00:22:48.000
inside of Parker, you could say inside of wherever.

00:22:48.000 --> 00:22:59.000
This is what you should use and then just mirror what like make a version of what you see on the template for us using our VOC to inspire the copy that's created.

00:22:59.000 --> 00:23:15.000
Now, don't forget, we're also going to be approving the copy before the landing pages get built. You don't have to do that, but I prefer to do it just so I can give it a once over. And if there's anything I want to change, I can change it before it goes and builds it itself

00:23:15.000 --> 00:23:23.000
Again, you don't have to do that, I just prefer to have him in the loop, especially when I build this skill for the first time. I like to have

00:23:23.000 --> 00:23:30.000
I like to be more involved

00:23:30.000 --> 00:23:39.000
And if you wanted to build this, you could literally just say

00:23:39.000 --> 00:23:44.000
then go and build this skill. Here's the process

00:23:44.000 --> 00:23:49.000
took a screenshot of the artifact and say, go and build something like this.

00:23:49.000 --> 00:23:54.000
Once you run that, it is going to go and create

00:23:54.000 --> 00:24:02.000
So we're creating the swap file now and then it will give you a page like this. You're going to say, I want to build

00:24:02.000 --> 00:24:10.000
This template today, I want to build a list of call based on this one from Roujet. So I'm just going to select build this one

00:24:10.000 --> 00:24:25.000
Here, if I queue that one next, obviously I don't have time to wait for each of the chats here, but then I can say this is the template that I want you to build. Go and build it. And assuming you have all the context inside of the brand brain and inside of

00:24:25.000 --> 00:24:33.000
And the template is good, then it should be good to go and build it. This is literally the exact same process that I've used to build

00:24:33.000 --> 00:24:51.000
all of these in here this morning. And again, like, are these the… I mean, some of these need a little bit of adding assets for the wings brain. I don't think I asked to call the asset, so it hasn't done that yet. Some of these need a little bit of work, but, like, some of these also, I think, are pretty good to go. If we look at some of these

00:24:51.000 --> 00:24:57.000
Yeah, this is the one that needs a little bit more love. But this was a one shot

00:24:57.000 --> 00:25:14.000
With me not approving the copy, me not going and added more images for wings, I could get to scrape their site and pull in more assets. And, you know, this is a scrappy page that, like, is good to go, and I can go and generate five more versions of this. One actual, like, use case that I've, that I've had

00:25:14.000 --> 00:25:18.000
And I replicated this chat for this

00:25:18.000 --> 00:25:37.000
webinar, so it should be somewhere here. I don't know if I can find it. But anyway, basically, we had a winning landing page or an ad that had a winning ad that had a landing page that has worked for us historically worked really well. That's actually one of the templates. And I found that for this brand, the older demographic always tended to

00:25:37.000 --> 00:25:46.000
resonate with our ads, and we were starting to see some older, older people ads that were doing well. So I said, take this

00:25:46.000 --> 00:25:52.000
Template page, and I want you to make a listicle on why

00:25:52.000 --> 00:26:09.000
older people will love this product, and then it just did it, and it went and drafted like a persona based land page for me. And this is how you go and execute the groom's playbook of like different personas. You, you build your land page templates, and then you say, okay, now I want this

00:26:09.000 --> 00:26:28.000
for this persona. And then you want to build this for this persona. And because it's all done agentically, it'll pump these out super quickly, and you know, you're going to be able to test a lot more landing pages quickly. All these are one-shot, like, I'm not actually showing, like, these are our clients, but, like, I'm not showing the real client examples, because

00:26:28.000 --> 00:26:43.000
We usually keep ourselves confidential. But, I mean, these are using the same skill that we actually use, and then what you can do here is you can just start giving it feedback. So, like, this template, for example, I can say, when you have

00:26:43.000 --> 00:27:00.000
if I was in the chat, I could say, when you're working on template 3, I don't want you to include the splash on the fold. That was something that Primal Queen did in the original template, but it doesn't apply to all brands, so if it's not on brand for the brand assets, don't do it.

00:27:00.000 --> 00:27:04.000
And the next time that it runs template three from my

00:27:04.000 --> 00:27:06.000
from my playbook

00:27:06.000 --> 00:27:10.000
It is going to consider that, and it's not going to do this here.

00:27:10.000 --> 00:27:26.000
And that's how it's going to get better. Like, you're just going to keep on giving feedback to these templates. They're going to get better and better. You add more assets. And again, if you have a lot of assets inside of here, which this was just a one-shot, I haven't done any feedback on this, if you add a lot of assets inside of here, it's going to make it really easy for it to go and make

00:27:26.000 --> 00:27:39.000
Good landing pages that you can then either send straight through to the product page, or you can embed the buy button onto the landing page itself.

00:27:39.000 --> 00:27:53.000
So I mean, you could put out a lot really, really quickly. Advertorials, I put out a lot advertorials and listicles are probably my two favorite use cases for this because they're super easy to make. It's copy heavy. It's not really design dependent

00:27:53.000 --> 00:28:00.000
So you can really just, like, get it to look into the voice of customer, and look for original

00:28:00.000 --> 00:28:14.000
angles or things we haven't tested inside the ad account, and then, look for ads to pair it with and find… and go and write an advertorial for us versus competitor, or us versus industry, or whatever it is.

00:28:14.000 --> 00:28:37.000
ballistic is the same thing. They're probably my two favorites. The more, again, same thing with statics, the more design work you get it to do, the more variation you want to get in the result. But like, you know, this one came out pretty well. A bunch of these other ones as well, they're probably a few minutes away and a few prompts away from like getting them to the point where they're launchable. And again, the goal here is not to make super

00:28:37.000 --> 00:28:51.000
super pretty ones like this. If you want to do this, then I probably would still do them outside of Claude Code. But if you just want to test a lot of iron pages quickly, or test a bunch of different persona landing pages, or just have something that aligns with your ad, so your top ads

00:28:51.000 --> 00:29:04.000
then you can do that. That's another thing you could do. You could say, look at my top 10 ads, and I want you to build landing page as specific to, like, tailored to that ad, and feels like something that someone who is going through that ad would,

00:29:04.000 --> 00:29:14.000
Would be able to like what was the relevant land pages for them to land on based on one of our templates.

00:29:14.000 --> 00:29:19.000
So yeah, I mean, these are a bunch of the ones they put out this morning for me and I

00:29:19.000 --> 00:29:39.000
I haven't even reviewed half of these, because, honestly, my last call ran over. I was doing a training session, but you can put out very good landing pages when you give it the right assets, when you pick good templates here and you then just let it go to town on your brand brain and on your voice of customer. And again, not to pitch Parker, but this is why I think it's so important to

00:29:39.000 --> 00:29:58.000
Have not only your brand and brain built, but to have it connected to the ad account, and have it connected to voice of customer. If you can't pull in voice, customer reviews, add comments, post-purchase surveys, things from the organic feed, it's gonna struggle to speak in the way that your customers speak, and then you're just gonna, like, spend a lot more time

00:29:58.000 --> 00:30:00.000
In this

00:30:00.000 --> 00:30:21.000
In this part of the process, when you're approving copy and going back and forth, whereas I'm able to put out a bunch of landing pages quickly, and then I can just go over and review the copy, like, one by one, and whisper flow it, it's gonna take a lot longer if you're not doing it based off the voice of customer, which is, again, what Ruslan and Andre were saying on Tuesday, like, that is what their

00:30:21.000 --> 00:30:40.000
Their research and ideation, copyright is revolved off of. So you want to make sure that you have some way to connect it and I mean, I'm biased, but I personally think the Parker MCP is the best way because it has the most data sources to connect to and pull in straight into Claude. So you're going to have less time. You're going to spend less time reviewing and approving

00:30:40.000 --> 00:30:42.000
The copy.

00:30:42.000 --> 00:30:56.000
Again, there is… there's actually not too much to show in terms of the rest of this workflow. When you say, you know, like, desktop and mobile, like, I get it to give me the mobile version

00:30:56.000 --> 00:31:15.000
on the artifact, and I get it to give me the… when I click open page, it goes to the full desktop version, so it makes both for me. And then I just have… I just said to it, like, I want to create a… a desktop, sorry, I want to create a review agent that basically goes in and checks all the spacing in all of these.

00:31:15.000 --> 00:31:29.000
To make sure that there is not anything that looks out of line on either mobile or desktop. And it goes and does that, and that's the last part, and then it reviews and gives me the last version of the landing page, and then I can either approve it or give it feedback.

00:31:29.000 --> 00:31:45.000
And that is… that is pretty much that. And when it gets the questions shortly because I'm going to have our guests come on in a second. So that's one of the skills I have built for landing pages. This is kind of the rest of the skills that I have

00:31:45.000 --> 00:31:49.000
built over the last month or two.

00:31:49.000 --> 00:32:10.000
what I just showed you was like the new landing page here like that's the process for actually creating another landing page. But I have a skill for extracting a landing page template. So, for example, if I saw like a new template online, if I imagine this was a new temp, a new a new landing page that I really liked, I could just give it to this extract page template skill, and it add

00:32:10.000 --> 00:32:25.000
this template to my library of templates, which I think is pretty cool, because then you can, at any time, if you see something really, really nice, or you see something you know is performing, just put it in your library. New landing page, you guys saw that one, iterate landing page was just iterating on top performing landing pages.

00:32:25.000 --> 00:32:41.000
build ugly land. So here's the interesting thing. If you have things that work for you, like, if you know Avatara's crust, if you know Avaturals Crush, you can, go and build, like, an Avatorel-specific skill. Let's just, like, purely… this is… this is only context about how to build advertorials

00:32:41.000 --> 00:32:45.000
Like, for us, it's Ogiland, it's, like, listicles and stuff.

00:32:45.000 --> 00:33:01.000
QA at skill, CRO at QA at scale, CRO at scale, just review agents that have a look at the page and make suggestions on what to improve. We don't use those ones as much, it's more so these first four, or at least these three that I use the most

00:33:01.000 --> 00:33:15.000
inside of inside of here. And once there's any questions in the chat, and I'm going to hit them. But I do want to bring up our special guest very very shortly.

00:33:15.000 --> 00:33:31.000
Okay. Someone asked, would anyone want the ability to save landing pages to the Parker swipe file instead of ads or posts? That's interesting. That's probably one of the Parker team who asked that, but if you guys would be interested in that, we can make that available. It's not going to be difficult to do that

00:33:31.000 --> 00:33:50.000
Right now, I'm just pulling the landing pages from Parker. It's not actually I couldn't say this in the swipe bottle. I couldn't yet say, now go and say this in my swipe button, Parker, because we only save ads currently, but we can add that if you guys find it useful.

00:33:50.000 --> 00:33:54.000
Where are the skills? I'm going to

00:33:54.000 --> 00:34:02.000
the skills, these skills are all saved them, like, my.claude inside of the ad crick brain. So if I go inside of

00:34:02.000 --> 00:34:19.000
here, like, in the docload here, they will be saving here. I am going to put them in the GitHub. All the skills I've shared so far in this course are already in Notion, and we're going to be putting out a GitHub after this that has all the skills and all the transcripts, so you guys have access to them, but again, you can make something way, way better than me, because I'm showing you a generic version, and I had to

00:34:19.000 --> 00:34:36.000
code, so I wouldn't show you, like, actual real client chats. You can make something specific to you. So, like, take this and build on it. Make something that's specific to you, like, with your templates and with your, like, landing pages that work for you, you're mixing this way, way better, and you'll probably find three or four templates that work really well for you, and you can just

00:34:36.000 --> 00:34:42.000
Spin up a ton of landing pages with your context.

00:34:42.000 --> 00:34:51.000
Landing page inspo would be amazing. Yeah. Yeah, we can absolutely put that in if that's something that people would find useful.

00:34:51.000 --> 00:35:04.000
Yes, artifacts will also be this artifact here with the whole process, it's going to be shared in the notion doc and the notion hub, sorry. Same thing with the skills doc. Everything I've shared with you today is going to be

00:35:04.000 --> 00:35:06.000
Made available.

00:35:06.000 --> 00:35:22.000
Okay. Keep the questions coming, guys. In the meantime, special guests, please put your hand up. We're gonna bring, them on now. I want to talk about, something that we've been using internally that,

00:35:22.000 --> 00:35:33.000
has helped us, not just with landing pages, but with overall growth of the business. There is a really interesting pain point that this person has sold for, and I want to share it with you guys and just,

00:35:33.000 --> 00:35:44.000
made people aware of it, because it's something that's been very, impactful in, in our business. And here he is! This may be

00:35:44.000 --> 00:35:49.000
Probably as someone that you guys recognize, it is my good friend

00:35:49.000 --> 00:35:54.000
partner and mentor, Barry Hot. Barry, what's up, dude?

00:35:54.000 --> 00:36:10.000
It's me. Hello, I'm here. Good to see you. Thanks for having me on. I really appreciate it. Excited to chat about this. This is a great session. This course has been amazing. I really appreciate that you're doing this. And as I've said publicly, and I will say again, I think it's insane that you're doing any of this for free

00:36:10.000 --> 00:36:27.000
And I'm very mad at you for doing that, but hello, I am here, I'm also glad to be giving away stuff for free, but it's what we're supposed to do, says Alex Hormozy, so I guess if he's named Alex, I have to listen to him.

00:36:27.000 --> 00:36:29.000
That's the rules

00:36:29.000 --> 00:36:49.000
That is the rule around here. Guys, keep the questions coming in the chat and the Q&A. We're going to get back to some of the landing page builds I was doing just now at the end of the session. Barry's going to cover something on land pages that I think you guys are going to find really, really interesting. And yes, he is absolutely mocking me with his setup right now

00:36:49.000 --> 00:36:57.000
Like, I'm literally, in my kitchen on my laptop, and Barry, you've got probably the best setup in DTC.

00:36:57.000 --> 00:37:00.000
Yeah, and I'm the ugly ads guy. What's this about?

00:37:00.000 --> 00:37:03.000
Yeah. Hold on a parallel universe.

00:37:03.000 --> 00:37:19.000
Yeah, this is… no, this is all AI. Actually, I'm here to talk for 30 minutes about how to set up an AI to blur your background and make it look like this. No, it's real 70 millimeter Canon L lens. Well, 7200, but it's at 70

00:37:19.000 --> 00:37:36.000
Anyway, if any lens geeks out there, glass nerds, send me a message. But yeah, anyway, or should we dig in or do you want to chat about landing page stuff more first?

00:37:36.000 --> 00:37:37.000
Okay.

00:37:37.000 --> 00:37:38.000
Okay, sure.

00:37:38.000 --> 00:37:51.000
Let's dig in. I mean, I'm sure we'll riff. As you pull the slides up, because Barry has actually built something that we've been using a lot internally. Like I said, it's been impactful for us with landing pages, but just also overall growth, for clients and,

00:37:51.000 --> 00:37:56.000
In our own business. So I'm very, very excited.

00:37:56.000 --> 00:38:11.000
All right, sweet. And yes, I do apparently sound like Seth Rogen when I laugh. Also, funny someone noted that this looks more like an 85 millimeter. Not that I want to geek out about this, but I am stalling while I pull up my deck here. It is a 70 millimeter, but on a modifier on a connector

00:38:11.000 --> 00:38:13.000
Cool.

00:38:13.000 --> 00:38:20.000
increases it. So, it is probably closer to 85. That's a weird eye for that. That's nuts.

00:38:20.000 --> 00:38:37.000
I can't believe someone would even notice that. That's insane. But yeah, this, you know, I don't know if any of you, are any of you familiar with what I've built or what I've talked been talking about URL love it or you'll love it, as we like to call it.

00:38:37.000 --> 00:38:48.000
heard about that at all. Heard me talking about it. You know, give me a give me a some sort of emoji. Okay, some people, cool. So

00:38:48.000 --> 00:39:04.000
We're going to talk a little bit about that, and I'm actually also very much to my own pain, I'm going to give you guys a prompt so that you can basically not need to use URL love it, which

00:39:04.000 --> 00:39:10.000
Can I also explain to you why I'm going to do it because, you know, we'll see. So can you guys see my screen here? The deck?

00:39:10.000 --> 00:39:13.000
Yep, you're good.

00:39:13.000 --> 00:39:16.000
All right, well, I'm eager to see if Claude

00:39:16.000 --> 00:39:29.000
Keeps updating this while I'm going, because I'm pretty sure it's going to update a slide here, but we'll see. So really what I want to talk to you guys about on the back of talking about landing pages is what happens after people see your ad, right? So

00:39:29.000 --> 00:39:36.000
Obviously, they go to landing pages, right? But that's not always the case. First of all, a lot of people just ignore it

00:39:36.000 --> 00:39:46.000
they don't go anywhere, meant to pull out the words goes to, sorry. But yeah, so most people who see your ads ignore it. They don't click it, they don't pay attention to it

00:39:46.000 --> 00:39:47.000
They nothing it

00:39:47.000 --> 00:39:55.000
So that's the first batch. Second batch of people notice it, but they don't do anything right now. They're paying attention. Maybe it got in their brain.

00:39:55.000 --> 00:40:01.000
What a lot of us don't really think about, you know, I don't want to get too far into media buying right now, but

00:40:01.000 --> 00:40:17.000
We don't do a good job as marketers, media buyers, of really understanding what it means when someone pays full attention to an ad and doesn't click right now because they're just not ready to buy right now. But a lot of people fully pay attention to the ad. It gets stored in there and

00:40:17.000 --> 00:40:23.000
Then that leads to more stuff that can happen later down the road. That makes

00:40:23.000 --> 00:40:35.000
Like, if someone watches a 3-minute ad of yours, the next time they see an image ad from you, they're more likely to buy from it. So, there's a lot of that that's going on. We're also not going to be talking about that much more on this call.

00:40:35.000 --> 00:40:43.000
The next thing is, as we talked about, people click right away, they go to your landing page. We just talked about how to build landing pages. That's awesome.

00:40:43.000 --> 00:40:51.000
The other two things that they do is either they go straight to your .com, right, they just open up a browser and go to whatever your .com is, and go check it out

00:40:51.000 --> 00:40:56.000
Hopefully they go to the right one, knowing that I've worked with Tushy, the bidet brand,

00:40:56.000 --> 00:41:13.000
A lot of people just think it's tushy.com. That is a very different website. I am warning you right now, don't go to tushy.com on your work computer or in front of anyone. Don't do it. It's hellotushy.com, so

00:41:13.000 --> 00:41:25.000
You want to make sure that your website is easy to find. And then lastly, people are going to search your brand name and they're not just going to search the brand name. They're going to search it in like maybe look up Reddit or something else. So

00:41:25.000 --> 00:41:41.000
These are all the things. Which of these have you done? Just, you know, put in a number here in the chat if you can just like let me know like which of these you've you do frequently because I know I'm a big brand searcher

00:41:41.000 --> 00:41:57.000
I'm not a big .comer guy. Like, I don't always go to the .com, but one of the other things I often frequently do is click on the landing page, and then go to, like, escape the landing page. I'll go to go to their homepages

00:41:57.000 --> 00:42:02.000
Kind of as quick as I can, and I think a lot of people do that

00:42:02.000 --> 00:42:13.000
So yeah, just curious what, yeah, a lot of people said all. I appreciate that. Nice. Okay, cool. Thank you for… Don't link to dushy.com, please.

00:42:13.000 --> 00:42:19.000
Don't do it, I shouldn't have even brought it up. I apologize. Don't go there. It's not safe for work

00:42:19.000 --> 00:42:22.000
So,

00:42:22.000 --> 00:42:30.000
You know, every page on your site matters, not just your landing page. This is the thing that I think people don't

00:42:30.000 --> 00:42:37.000
fully wrap their heads around well. Like, I think, obviously, there's conversion rate optimization, so yes, people do understand improving their website is important.

00:42:37.000 --> 00:42:42.000
But I think there's a big gap between the people who are running ads

00:42:42.000 --> 00:42:52.000
And the people who are modifying, like, the product page or the categories page, or the home page. And I don't think there's a good enough

00:42:52.000 --> 00:43:02.000
across the industry, I don't think enough people really understand how much it matters when something changes on one of those, for better or for worse. So

00:43:02.000 --> 00:43:19.000
on your site, the homepage, product pages, category pages, shop all, the menu, cart, checkout, all of those things matter fundamentally to your customers, your potential customers, anyone who's learning about anything

00:43:19.000 --> 00:43:25.000
Someone said to zoom out, please. The text is too big because I can't tell if this is a joke

00:43:25.000 --> 00:43:26.000
Is there something wrong with my… my slides look good

00:43:26.000 --> 00:43:28.000
No, I hate the joke with you

00:43:28.000 --> 00:43:32.000
Yeah. I like a sparse slide.

00:43:32.000 --> 00:43:35.000
I don't know.

00:43:35.000 --> 00:43:43.000
Thanks. And then the next thing is, you know, pages you don't own

00:43:43.000 --> 00:43:58.000
Let me back up. One thing I forgot to do was tell you who I am. Like, yeah, Alex, you give me a nice intro, and I appreciate that. But something I forgot to do is tell you why you should listen to me about any of this. I've been advertising on Meta for over 18 years

00:43:58.000 --> 00:44:06.000
I've been doing it for a long time. I've spent literally over a billion dollars. I've studied billions of dollars in

00:44:06.000 --> 00:44:12.000
Meta ads and other ad platforms as well. I am a nerd about this. I am passionate about this

00:44:12.000 --> 00:44:16.000
I geek out about this in my spare time

00:44:16.000 --> 00:44:23.000
So when I'm really thinking about is what are the things that make performance

00:44:23.000 --> 00:44:30.000
go up and make performance go down. And the thing I've learned over time is

00:44:30.000 --> 00:44:43.000
When performance is bad, don't go change things. So many people, they see ROAS goes down, CPAs are spiking, every other metric, whatever metric you want to talk about, it's bad, okay? When it's bad.

00:44:43.000 --> 00:44:58.000
You need to know why. And for me, I'd say like 80%, maybe 90% of the time I've noticed, and then the more I noticed it, the more I notice it is that it's almost always a website change and something I didn't do and something I wasn't made aware of

00:44:58.000 --> 00:45:06.000
And the only reason I know it is and figure it out is because I study the website that we're driving traffic to. I pay close attention to it.

00:45:06.000 --> 00:45:08.000
So having done that

00:45:08.000 --> 00:45:12.000
So many times, I've learned that

00:45:12.000 --> 00:45:24.000
It's not me. If I didn't make a change in my media buying, like I didn't change a budget, I didn't change a bid, I didn't add new creative, why is performance bad? Yeah, maybe it's Zuck. Maybe it's, you know, something else macro

00:45:24.000 --> 00:45:40.000
But almost always, if it's me and it's just me and it's just this one account, and I'm asking other people and they're not seeing the same kind of thing, it's the website. The first place I always go to is the website. Second place I go is the other stuff I don't own. So Google search results for

00:45:40.000 --> 00:45:41.000
for your brand

00:45:41.000 --> 00:45:51.000
Amazon listings, reviews, Reddit, discount websites, like coupon sites that have coupons for your

00:45:51.000 --> 00:45:59.000
for your business. And then also, I might even go check competitors, see if they're having a sale, see if they're, like, shitting on this brand suddenly

00:45:59.000 --> 00:46:12.000
See if they're doing something different. Because all of those things fundamentally matter to the user, and if they matter to the user, and the user we're trying to turn people from users or visitors into customers.

00:46:12.000 --> 00:46:22.000
If it matters to them, it matters to your business. So you need to be studying these things. You need to be looking for these changes. And I mean, drop in the chat here, like, how many of you guys are

00:46:22.000 --> 00:46:26.000
Taking screenshots of your clients or your own

00:46:26.000 --> 00:46:28.000
homepage every day.

00:46:28.000 --> 00:46:39.000
Seriously, actually, just drop in there, say me if you do that. Put that in the chat if you're already doing that and bravo if you are.

00:46:39.000 --> 00:46:41.000
So

00:46:41.000 --> 00:46:54.000
Every one of these pages is changing also, right? Landing pages, we just talked about how to improve landing pages, how to build more landing pages. We're always going to be improving those and changing this. That's landing pages. There's new offers, new headlines, tons of stuff you can be doing.

00:46:54.000 --> 00:46:59.000
But there's also, like, same thing on the website. And also depending on how involved you are

00:46:59.000 --> 00:47:15.000
With the team who's building, like, building the website, fixing the website, right? If you're in a big org, you're nowhere near those people. If it's just you, you know, you're a solopreneur, then it is just you. But either way about it, you're probably not doing a great job of monitoring those changes over time, or getting those

00:47:15.000 --> 00:47:23.000
There's not a lot of teams that are very transparent with each other that are like saying like, hey, I just made this change

00:47:23.000 --> 00:47:35.000
And then you're like, thank you for telling me you made that change. Like, that's almost never happening. And even in those teams where there is that high transparency, it's so rare that they remember to tell you about every change

00:47:35.000 --> 00:47:37.000
And that's also

00:47:37.000 --> 00:47:42.000
Not even including all of the things that just change and break

00:47:42.000 --> 00:47:45.000
All the time from other things

00:47:45.000 --> 00:48:03.000
review plugins, or, you know, Klaviyo pop-ups, or whatever it is. So many things can change and break all the time, and you won't know unless you're literally going to the website every day. And I do encourage you to be visiting your website and going through the funnel

00:48:03.000 --> 00:48:10.000
Every day, if you have one, if you can't do it every day, at least every week. If you can't do it yourself, have someone do it.

00:48:10.000 --> 00:48:18.000
And that's basically what I'm building here with your Levitt is a way to monitor that. So

00:48:18.000 --> 00:48:29.000
You know, and then the last thing is that nobody's documenting this stuff, right? Even if you are, you know, one of these people here that says that they're getting screenshots all the time. Yeah, I mean, like

00:48:29.000 --> 00:48:36.000
Even if you are doing that, are just storing that with the rest of your screenshots? Are you, like, organizing that neatly into folders? Are you, like.

00:48:36.000 --> 00:48:42.000
Making that into a nice timeline that you can easily access. No, I don't think so.

00:48:42.000 --> 00:48:43.000
So

00:48:43.000 --> 00:48:50.000
You're probably not watching any of them, most of you, I assume, and that's okay. Not shitting on you guys. It's all right.

00:48:50.000 --> 00:48:57.000
But here's an example that I pulled from Ridge. This is just… I'm pulling an obvious example here, right?

00:48:57.000 --> 00:49:03.000
I would hope and expect that the media buying team, the marketers were aware of this change

00:49:03.000 --> 00:49:18.000
Right? Happening from June 22nd to June 23rd, where it's going from Father's Day sale to a more evergreen offer. But I want to note here, this is what we caught. So there's two ways to look at this. One is from the perspective of, like, imagine your ridge

00:49:18.000 --> 00:49:34.000
And the other is imagine you are a competitor, and the other is imagine you're just, like, looking at them for inspiration. Not only did they change from a Father's Day sale to this evergreen thing, look at the difference in the header. Look at the difference in the top bar

00:49:34.000 --> 00:49:43.000
The menu button literally changed from the right side to the left side. There's now there it went from having different categories in the top to not having them.

00:49:43.000 --> 00:49:50.000
And it went also from shop to sale to shop wallets, and you can even see at the bottom here, it's showing, Ridge Wallets

00:49:50.000 --> 00:50:04.000
Versus shop by categories. These are huge differences. Wild, wild differences in what people are getting when they go to the homepage and what they're experiencing and what they're thinking about. So I want you just thinking about

00:50:04.000 --> 00:50:18.000
if and how you're updating your homepage, first of all, if you are, think about how that can change who the site is relevant to, just like you'd think about how ads can change who you're, like, by changing the content of your ad, you can change who it's relevant to

00:50:18.000 --> 00:50:28.000
And I want you to also think about if you're not updating your website, not testing it, not playing with it, why not? Because there are… there is money you're leaving on the ground by not

00:50:28.000 --> 00:50:31.000
tinkering with it, not playing with it more

00:50:31.000 --> 00:50:32.000
So

00:50:32.000 --> 00:50:41.000
You know, and even if you are thinking about this, even if you did know about this on June 23rd, right, and you're like, yep, we know this change.

00:50:41.000 --> 00:50:44.000
If you're looking back historically

00:50:44.000 --> 00:50:51.000
Let's say it's today and you wanted to go back to June and you wanted to understand why did our CPAs go down? Why did our CPAs go up?

00:50:51.000 --> 00:50:55.000
Or why did click-through rates change? Or why did anything change?

00:50:55.000 --> 00:51:02.000
This is a huge factor. And maybe you have that well-documented, maybe you can see that in your campaigns

00:51:02.000 --> 00:51:03.000
But

00:51:03.000 --> 00:51:21.000
Being able to see what the website looked like on that specific day is very helpful. Now, if you're ridge.com, yeah, you can go on the Wayback Machine, I'm sure most of you are familiar with the Wayback Machine, and go and see what it looked like, but most of your websites are probably not well documented on the Wayback Machine, and certainly not all of the pages on your website.

00:51:21.000 --> 00:51:23.000
So

00:51:23.000 --> 00:51:39.000
This is an example of here's what your URL love it flagged. You can see here it caught these different details. You know, we use AI to analyze these screenshots and not just the screenshots, but also the HTML code. We're literally reviewing the code every day

00:51:39.000 --> 00:51:49.000
from the day before to the next day, to compare what changed. We can catch these things. And then we can flag what's important and what's not

00:51:49.000 --> 00:51:50.000
Now.

00:51:50.000 --> 00:51:56.000
I need that context. If I'm the media buyer here, or if this is my competitor or anything like that

00:51:56.000 --> 00:51:59.000
I need to know

00:51:59.000 --> 00:52:03.000
What's, what's happening so that I can understand why my performance is changing

00:52:03.000 --> 00:52:10.000
Here's some other examples of, like, tiny changes, but that probably matter in impact performance

00:52:10.000 --> 00:52:14.000
If it's a 1% impact, the 2% impact, it's kind of almost imperceivable

00:52:14.000 --> 00:52:19.000
When you're running meet, you know, Facebook ads, if you're running meta ads.

00:52:19.000 --> 00:52:21.000
It's really hard to see and feel

00:52:21.000 --> 00:52:36.000
When a small thing happens, you kind of just get this like feeling in your chest, you know, you kind of just feel it maybe in your gut. You're like, something feels wrong. And these are the things where you kind of like you

00:52:36.000 --> 00:52:53.000
you know, your ads kind of go to die. And most media buyers don't even think about this stuff at all, they just go and be like, alright, let me go tweak the bids, tweak the budget, let me go turn off the top, you know, let me go turn off these ads that now are worse. By the way, one of the things I often talk about as a media buyer

00:52:53.000 --> 00:52:58.000
And I hate is when people turn off top-spending ads because

00:52:58.000 --> 00:53:13.000
If you have an ad that's your top spender and something changes on your website that makes performance get worse, which ad in your campaigns, which ad in your account is going to bear the scars of that

00:53:13.000 --> 00:53:25.000
decline in performance, your top-spending ad. So turning off your top spending ad is just punishing your best ads for something that's probably happening on your website. And I literally built this entire tool to help

00:53:25.000 --> 00:53:35.000
solve and prevent that problem. So you can see here, this is very small, and surely they're A-B testing this, for AG1 here. But

00:53:35.000 --> 00:53:49.000
You can see it literally went from their first price thing here, went from monthly delivery to 90-day supply. That is a huge change in terms of psychology, right? We're talking about a really big difference

00:53:49.000 --> 00:53:51.000
in what people

00:53:51.000 --> 00:54:06.000
how people are going to compute that, and how people are thinking about monthly versus 90 days, and, like, also looking at the price per month there, 79 versus 69. So there's… there's a little bit of different perception in price as well. Huge change

00:54:06.000 --> 00:54:21.000
Huge, huge, huge change, but also, in a lot of ways, a really tiny change. Depends on how you, like, think about it. And then looking at this Ridge example, they had the add to cart button at the bottom there versus removing it, on their collections page. I'm sure they were just testing that.

00:54:21.000 --> 00:54:29.000
And then, over here on the landing page, they're just changed again from the evergreen offer to their, Lamborghini sweepstakes.

00:54:29.000 --> 00:54:43.000
you know, at scale, like Shirley Ridge knows about this, their marketing team, advertising team is aware of this, right? So this wouldn't be a surprise, but still, having it documented well is extremely valuable. Here's an example from Ritual's homepage that keeps changing.

00:54:43.000 --> 00:54:45.000
And it's changing who it's for

00:54:45.000 --> 00:54:53.000
You can see, like, even, this one right here, the September 15th one, is a call-out for perimen… oops, a call-out for perimenopause.

00:54:53.000 --> 00:55:00.000
Which is very different than something for pregnant women or something different for all women.

00:55:00.000 --> 00:55:16.000
And that's the hero image and hero headline on their homepage. So if you're a younger woman who's going to ritual, you're getting an ad for ritual and then you go to their homepage, you're like, wait a second, I'm not in perimenopause. I'm

00:55:16.000 --> 00:55:20.000
I'm not in my 40s, I'm in my 20s, let's say. And

00:55:20.000 --> 00:55:31.000
like, you just… you… the homepage is that much less relevant to you. You're probably gonna really get out of here, because you're like, this isn't for me. If this woman on this page doesn't look like

00:55:31.000 --> 00:55:32.000
The audience

00:55:32.000 --> 00:55:42.000
Or doesn't… isn't relatable to the audience, or this offer free ritual water bottle? I don't… I don't know. Maybe that's great! Maybe people are like, yeah, give me that free ritual water bottle. I don't know.

00:55:42.000 --> 00:55:52.000
But my point is, yes, some of the stuff gets AB tested. Some of the stuff just gets changed because it's a campaign update, and some of the stuff is just changed because of some someone wants to change it, right?

00:55:52.000 --> 00:56:08.000
Let me see in chat if you're allowed to. If you're allowed to say, that you work for someone, or you are that someone who just makes changes willy-nilly, please write in the chat willy-nilly. Please. Because

00:56:08.000 --> 00:56:12.000
I think that's a common problem.

00:56:12.000 --> 00:56:17.000
Yeah, so let's look at another example here.

00:56:17.000 --> 00:56:30.000
We have a glossy example. We have another ritual example here where their sail changed. Again, like, you know, a lot of this is about sales changing, but these are just obvious examples. It's not always, it's not always as simple as that

00:56:30.000 --> 00:56:41.000
There's also, we had found, I don't have a screenshot of it here, sorry, but on Amazon, we had groom's pricing change. That's also something that we monitor and capture.

00:56:41.000 --> 00:56:50.000
So, here's something else that we're capturing is, search engine results. This was something really interesting that we found. So, for, like, nuts.com,

00:56:50.000 --> 00:57:03.000
Which is a completely, excuse me, nuts.com, unlike tushy.com, nuts.com, completely safe for work. You can go to that website, I encourage you to do it

00:57:03.000 --> 00:57:11.000
It would be funny if that one was also inappropriate, but Nuts.com totally safe. They sell very delicious nuts.

00:57:11.000 --> 00:57:30.000
But if you go to Google, best nuts online, you'll see that they were in that top spot for a very long time. And then suddenly something happened. I think they changed something about their like web server or something like that. I actually don't, I don't work with them, so I don't know

00:57:30.000 --> 00:57:36.000
I have worked with them in the past and they lost the top spot for that.

00:57:36.000 --> 00:57:48.000
So I thought this was really interesting. They lost the top spot. You can see this green line here. They dipped all the way down to here, and then they made it back up, but they have not taken over that number one top spot since then.

00:57:48.000 --> 00:58:03.000
And that's kind of crazy if you think about it, because that's going to impact your Facebook ads. That's going to impact your entire business, really. If people are trying to search for how to buy nuts online and now you're number two

00:58:03.000 --> 00:58:07.000
to some other brand. That's insane. So

00:58:07.000 --> 00:58:23.000
you know, because we're capturing and monitoring this every day, we know exactly the day it happened, and we can pinpoint our, you know, performance data or site data back to exactly when that changed. Does anyone else have a way that they could monitor this for their own brand, for their own site?

00:58:23.000 --> 00:58:31.000
Let me know. I'd be very curious. And I doubt it, but I'd be fired up if someone was. So if you want to build this for yourself

00:58:31.000 --> 00:58:43.000
absolutely do it. I'm gonna give you a prompt. I will absolutely, for free, right now, give you a Grokbot prompt, so you can go build this yourself. Because, why not?

00:58:43.000 --> 00:58:58.000
I want you to be able to see how valuable this is. I want you to be able to… it doesn't have to be Grokbot, by the way, you can use whatever AI you'd want. Who is the one that, Alex, remind me, who is it that spoke last week, I think

00:58:58.000 --> 00:59:00.000
That had a

00:59:00.000 --> 00:59:05.000
thing

00:59:05.000 --> 00:59:09.000
Where's my head going blank now?

00:59:09.000 --> 00:59:11.000
Sorry to put you on the spot. I'll come back to you.

00:59:11.000 --> 00:59:14.000
Great. Andre's welcome to Tuesday spoke last week. Manish. Manish spoke last week.

00:59:14.000 --> 00:59:16.000
Yeah, yeah, yeah, yeah. What was it?

00:59:16.000 --> 00:59:19.000
Yeah, Nation Drew from Skydive

00:59:19.000 --> 00:59:29.000
Yeah, skydive, exactly. So like skydive is a perfectly good example. Like, go use that. So let me give you a prompt here. I'll come back to it in a second when I pull it up. But

00:59:29.000 --> 00:59:40.000
Yeah, you can take this, go put it in there, and it will absolutely do it. I have it running right now on my Grokbot for a client that I work on, just to see what it does, and it does… it is absolutely better than nothing.

00:59:40.000 --> 00:59:52.000
It fundamentally gives me updates every day of like the things that change. It's often wrong, but that's okay. It's still better than nothing. So let me, let me, I'll come back to it in a second. I'll give, I'll give you that prompt in the chat here.

00:59:52.000 --> 01:00:09.000
And then, what I'd also tell you to do is go to urllovett.com and I'll pull that up in a second and have you guys go through the onboarding or not even the onboarding, just go through the site scan and you can see in our site scan what pages we'd recommend that you monitor

01:00:09.000 --> 01:00:15.000
So it's typically, like, home page, your top selling product pages

01:00:15.000 --> 01:00:26.000
category pages, about us, and then a few search results, some competitors, if you're on Amazon, your Amazon listings. Any other place where you're selling, we would recommend monitoring.

01:00:26.000 --> 01:00:33.000
So go capture any of those, go put those in with the prompt that I'm going to give you and then

01:00:33.000 --> 01:00:45.000
You know, just start monitoring that every day. If you have a lot of, that's only really going to work if you have a lot of AI tokens available first, because it takes up a lot to actually do that every day.

01:00:45.000 --> 01:00:55.000
And if you have a multiple clients, then it's going to take up even more. So I wouldn't really recommend it. But yeah, I,

01:00:55.000 --> 01:00:58.000
Give me one sec. Give me the prompt.

01:00:58.000 --> 01:01:04.000
You know, and make sure you have it run it daily if you're really lazy about it, run it weekly. That's fine. Have a summary run weekly.

01:01:04.000 --> 01:01:18.000
But here's the thing. If you're gonna be doing that yourself, you only have, you know, one computer, you have the bot, if you… if it fails, misses something, there's gonna be a gap in your record. That also assumes that your bot is able to get around,

01:01:18.000 --> 01:01:30.000
certain block scripts and walls that are up there. You might have some false alarms, and you're also gonna have, like, a folder of images on your computer if you build it properly. And then it also probably won't tell you like

01:01:30.000 --> 01:01:34.000
the severity, although you can probably train it to do better

01:01:34.000 --> 01:01:37.000
So here's what I also know about you

01:01:37.000 --> 01:01:42.000
Everyone watching this, probably maybe 90% of the people watching this

01:01:42.000 --> 01:01:44.000
You're ahead of the game on AI

01:01:44.000 --> 01:01:46.000
Most of you could build this yourselves

01:01:46.000 --> 01:01:59.000
Maybe not most of you, many of you can build this yourselves. But what I also know about you is that you have much bigger problems to solve. You have way bigger fish to fry than this niche problem.

01:01:59.000 --> 01:02:17.000
I'm also obsessed with this problem way more than you. So if there is anyone here who is more obsessed about screenshotting their website than I am, please hit me in the Q&A and let me know because I would love to chat with you and I would love for you to challenge me on that

01:02:17.000 --> 01:02:27.000
And yes, I think the Q&A. Oh, yeah, Alex, I saw said, yeah, this will be available. The Q&A

01:02:27.000 --> 01:02:43.000
So yeah, and then your time costs more. You know, yeah, you could go ahead and build this, but like even for you to like go through the prompting, go through managing this yourself, go through all the problem solving, everything involved in building this

01:02:43.000 --> 01:02:45.000
And troubleshooting it

01:02:45.000 --> 01:02:47.000
If your time

01:02:47.000 --> 01:02:54.000
is worth more than $50 an hour, then this is not it's not worth it for you to go build this yourself

01:02:54.000 --> 01:02:56.000
I've literally built

01:02:56.000 --> 01:02:57.000
URL, URL love it

01:02:57.000 --> 01:03:00.000
So that you can pay 50 bucks a month

01:03:00.000 --> 01:03:03.000
And we will handle all of this for you

01:03:03.000 --> 01:03:15.000
Because we get to work on this niche problem and absolutely just scale the shit out of it to make an amazing product so that you get the value from it

01:03:15.000 --> 01:03:22.000
Without having to think about it. Yeah, I'll give you the prompt right now. Sorry. Here you go

01:03:22.000 --> 01:03:23.000
Prompt

01:03:23.000 --> 01:03:29.000
Oh, it's too long. Alex, what's the best place for me to put this prompt? Because it is four times too long than I can

01:03:29.000 --> 01:03:40.000
If you send it to me, we've got, like, a Notion hub where we put everything, so guys, we've brought the resources in the notion hub, and we'll do a recap email tomorrow and send you guys there, so I'll make sure it's in there.

01:03:40.000 --> 01:03:43.000
Apologies, everyone. But yeah, it is

01:03:43.000 --> 01:03:51.000
It is real, I'm not, not like baiting you, I'm not making you have to, like, pay for anything or give me your email to get this thing.

01:03:51.000 --> 01:03:52.000
Please just go

01:03:52.000 --> 01:03:55.000
Yeah, you can get the prompt for just 49 bucks a month

01:03:55.000 --> 01:04:12.000
Yeah, that's what I'm getting, you guys. Sorry about that, everyone. But yeah, that's, and that's the other thing that I also know about this audience is that you can also afford $49 a month to have this handled for you. Now that's that is just for like one brand, like 15 captures a month. I'm sure you'll probably

01:04:12.000 --> 01:04:19.000
A lot of people probably want or need more, and if you have an agency, by the way, how many agency owners are up in here?

01:04:19.000 --> 01:04:32.000
Yeah, give me, like, drop the word agency in the chat, it would be helpful to know. If you're interested in getting onto your role of it, we actually do the onboarding for you. Yes, it is $49 for a screenshot app, but it's actually way more than that.

01:04:32.000 --> 01:04:37.000
Nice. Thanks for dropping the agencies in there, in there

01:04:37.000 --> 01:04:38.000
So

01:04:38.000 --> 01:04:54.000
Go check out EuroLovett.com. You can get your… you can try your first month for a dollar, if you hate it, okay? Let me know, and I will happily build more, build it more out. I'll give you some more months to try it out and let it go. But we have built and are continuing to build

01:04:54.000 --> 01:05:08.000
everything around screenshots and capturing your pages every day, so that you can not just have those, like, that's… yeah, I agree, like, $49 for that, why would I do that? No, it's to build your intelligence

01:05:08.000 --> 01:05:17.000
It's to build your understanding of what the heck is actually going on with your ad performance and business performance in a way that you never had before.

01:05:17.000 --> 01:05:25.000
It is a security blanket. It is a way to make you feel and understand

01:05:25.000 --> 01:05:42.000
Things about your ads that you've never understood before. So that's what I want to talk about. I would love to open up questions and talk about this more. I think there's plenty of other stuff I also forgot to cover here. So yeah, any questions, please drop them in here. And again.

01:05:42.000 --> 01:05:59.000
You saw a bunch of people called out that they work in agencies with the agency thing we offer, we will do the onboarding for you. Like, I don't know how much you guys hate onboarding onto SaaS. It sucks, I hate it. So we will handle, like, all of your clients onboarding

01:05:59.000 --> 01:06:10.000
We'll figure out all of the pages that you'd want to monitor for each of those, and we'll just set it up automatically for you, so you don't even have to think about it. So it's super easy, and day one, you start

01:06:10.000 --> 01:06:12.000
monitoring immediately

01:06:12.000 --> 01:06:22.000
And by the way, the other beauty of this is that this gets more valuable over time. The more and more you capture more screenshots, the more you're able to look back and understand your data

01:06:22.000 --> 01:06:31.000
I'm able to look back at like March when my client asked me, hey, why is performance, you know, why was performance like this? Why was conversion rate this

01:06:31.000 --> 01:06:38.000
Back in March and I can go back to the site and look at like, oh, well, that's when we changed this on the site

01:06:38.000 --> 01:06:48.000
Speaking of, we haven't built it yet, but we're building the MCP so that you can just ask your AI to tap into your love it to pull that for you so that we can have that.

01:06:48.000 --> 01:06:58.000
We are building anything that can help you to understand everything about the history of your business, your client's business

01:06:58.000 --> 01:07:02.000
In a way that's never existed before. And by the way, there are plenty of other screenshot apps

01:07:02.000 --> 01:07:19.000
that are out there. I encourage you to check them out. Visualping is a great one. Distill.io is a great one. All of these things exist, and none of them are catered to actual marketers or business owners. There's almost all catered to developers. I've built something that makes it easy for marketers

01:07:19.000 --> 01:07:26.000
to just kind of set it and forget it, and then get the information that they need, that you need

01:07:26.000 --> 01:07:41.000
In order to operate better and faster without having to, like, manually set up every single individual page. We literally let you connect your meta ads so that we can monitor automatically any new landing page you start running ads to. So you don't have to

01:07:41.000 --> 01:07:50.000
Every other tool you'd work with, you'd have to be like, oh yeah, we're running a new ad, let's go add it to our screenshot capturing tool.

01:07:50.000 --> 01:07:58.000
So we have the AI built in. We have, what's the other thing we have built in? We can get around most

01:07:58.000 --> 01:08:17.000
Websites that try and block bots, but you can get around most of them. Like 99.5% success rate, and you don't have to pay extra for that. That's built in. So there is a ton that we are building here that makes it so that you don't have to solve any of the problems that we have to solve every day

01:08:17.000 --> 01:08:28.000
about getting screenshots, analyzing them, and reporting on them and matching them up. We are building that because it is a huge actual logistical nightmare to solve.

01:08:28.000 --> 01:08:38.000
So yeah, happy to open up to any questions anyone might have here. If anyone's curious about what this is or why they should be using it.

01:08:38.000 --> 01:08:41.000
Yeah, just to say a bit more on

01:08:41.000 --> 01:08:42.000
Oh, sorry, yeah.

01:08:42.000 --> 01:08:59.000
the the the comment there is like, yeah, it is 50 bucks for a screenshot app, but it's just… it's 50 bucks for… for you not to have to stress about what's changing… causing the change in performance, and I've literally seen Barry spend hours

01:08:59.000 --> 01:09:12.000
doing this process manually before he built this. Like, I've been in his office and watched him be in the ad account and watched him look at the analytics on the site, and try and do this stuff, like, by comparing two different tabs.

01:09:12.000 --> 01:09:22.000
So he's built for the pain point that he had, and we use it at Create, and it's just so useful to be able to go and see, okay, performance change

01:09:22.000 --> 01:09:34.000
Why that is that because, oh, we made this huge change on the site. That might have saved me 30 minutes of investigation. Is that worth 50 bucks to do that, you know, 5 to 10 times a month per brand? Absolutely it is.

01:09:34.000 --> 01:09:46.000
Yeah, I mean, the amount of, I mean, there is not a week that goes by for my clients and my work that we don't catch something significant. One of the biggest ones recently was like

01:09:46.000 --> 01:09:58.000
The, like, part of the reviews section of our PDPs, all PDPs for one of my clients, was just completely missing images and formatting, and the stars were all missing.

01:09:58.000 --> 01:10:13.000
So like imagine you're trying to sell a supplement and like the thing that people are going to to that needs the most trust that, you know, people are going there to read testimonials and they're like, they're like, wait a second, I don't can't trust this website

01:10:13.000 --> 01:10:30.000
This is probably a scam website if they can't, like, even get their images to show properly. They don't even show the stars, like, there's, like, text missing. So it erodes trust. And we literally could see that in our conversion rates, in our CPAs for that period, and we were able to catch it because of

01:10:30.000 --> 01:10:32.000
this tool. I don't know

01:10:32.000 --> 01:10:45.000
how any of you could be catching that. I literally don't understand. So when I think about $50, by the way, the $50 is intro pricing for pre-launch. This isn't even fully launched, but we're going to be charging way more later.

01:10:45.000 --> 01:10:57.000
You get in now, you get to keep this pricing. The first 100 people or the 60-something we have spots we left, get to keep this pricing into the future when we increase pricing later.

01:10:57.000 --> 01:10:59.000
That's the crazy thing to me is like

01:10:59.000 --> 01:11:16.000
That's 50 bucks a month to cover probably tens of thousands of dollars in problems for that one problem. That's $50 a month, which is cheaper than having a VA do this every day. It's cheaper than and easier than having… setting up your own AI and monitoring your own AI to do this every day.

01:11:16.000 --> 01:11:32.000
So that's why we're building it. And I also hope to be able to continue with economies of scale. I hope to potentially make it cheaper in the future, make it more accessible, make it more scalable. But we're also building more features to make it more valuable

01:11:32.000 --> 01:11:34.000
We're all, like, one example

01:11:34.000 --> 01:11:39.000
That we have is because we're scanning your entire website every day, we're not just monitoring

01:11:39.000 --> 01:11:54.000
what's changing on your website. We literally can know every plugin that you use. So think about every Shopify plugin that you use, like, let's say Klaviyo, right? And we are monitoring Klaviyo's change logs. We are monitoring Klaviyo's outages.

01:11:54.000 --> 01:12:05.000
So that we can also report on that and help you better understand what is happening with those things that is impacting your users, that's impacting your business, that's impacting your ad performance.

01:12:05.000 --> 01:12:09.000
If you have that already, cool. I guarantee you, you don't

01:12:09.000 --> 01:12:19.000
And that's what we're building. Again, for this overall business intelligence at a level that nobody's had before.

01:12:19.000 --> 01:12:22.000
Sorry, I'm just fired up. I love this stuff.

01:12:22.000 --> 01:12:41.000
How's it going? Guys, put your questions in the chat, put your questions in the Q&A. By the way, I know we didn't get to stop at the hour, but like anyone who does have to drop soon, thank you so much and put messages in the chat. It's been an honor to host you this course, and we've loved every second of it, so we really, really appreciate you. Really appreciate the love as well. Everyone's sharing the chat. It's, it's really cool to see

01:12:41.000 --> 01:12:57.000
People saying that this is a company that's free, I think. David said, thank you, I'm incredibly ignorant yet enthusiastic. This course has been eye-opening. I appreciate the self-awareness there, David. Just so much

01:12:57.000 --> 01:13:12.000
Gratitude from Jimmy and I've been able to spend these six weeks with you guys and all the resources, all of the transcripts are going to be put on YouTube, put in the notion hub and put on GitHub very shortly. It's hard to believe it's the last one already and it's going so quickly

01:13:12.000 --> 01:13:22.000
Barry, Andy asked in the Q&A, because you were showing some of the examples, were mobile, do you always prioritize mobile design over desktop

01:13:22.000 --> 01:13:27.000
Yeah, yeah. Actually, we are. It's all completely built mobile first. You can

01:13:27.000 --> 01:13:35.000
capture screenshots of your desktop, but this is prime was primarily built for

01:13:35.000 --> 01:13:42.000
like, a lot of the stuff that I'm working on, which is 85 to 95% mobile traffic

01:13:42.000 --> 01:13:46.000
So that's what we've prioritized, and most of the time,

01:13:46.000 --> 01:13:54.000
It's, you know, easier to monitor for that, but yeah, you can absolutely monitor desktop as well. It just defaults to mobile, because that's where most traffic is.

01:13:54.000 --> 01:14:08.000
Have a look at this in the chat, Barry. Have you thought about being able to have a community built out like this? Like have a Discord or a Slack we could all join with you and just have us do this regularly going forward.

01:14:08.000 --> 01:14:13.000
Which part of this

01:14:13.000 --> 01:14:22.000
Yeah, Joyce, yeah, let us know which part of this you're referring to. Like this course or talking about, oh yeah

01:14:22.000 --> 01:14:28.000
Yeah, that's a good point. I think that's a great point. I think it's, I don't know, Alex, what should we do?

01:14:28.000 --> 01:14:45.000
I mean, if that's something that you guys would want, you know, we can do that. Like, I mean, we wouldn't… we wouldn't continue to do it for free if it was an ongoing basis. But I mean, I love these sessions. I love doing things live with you guys, and I just love sharing what

01:14:45.000 --> 01:15:05.000
What we're building and just jamming with people, and we get to have people like Barry on do this together. I learn a lot, too. So if that's something that people have appetite for, if you'd want these to be regular, if you want to be on here regularly with with me, you know, Jimmy, Barry, and some of the people who we've had like in these sessions over the last 6 weeks, and like

01:15:05.000 --> 01:15:09.000
Let me know, and I can… we can start something, for sure.

01:15:09.000 --> 01:15:21.000
Nice to see a vote for Slack over Discord. I'm team slack also. But yeah, I would love to do that as well. I think top secretly with something Alex and I have definitely been talking about doing

01:15:21.000 --> 01:15:34.000
So yeah, it's good to know there's some demand for that. I think it's definitely worthwhile. I think we love sharing this stuff and we love researching this stuff and finding the stuff and then curating it. So yeah, good to know. I'm honored, by the way.

01:15:34.000 --> 01:15:42.000
Can I make tea? Can I be cheeky, guys? Because I know you guys are the OGs. If you stay around for the second hour, I feel like I can ask you this question

01:15:42.000 --> 01:15:51.000
If we were to do that, like, if me embarrassed someone, I'm like, what would you pay for it

01:15:51.000 --> 01:15:52.000
Ilano

01:15:52.000 --> 01:15:53.000
Probably 10 million, 10 million a month

01:15:53.000 --> 01:15:57.000
You guys just give away everything for free.

01:15:57.000 --> 01:16:00.000
Yeah, right. Nice.

01:16:00.000 --> 01:16:08.000
I don't know, we could, we could do it. We could set it up

01:16:08.000 --> 01:16:12.000
Oh, there's a good question. Hold on a sec.

01:16:12.000 --> 01:16:21.000
From Tristan. Okay, cool question here. Talk about, people falsely diagnosing ads, shortcomings due to changes to the website.

01:16:21.000 --> 01:16:26.000
What's my idea? What's your ideology on the nature of homepages versus landing pages? Should your homepage

01:16:26.000 --> 01:16:30.000
Should always feel generic to avoid pitfalls and change in creative

01:16:30.000 --> 01:16:36.000
I don't have a great answer for it, right? There is no right answer to it, because sometimes you have to run

01:16:36.000 --> 01:16:39.000
campaigns, you have to launch new products, you have to expand

01:16:39.000 --> 01:16:51.000
And you have to, like, let people know that. And people, some, you know, some people are gonna skip by that, and some people aren't. You just, I guess all my point about talking about this is to make people aware of it, make people mindful of it

01:16:51.000 --> 01:16:53.000
make people think about it

01:16:53.000 --> 01:16:55.000
So that

01:16:55.000 --> 01:17:02.000
When performance does change inevitably, when, when things do maybe go wrong, that they understand why.

01:17:02.000 --> 01:17:18.000
That's all I really care about is that understanding of why, whereas so many people, like, either throw their hands up in the air and just go like, I don't know, or they're like, they're blaming some other cause, right? Or they're blaming, like, the macroeconomics, or they're blaming some other thing, but

01:17:18.000 --> 01:17:23.000
You know, I just want people to be able to understand the truth and understand why.

01:17:23.000 --> 01:17:31.000
Because sometimes you kind of also have to do those things. You have to update the homepage to have a different offer sometimes. So

01:17:31.000 --> 01:17:34.000
Yeah, I think

01:17:34.000 --> 01:17:44.000
I think that's a great question and it's a common problem that I have working with brands where they have a new product, a feature. I'm like, well, you're going to

01:17:44.000 --> 01:17:50.000
feature a product that like are relevant to 2% of our current audience

01:17:50.000 --> 01:18:00.000
you know, that we're advertising to. But, you know, then it changes over time as we start advertising to that new audience more, as we start advertising that new product more and it starts to shift and change.

01:18:00.000 --> 01:18:02.000
So, it's difficult.

01:18:02.000 --> 01:18:09.000
But great question, and a really, again, important to think about, and that's why we capture these screenshots, to be able to monitor

01:18:09.000 --> 01:18:24.000
how that changed… when that change started over time. Just like we were able to see that chart for Nuts.com, where they lost the number one spot, you'd be able to pinpoint, where in your, like, Shopify performance, GA4 performance, Facebook ads performance, that change occurred

01:18:24.000 --> 01:18:26.000
To be able to,

01:18:26.000 --> 01:18:32.000
understand, make, make sense of that

01:18:32.000 --> 01:18:35.000
I saw a question for Mark here.

01:18:35.000 --> 01:18:43.000
When we say performance, you're mainly looking at overall ad and MTA and channel MTA? Are you looking at funnel step conversion as well? I'm looking at a lot of things.

01:18:43.000 --> 01:18:54.000
I'm, you know, I'm talking about a lot of it is like in platform data, but it's also like, you know, in Shopify data, right? Like if I'm seeing a bad day on

01:18:54.000 --> 01:19:00.000
Facebook ads? Am I also seeing a bad day relatively, on Shopify as well?

01:19:00.000 --> 01:19:02.000
You know, I'm looking for different

01:19:02.000 --> 01:19:17.000
different markers of performance anytime performance is bad in one of those, I'm looking at the other ones to try to make sense of what's going on. And that's why, again, I've built this tool. That's why, like I saw, I'm solving this problem is because

01:19:17.000 --> 01:19:22.000
I have seen so many times where it's literally like

01:19:22.000 --> 01:19:38.000
These changes in add to cart, these changes in checkout rate, these changes are happening because of small copy changes, small button placement changes, small changes to like images that are on sites. I can't answer exactly like, oh, this image changed

01:19:38.000 --> 01:19:44.000
Therefore, it's less relevant to these people, or more relevant to these people. I can't answer that perfectly.

01:19:44.000 --> 01:19:46.000
But what I can answer is

01:19:46.000 --> 01:19:51.000
When that change was made, it had an impact on performance. And here's how

01:19:51.000 --> 01:19:55.000
And that's what I'm trying to build here to help more people see that more clearly.

01:19:55.000 --> 01:19:59.000
And hopefully via lots of forms of data. Again, you'll love it.

01:19:59.000 --> 01:20:16.000
types into we're not fully piped for Shopify yet, but we're connecting to GA4 and meta ads directly and Shopify pretty soon.

01:20:16.000 --> 01:20:17.000
Yeah, so.

01:20:17.000 --> 01:20:25.000
All right, cool. There's a lot of chats about the community, Barry, the idea. I love you guys and I love doing these sessions. If I'm being completely honest, it would probably be at a higher price point than 10 to 20 bucks a month.

01:20:25.000 --> 01:20:35.000
But, you know, we could, we could wipe something out, and especially, like, whatever the rate is that we… that we would do it for, we would make sure that you guys, of course, get a discount, for

01:20:35.000 --> 01:20:42.000
or being the homies and Sam throughout the whole, the whole six weeks, for this course

01:20:42.000 --> 01:20:43.000
For sure.

01:20:43.000 --> 01:20:59.000
Okie doke. Questions from my part of the session? There's a couple that I want to get through. What tools would you use to actually publish these pages online? So anything that I use that I build inside of Claw Code, I publish on Cloudflare

01:20:59.000 --> 01:21:01.000
Pages

01:21:01.000 --> 01:21:13.000
I mean, you could use GitHub or Vercel and I don't really like I don't have the arguments for or against the cloudfly works for me. So that's why I deploy on.

01:21:13.000 --> 01:21:29.000
What else? I would love to hear how you build loops for each workflow. I actually don't have loops built into that workflow that I showed. I just build landing pages when I want to build landing pages. There's no loops actually built into that skill.

01:21:29.000 --> 01:21:45.000
Well, I guess you could, you could put like loops for feedback, but it's just like I have a new landing page, I want to make this landing page for this persona. I pick a template, it goes and builds it, and then I'll give it feedback in the chat. It's like, it's quite a simple skill. You could probably build something a lot more complex and probably better than what I've got

01:21:45.000 --> 01:21:51.000
But it works for me. So, no actual loops inside of the

01:21:51.000 --> 01:21:55.000
So the thing itself.

01:21:55.000 --> 01:22:02.000
conversion tracking for A B tests for landing pages

01:22:02.000 --> 01:22:09.000
That's not something that URL ever does yet, Barry, is it? Conversion tracking? Is that something that is of interest to you guys?

01:22:09.000 --> 01:22:21.000
So A/B test is a challenge right now for anyone capturing screenshots on any website anywhere, right? We can't monitor for that. We're thinking about how to

01:22:21.000 --> 01:22:30.000
better account for that by, like, literally connecting either via API or MCP or whatever to things like IntelliGems. It's on the roadmap, we're trying to figure it out

01:22:30.000 --> 01:22:40.000
But like, it's easy enough to know when you are AB testing something because it just kind of wavers between the two for that time. So

01:22:40.000 --> 01:22:49.000
We're, we're building around it. It's a great question. It is a legitimate problem, but it's a problem with this no matter how you do it.

01:22:49.000 --> 01:22:52.000
I need a link

01:22:52.000 --> 01:22:53.000
There we go

01:22:53.000 --> 01:23:15.000
Clay's got my offer stack filled out there. You're on to me, Clay. Free content on YouTube and course. Community and then upsell to Parker. Well, that could be what happens. We'll see. Did we put Pat was asking about the, yeah, URL. Love it. URL. We've got that there. I'm going to have to go in a second, guys. Is there any questions you really want us to ask

01:23:15.000 --> 01:23:24.000
get them asked now

01:23:24.000 --> 01:23:39.000
Yeah, drop your LinkedIn if you want to stay connected. I mean, we'll send an email out with, I don't know, I think given that you guys have a lot of interest in it, we'll probably do some form of community, like whatever, however it is structured. Definitely want to stay connected with especially you guys have stayed on right to the end. So

01:23:39.000 --> 01:23:53.000
Yeah, we'll do something. If you want to drop your LinkedIn or your Twitters or anything, love to follow you guys and see what you're building. Stay connected. Juano

01:23:53.000 --> 01:23:58.000
Anything else you want to cover, Barry?

01:23:58.000 --> 01:24:01.000
No, just

01:24:01.000 --> 01:24:12.000
You know, just a reminder for everyone to go to your 11url love it.com. Do a scan of your site, see what pages we recommend monitoring

01:24:12.000 --> 01:24:16.000
Go, we'll send, we'll send through the prompt so you can go monitor it yourself

01:24:16.000 --> 01:24:32.000
without paying us anything, and then if that's not sufficient for you, then I would strongly recommend you come on either Uralovett.com or go use something else to capture screenshots. But definitely want you to cover your butts. Like, there's a whole… you're… if you're not monitoring this stuff

01:24:32.000 --> 01:24:43.000
If you are running ads or not running ads, if you are doing anything else in this, and you're not currently monitoring these changes over time, even if you don't make changes every day, which you're not

01:24:43.000 --> 01:24:49.000
It's so helpful for me to see when I see like a wall of screenshots. I should have shown that earlier

01:24:49.000 --> 01:24:55.000
a wall of screenshots where they don't vary at all. I meant to show this. Sorry, can I show something really quick

01:24:55.000 --> 01:24:59.000
Correct.

01:24:59.000 --> 01:25:01.000
I think this one

01:25:01.000 --> 01:25:04.000
Like we have this

01:25:04.000 --> 01:25:05.000
You see this?

01:25:05.000 --> 01:25:06.000
Yep.

01:25:06.000 --> 01:25:10.000
Okay, so

01:25:10.000 --> 01:25:17.000
So here's like a wall of just the calendar for September, right? For the, they're all gifts page for nuts.com, right?

01:25:17.000 --> 01:25:31.000
And you'd think there's, like, nothing crazy would change here, right? You can kind of see it's all the same, but like, if we keep going, scrolling through the history, you're going to notice

01:25:31.000 --> 01:25:39.000
Should have queued it up a different one. Hold on. Oh, there you go. Right here. Literally the sort and the products that they're featuring change

01:25:39.000 --> 01:25:42.000
And all of this

01:25:42.000 --> 01:25:48.000
whether it's price, whether it's relevance, has an impact on your business. I also

01:25:48.000 --> 01:25:53.000
Oh, sorry, can you see this or no?

01:25:53.000 --> 01:25:54.000
Oh, really? Oh, sorry.

01:25:54.000 --> 01:26:01.000
Yep. Oh, moving your slides again. Oh, no. You can see you're all of it. Sorry, I was in the wrong window

01:26:01.000 --> 01:26:02.000
We can see

01:26:02.000 --> 01:26:08.000
You're on the URLs page for Barry Hot. Yeah.

01:26:08.000 --> 01:26:10.000
But you see the nuts.com screenshots here? Sorry

01:26:10.000 --> 01:26:11.000
Yeah, yeah, I can

01:26:11.000 --> 01:26:14.000
Okay, my bad.

01:26:14.000 --> 01:26:17.000
But you can see here, literally, like, the difference

01:26:17.000 --> 01:26:27.000
I know it's minor. I'll make it larger there. But you can see it had like the red hot gift basket and then the caramel and pumpkin spice delight changed from the September 15th to September 16th

01:26:27.000 --> 01:26:37.000
like, you might think, like, oh, that's so minor, Barry, why do I give a ? If you're nuts.com, or if you're the person who's running ads for Nuts.com, and people are shopping on your website

01:26:37.000 --> 01:26:57.000
The difference in price between these is significant. Literally, the third and fourth product here, look at it, it goes from 99 to 55, 99 to 59 and 39. That's just, they're totally different products, totally different things. Like, so your AOV is going to go down, your ROAS might go down, or maybe those are more relevant. So your performance goes up

01:26:57.000 --> 01:27:06.000
People don't understand how much stuff like this has an impact. So if you have a large catalog and your like best sellers changes

01:27:06.000 --> 01:27:22.000
where you're changing your featured products just a little bit, or some dynamic tool is doing that over time, stuff like this is killing you. Or, it's actually helping your performance, and you don't know it, and you're attributing it to some other stuff, or you're patting yourself on the back like you're the golden god

01:27:22.000 --> 01:27:37.000
of advertising when it's actually just something else is, you know, a tailwind there. So that's what I just wanted to show real quick, is, like, these are the kinds of things that you can both see and have AI monitor and be able to look back at. So you have a historical log

01:27:37.000 --> 01:27:39.000
So you can know

01:27:39.000 --> 01:27:51.000
What these things looked like, even these small little things that you think don't really matter, but actually really fundamentally matter to your business. So I hope that's a helpful explanation there that I forgot to show earlier.

01:27:51.000 --> 01:28:13.000
That is very useful to see that inside of how it works. Andrew asked, are you able to publish to Cloudflare automatically from Claude? Yep, they have an MCP. You can do that. And the question about my Google Doc notes in Parker, please. How are you using notes in your brand brain? I'm using Google Docs for mine so they are not stored locally or linked to the project directly.

01:28:13.000 --> 01:28:28.000
No, I don't do Google Docs for anything. All of my notes, everything is markdown files. I try and do markdown files as much as possible. It's just easy for agents to read. I know it's easy for humans to read Google Docs and things like that, but like

01:28:28.000 --> 01:28:44.000
If you really need to access it, then you can just ask Claude what's what's in my brand brain, but no, everything in the brain is stored locally on Markdown files, and then is shared across the team in the Parker desktop app that we showed a few weeks ago.

01:28:44.000 --> 01:29:14.000
Where you can see… you can literally see the Parker brain here where people update it, like, in real time. So this is how we have, everyone making sure that they have the same context. So everything's done through that folder, and nothing is done outside of it. And if you're bringing in things from outside, then, like, you know, briefs, for example, they stay in Notion. We pull in slack frame ad account data, all that stuff comes in and is stored in that brain then shared across the organization. So everyone's working on the same context

01:29:14.000 --> 01:29:28.000
Hope that answers it. All right, guys, I'm gonna have to run. Sorry I didn't get to all the questions. If you still have questions that I didn't manage to get to, DM me on Twitter. I will try my best to get back to the remaining ones, or email me.

01:29:28.000 --> 01:29:35.000
at adcrate.co. Thank you so much.

01:29:35.000 --> 01:29:37.000
Thank you, Alex.

01:29:37.000 --> 01:29:38.000
Thank you.

01:29:38.000 --> 01:29:58.000
Really appreciate you guys, it was an honor. Thank you, Barry, for jumping on, showing us your a bit. Would highly recommend going to You AllLoveIt.com a dollar to try it is an absolute steal. Now, you can, for a total of $1, trial Parker for free to make your ads, and you can trial you all love it to monitor your landing pages and performance. That is, we've just given you pretty much a

01:29:58.000 --> 01:29:59.000
It's insane.

01:29:59.000 --> 01:30:00.000
tech stack for a dollar. So if you don't take us up on that, then I don't know what you're doing

01:30:00.000 --> 01:30:03.000
Yeah, really. Same

01:30:03.000 --> 01:30:04.000
All right, guys, we'll see you soon.

01:30:04.000 --> 01:30:09.000
This has been an incredible course. Thank you so much, Alex.

01:30:09.000 --> 01:30:10.000
Of course.

01:30:10.000 --> 01:30:14.000
Thank you, guys. Shout out to Jimmy as well. He's not on here today. Thanks. Have a wonderful rest of your Thursday and we'll see you very soon.

01:30:14.000 --> 01:30:15.000
Thanks. Doodles.

01:30:15.000 --> 01:30:21.000
All right.

```

