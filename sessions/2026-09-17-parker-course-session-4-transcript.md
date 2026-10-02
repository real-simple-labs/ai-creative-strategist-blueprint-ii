---
title: "Parker course — Week 4 transcript"
date: 2026-09-17
session: "Week 4 — Static ads in code"
source_type: "Google Drive VTT transcript"
source_file_id: "1j3dPTB0XMZw_I-UOsUqhwFGlScQg3HKN"
source_file_name: "transcript.cc.vtt"
source_url: "https://drive.google.com/file/d/1j3dPTB0XMZw_I-UOsUqhwFGlScQg3HKN/view?usp=drive_link"
source_modified_at: "2026-09-21T14:31:53.452Z"
---

# Parker course — Week 4 transcript

Verbatim caption export from the September 17, 2026 Parker course session. Captioning errors and timing are preserved.

```vtt
WEBVTT

00:00:05.000 --> 00:00:08.000
What's up, peeps?

00:00:08.000 --> 00:00:16.000
How are we doing?

00:00:16.000 --> 00:00:20.000
Welcome, one, and welcome all to learn about

00:00:20.000 --> 00:00:29.000
Static ads in code. Oh, this is going to be a good one. This is going to be a good one. I've had a lot of you messaged me saying that this is the session you're looking forward

00:00:29.000 --> 00:00:31.000
And

00:00:31.000 --> 00:00:39.000
I hope I can make it valuable for you. I think Jimmy should be jumping on shortly. But

00:00:39.000 --> 00:01:00.000
We will give it 30 seconds or so, and then we will get started. I don't know if anyone's on the session on Tuesday with Jacob, which is a really good session, if you haven't checked it, you should go and watch the recording. I've been playing around with Astra in Codex, for video editing, and it's getting good, guys. Like, I really don't think we're far away at all from

00:01:00.000 --> 00:01:15.000
being able to agentically edit videos, which is really exciting, and something that we've been doing internally that I would recommend you guys start to do is, start getting your editors to commentate over their edits, and say, like

00:01:15.000 --> 00:01:34.000
I'm making this cut because of this, or I'm making this pacing, or this selection of B-roll because of this. Because then what you're going to do is you're going to take that transcript and you're going to put it in to an agent like Codex, and that's going to help you edit agentically, because these tools are going to get better and better and better. I literally had a video the other day that I put in a raw

00:01:34.000 --> 00:01:37.000
Fourth piece of footage, 5 minutes long

00:01:37.000 --> 00:01:55.000
One shot, it returned me, like, a perfectly cut-down, unedited video, which, that alone saved my editors, like, you know, 30, 45 minutes. And then I go and put the edit on it, and sometimes it's… sometimes it's, you know, solid, sometimes it's a little bit shaky still, but we also haven't replied the right context to it yet. So, anyway

00:01:55.000 --> 00:02:03.000
That's not the topic of today's session. Today's session is about static ads, and we are

00:02:03.000 --> 00:02:23.000
gonna go deep. For the last three sessions of this course, is going to be mainly me hosting them, and Jimmy's going to be filling in where he can. I'm just going to share screen inside of Claude Code and Codex, build ads, show you my systems, answer the questions that you guys have got, and I'm going to try and be as open of a book as I possibly can. So.

00:02:23.000 --> 00:02:36.000
Please put your questions in the Q&A as I go through this. I imagine we'll have quite a few questions from today because I'm just going to be showing my entire workflow. So if you're newer to AI statics.

00:02:36.000 --> 00:02:54.000
And doing the magentically, then it might be a little bit overwhelming, but again, I'm not saying this is the way to do AI just that the process that I have built, and I'm trying to present it in a way that I believe is easy for everyone to take from the end of this call and start making a lot of good static ads inside of

00:02:54.000 --> 00:03:07.000
Claude code. And yes, it will be applicable without the Parker MCP. Now, the Parker MCP is going to make this a lot easier, but you don't have to have Parker to be able to execute on what we're going to be talking about today.

00:03:07.000 --> 00:03:15.000
Let's go straight in and share

00:03:15.000 --> 00:03:19.000
Okay.

00:03:19.000 --> 00:03:28.000
Here we go. Oops, don't want to share slack. That's go stop. Okay, so what I'm going to be going through today is the framework

00:03:28.000 --> 00:03:43.000
That we use internally to put out tons of statics for our clients. I've shared this, you know, I shared this in the first week, but, like, you're gonna be able to come out of today with a board like this, or the knowledge on how to create a board like this

00:03:43.000 --> 00:04:00.000
Where all of these ads are generated with AI through the Hicksfield MCP inside of Claude Code or Codex. This was literally me the other day playing with some things for Winx, for Black Friday, because Black Friday is coming up, so I thought, what if I could build a Black Friday skill

00:04:00.000 --> 00:04:15.000
That could pump out a ton of ads for Winx to run over holidays and all of our clients run over the holidays. I thought, you know, these are pretty, pretty solid. And again, all of these are made with my skill. And again, I could show a bunch of these different boards, but like, you know.

00:04:15.000 --> 00:04:32.000
Are all of these statics absolutely perfect? No. Some of these will not end up launching inside the ad account, but many of them we will. So, I'm going to show you how to do all of that today, and as you can see here in Connor's tweet, this is actually from March, this is using the same framework that we're going to be going through today.

00:04:32.000 --> 00:04:34.000
Connor is the founder of the Essence Vault

00:04:34.000 --> 00:04:53.000
a 9 pickup brand, I think, at this point, and they use this exact framework to launch 3K ads in 7 days, not slop perfect imagery in his words. And I would put a lot of weight on his words, because they are very, very good at

00:04:53.000 --> 00:05:01.000
And this was in March, so it's even better now, and it's a lot more agentic now, so I'm super excited to get into this session.

00:05:01.000 --> 00:05:04.000
I'm just gonna make sure I've got the chat up

00:05:04.000 --> 00:05:08.000
Okay, perfect.

00:05:08.000 --> 00:05:12.000
Okay dokie. Let's get cracking.

00:05:12.000 --> 00:05:17.000
So a couple of things here

00:05:17.000 --> 00:05:35.000
housekeeping things that I've covered, covered those. Yeah, questions in the chat, or Q&A, I will try and get through as many as I can. I'm gonna stay on for another hour. I think Jimmy should be joining shortly. If not, I'm just gonna take the whole session. And yeah, I'm gonna be sharing completed chats inside of Claude today

00:05:35.000 --> 00:05:52.000
I would have loved to show, like, me building it live, but it's just gonna take too long. Like, it's gonna take 10 minutes in between each prompt, you know, we don't have the time for that. So, I'm gonna show completed chats, but I will show you the exact prompts that I would use, to go and build this yourself. And I'm also going to give away the skills that I showed today. Like, everything that you see in this session

00:05:52.000 --> 00:06:06.000
is going to be given away. So you can take my skill and run it for yourself if you want. I'd rather you go and build your own one, but, like, if you just want to run my skill, then you can run that, and you can get ads like the ones that we just saw

00:06:06.000 --> 00:06:17.000
And again, this is my process. This is probably not the optimal process. Definitely not the only way you can make static ads inside of Claude Code. But it works for me. So I hope you get something from us.

00:06:17.000 --> 00:06:22.000
Okay, this one I want to start with

00:06:22.000 --> 00:06:33.000
I want to start with, I'm actually going to also finish on this, but I want to start with this

00:06:33.000 --> 00:06:37.000
This graphic here that I made. Now

00:06:37.000 --> 00:06:54.000
I've framed as like six tips, but we're going to come back to this and talk about the tips. I actually want to talk about like philosophies for building static ads because I have a certain way of doing things and it might be different to the way that you've seen it online.

00:06:54.000 --> 00:06:57.000
So

00:06:57.000 --> 00:07:14.000
First of all, what I want to like the way this is built is we are going to be building a template library, basically a swipe file of ads for us to look up against and then recreate the ads off of. This is the same concept that we

00:07:14.000 --> 00:07:29.000
used in an earlier session where we briefly covered this swipe file, and I'm going to go into this because this is actually from the video that I made a few months ago on this precord code. And we're going to basically build a swipe file together, and then we're going to use that swipe file to build out

00:07:29.000 --> 00:07:51.000
ads that just basically use these templates and apply it for our brand. So we're building it based on the template. What I want to make very clear is that the quality of the templates that we choose here is going to dictate generally the quality of the outputs that you're going to get. If you choose bad static ad templates to recreate, then you're going to get bad outputs

00:07:51.000 --> 00:08:12.000
Generally. A big philosophy of mine, especially if you've never built a static ad workflow before, is do not try to fully automate this from the jump. Please do not do that, because you're going to drive yourself insane going back and forth on Claude trying to make a perfect skill that gives you like a backslash statics, and it's going to automatically turn it into a PDF of 100 statics

00:08:12.000 --> 00:08:20.000
You can get there. It's very, very possible, but I would encourage you, if you've never built a static skill in Claude Code or Codex before.

00:08:20.000 --> 00:08:40.000
And please try and keep the human in the loop. And you're going to see my process shortly. I will show you where the human is in the loop. I approve copy, I approve the ads, and I prefer to do it that way because it increases the consistency of output and it gives me more control. Takes a little bit longer, but like I would highly, highly recommend

00:08:40.000 --> 00:08:50.000
Not trying to make this perfect from the jump, because you can always improve it. If you try and go for a perfect workflow, you're going to take ages, and you're going to be frustrated.

00:08:50.000 --> 00:09:07.000
Yeah, that's kind of tip three as well. And then feedback. We're going to build this in a way where we can give feedback to the skill, and it gets better and better and better. So it should be a lot better in two weeks time for you to use than it is today, which is why, again, we're not trying to make it perfect. We're just trying to make

00:09:07.000 --> 00:09:14.000
system that puts out static ads, uses the human in the loop, takes feedback and improves over time.

00:09:14.000 --> 00:09:21.000
Welcome back to this page later on, but this is just like how to think about going about building this

00:09:21.000 --> 00:09:25.000
This skill. Now

00:09:25.000 --> 00:09:37.000
I just want to take a break for a quick second because Jimmy's in the chat saying, can you pull me up? I actually don't know how to do that. I'm sorry, Melody, if you can try and help with that, then please do. I don't have the time to do that now.

00:09:37.000 --> 00:09:39.000
Okay

00:09:39.000 --> 00:09:41.000
So

00:09:41.000 --> 00:09:51.000
The way we're going to be generating this, starting from ground zero, the way that we're going to be generating ads inside of Claude Code is

00:09:51.000 --> 00:10:03.000
Using the Hicksfield MCP. Now, Hicksfield, for those of you who don't know, is basically a model aggregator. They are a site that allows you to generate static ads

00:10:03.000 --> 00:10:20.000
Through different models that you want to choose. So this is the Hicksfield web app. If I wanted to make an ad inside of here, I would just go to Image, and these are all the different models that I can choose from. You know, I've been using GPT Image 2 a lot recently, and I can just say

00:10:20.000 --> 00:10:22.000
Generate me an ad.

00:10:22.000 --> 00:10:29.000
Or blah blah, blah, winks. And here are some product images

00:10:29.000 --> 00:10:46.000
Here's the copy I wanted to use, and it'll go and do that. Now, it's not gonna be very good, but, like, that's how you can go and do it. You're gonna click generate once you're ready to do that. Now, you can use the web app, and actually, in the original version of this process, we were doing all of this through manual prompts and the web app, but we're going to use the Higgsfield MCP. So we're going to bring this MCP into Claude

00:10:46.000 --> 00:11:06.000
As we've gone through before, you want to make sure you go to Customize Connectors, and pull in the Hicksfield MCP. Now, you can use other ones. The cost of static ad generation is so cheap, I don't think there's that much of a difference at all, and it's the models that I care about more than the actual aggregator. So Higgsfield, Archives, and there's a ton of other ones that get used

00:11:06.000 --> 00:11:17.000
I personally use Hicksfield, but, you know, I wouldn't say you're wrong if you use another one. I also care about the models that we use. So that's going to allow us to generate these ads inside of Claude.

00:11:17.000 --> 00:11:27.000
And the reason you would do that versus doing it inside the web app is that if you do it inside of the Hicksfield web app, you have to type out

00:11:27.000 --> 00:11:36.000
Your prompt every single time and hit generate, and then wait for it to generate. Versus if you do it inside of Claude, can I quickly pull up a chat that has

00:11:36.000 --> 00:11:38.000
A lot of them

00:11:38.000 --> 00:12:03.000
As you can see here, we're going to go deeper into this chat in a little bit. As you can see here, I am working on this skill, and it's generating me copy for 20 ads at once. And then I can generate, like, 20 ads at once rather than just going like one by one, you can generate them at scale if you use the Hicks.mcp, which once you've got the skill down, which does take a little bit of time

00:12:03.000 --> 00:12:20.000
allows you to do way, way more volume than if you did it inside of the app itself. So let's start off with something really simple. I don't want to go into this workflow yet. We are going to go into it, but I want to start off with something really simple that everyone can literally go and do now. Let's start off by recreating an ad

00:12:20.000 --> 00:12:25.000
together manually. So I'm going to start with something super easy. I'm going to go into Parker

00:12:25.000 --> 00:12:38.000
And when we go to the discovery page. Again, you don't need to use Parker for this. This is just a demo, but it's going to help. So, let's say that I want to recreate a, an ad for

00:12:38.000 --> 00:12:39.000
My brand

00:12:39.000 --> 00:12:56.000
I want to create an apology. This is the discovery tab in Parker, by the way. If you're not using this and you are a Park user, you are missing out big time, because this is… I use this all the time now, and in the MCP. Let's say I want to create a static ad, and I want to create, you know, the apology ads. I'm sure a lot of you guys here have seen, like, the we're sorry

00:12:56.000 --> 00:13:08.000
you guys have sold us out too quickly that, you know, we're doing a special offer on this deal. Like, you know, I'm sure everyone here has seen these ads, so I'm just gonna go and find one of these ads

00:13:08.000 --> 00:13:12.000
Inside of here

00:13:12.000 --> 00:13:27.000
Yeah, ideally, I'd want the text. Like I've seen a bunch of them before. Yeah, something like this, I guess. So what I'm going to do is I'm just going to save that to my swipe file

00:13:27.000 --> 00:13:30.000
And I'm just going to copy this ad

00:13:30.000 --> 00:13:37.000
That was the one that I was working for earlier and I might do that one honestly. But let's go with this one.

00:13:37.000 --> 00:13:40.000
Okay, now I'm going to start a new chat.

00:13:40.000 --> 00:13:44.000
And I'm going to say

00:13:44.000 --> 00:13:51.000
Recreate this ad for

00:13:51.000 --> 00:13:54.000
Let's say, which brand

00:13:54.000 --> 00:13:58.000
Let's say for

00:13:58.000 --> 00:14:02.000
or wellness, which is one of the outbreak plans

00:14:02.000 --> 00:14:06.000
Using the knowledge

00:14:06.000 --> 00:14:09.000
You have a brain

00:14:09.000 --> 00:14:13.000
Should I keep it super simple. And by the way, I might get

00:14:13.000 --> 00:14:16.000
I might run into usage limits

00:14:16.000 --> 00:14:27.000
Yeah, that's very possible. Okay, well, we'll see. Fortunately, I already have a bunch of chats queued with outputs. So

00:14:27.000 --> 00:14:36.000
This is an apology ad, another super simple one that many of you would have seen, a simple post-it note ad. Again, I found this on Parker by going to the discovery tab

00:14:36.000 --> 00:14:50.000
And then I just went to the ad formats and then I went to post-it note. The cool thing about this is that it sorts it by impressions. So I can see the top

00:14:50.000 --> 00:15:05.000
Post-it note ads by impression, so I can just basically see the swipe file of all post-it note ads that are, you know, have a good… I mean, it's a good proxy for post-it ads that are literally working. I think, yeah, this is… this is the one that I pulled here. You can see this one is number one by impressions,

00:15:05.000 --> 00:15:19.000
And it's been in the top 5 for the last 3 weeks. Good sign that this is probably doing okay. Anyway, I went in here and I said, here's an ad for my Dharma Dream drafts and copy for the post.

00:15:19.000 --> 00:15:23.000
I want to recreate with Winx, which is

00:15:23.000 --> 00:15:25.000
Their sleep brand

00:15:25.000 --> 00:15:27.000
And

00:15:27.000 --> 00:15:36.000
go and draft me a bunch of copy, then we're gonna make the ads. Again, I'm gonna be… we're gonna go into copying a little bit, so I'm gonna be less particular about it now.

00:15:36.000 --> 00:15:41.000
And then it went and draft the copy for me here.

00:15:41.000 --> 00:15:43.000
And I said, now go and make these

00:15:43.000 --> 00:15:44.000
Alex.

00:15:44.000 --> 00:15:48.000
And this is where

00:15:48.000 --> 00:15:49.000
Oh

00:15:49.000 --> 00:16:05.000
One quick thing, I am up here, just because I know that this is gonna be… I know, we're… we made it, we made it, everyone, but just because I know this is going to be a common question, when it comes to the product image itself, so, like, Winks, for example, did you have to upload product images at some point, or

00:16:05.000 --> 00:16:09.000
How do you get it to know exactly what your product looks like?

00:16:09.000 --> 00:16:15.000
Yeah, great question. So I actually have another chat here where I did this. This is

00:16:15.000 --> 00:16:18.000
We went through the brain, building the brain last week

00:16:18.000 --> 00:16:30.000
And I… I taught you guys through the idea of building a brand brain for yourself or your clients. Now, what I've got inside of here, inside of my brain, is a folder

00:16:30.000 --> 00:16:35.000
Or is it gone

00:16:35.000 --> 00:16:43.000
I'm terrible when it's not sort by name. There you go, other. And then brand assets. So I put my brand assets

00:16:43.000 --> 00:16:55.000
Inside of this folder, and then every time that I generate statics, it points towards this folder and picks it up. So it's… if I try to do it for overpop, it would go and use these

00:16:55.000 --> 00:17:12.000
These images, so I just have a brand assets folder inside of your brain. Now, something cool that you can do if you're an agency is I literally said, this is yesterday, because I was, like, prepping for the session, I want to run the static skills for my other, ad create brands

00:17:12.000 --> 00:17:28.000
I said, look at the… look at… I think it was Honey Love. Yeah, look at the Honey Love Brain, which had the assets in it, and go to the websites of every other brain in this ad creep brain, and create a brand assets folder. So now, all of my brains have brand assets folders

00:17:28.000 --> 00:17:44.000
Because I asked fraud codes to go and get the assets for me. But you can also just drop in your assets if you have a, you know, if you have assets inside of here. I would drop them in instead of uploading them every time, because it's annoying to have to upload them every time, unless there's specific assets that you want to get. If it's just generic product pictures, which

00:17:44.000 --> 00:18:03.000
You know, is the case for most of the SaaS that we create. All of these have just come from a folder that is pointed at. So you can get Cloudicode to do that, or you can literally just drop it in yourself, and then just when you're setting up the skill, or when you're setting up this workflow, point it at that folder, or say, go into this folder and go and take the relevant asset from

00:18:03.000 --> 00:18:08.000
For this, ideal crane

00:18:08.000 --> 00:18:12.000
Colby was asking about

00:18:12.000 --> 00:18:16.000
The workflow to pull the ads. These are all

00:18:16.000 --> 00:18:33.000
like brands I don't have access to right accounts, they just ad libraries. So this is sorted by impressions. I don't have other engagement on there, I don't have spend, obviously, because I'm not in their ad accounts, but I do have impressions, and that's a pretty good proxy. Definitely stronger than how long ad's been running. So, I actually found this layout super useful,

00:18:33.000 --> 00:18:37.000
to go and pull

00:18:37.000 --> 00:18:43.000
If I'm making like an AI animation ad, for example, I can filter for AI animation ads in English

00:18:43.000 --> 00:19:03.000
that longer than 5 minutes in this industry, and it can find me some of the top inspo for that, and I can save it to my swipe file, share it with my team, go and recreate in Claude code, or whatever. So, I love the discovery time in Parker, probably one of my favorite tabs, that we've got inside of here. And you can also pull everything through to the MCP, too, so I can just query the exact same query inside of here

00:19:03.000 --> 00:19:11.000
Anyway, yeah, thank you, Jimmy. Feel free to interrupt me, by the way, if there are questions that people are asking a lot that I

00:19:11.000 --> 00:19:14.000
that I am not getting to.

00:19:14.000 --> 00:19:17.000
So I went and did that. Super simple

00:19:17.000 --> 00:19:20.000
Not incredible, but like

00:19:20.000 --> 00:19:33.000
I just said, now go and make these and it goes and makes all 10 of these ads without me doing it, like without me being able to go and work on other work. Now, I wanted to have a little bit more variation in my copy. So I said

00:19:33.000 --> 00:19:36.000
So just give me the board.

00:19:36.000 --> 00:19:51.000
And then I said, because I'm the Parker MCP, I said, now look into my ad comments or Reddit forums to find the most emotionally loaded phrases that we can use as copy for the post-it notes. Please suggest 10 options.

00:19:51.000 --> 00:20:08.000
So I went and did that, again, because we're connected to the Parker MCP, everything, all the different data sources from Parker are pulling through to Claude Code, so it was easily able to go and find ad comments, easily able to go and find Reddit forums, and it went and drafted copy for me. Again

00:20:08.000 --> 00:20:22.000
Some of these I still didn't think were that strong, so I actually then asked it for first person testimonials as well. And then from that, I ended up picking the 10 that I wanted. So I just said, go and make these 10 inside of Hicksfield

00:20:22.000 --> 00:20:25.000
Using the MCP.

00:20:25.000 --> 00:20:28.000
I said generate. And again

00:20:28.000 --> 00:20:32.000
Let's have a look at this one here.

00:20:32.000 --> 00:20:48.000
These 10, again, just generated without me having to do anything. I just press approve and then I now got 10 statics. Are these the best stats in the world? No, but like they are using copy from our actual customers in our ad comments and Reddit forums and they were generated in

00:20:48.000 --> 00:20:54.000
No time. I can go and run these inside of the ad account, today.

00:20:54.000 --> 00:21:06.000
That's the simple, like, super simple version of this, and I actually do this quite a lot. Like, if you see an ad that you want to recreate, just literally pull it into Claude Code or Codex and say

00:21:06.000 --> 00:21:12.000
Give me some copy ideas for this, and then just go and generate 20 different versions. Another

00:21:12.000 --> 00:21:22.000
Another example of this, I don't know if I have it to hand with me right now, maybe I can quickly act on this, if I go into another tab

00:21:22.000 --> 00:21:31.000
You guys may remember we shared the ads for the Parker course, that we made

00:21:31.000 --> 00:21:37.000
When we were trying to get people into this course and we dragged this over here

00:21:37.000 --> 00:21:53.000
And this was made through this exact process. The top performing ad was this ad that I actually took from Alex Hormozi. If you look at Alex Almosi's ad library, you will find this variation of this ad in here, white background, plain text actually works very well for B2B

00:21:53.000 --> 00:22:06.000
And I literally pulled this, put it into Claude code. It already had all the context about Parker, because we've got our Parker brain. And then I said, go and make me 20 variations of copy for this specific ad

00:22:06.000 --> 00:22:13.000
This was one of the 20 variations that it made me, and this ad went on to spend 12K and was our top performer

00:22:13.000 --> 00:22:30.000
for this course. So this is a really simple use case for this, but actually pretty useful one if you see an ad and you just want to be like, oh, I just go and create me a bunch of ads like this, without turning it into a skill, without turning it into a pro, it's just a one-time, just go and make a bunch of ads on this

00:22:30.000 --> 00:22:47.000
Alex, question for you. So when you have Higgs Field connected, is there anything that you need to do in terms of selecting which image gen model you want to use? Or is that all done just like as part of what Hicksfield offers

00:22:47.000 --> 00:23:09.000
Good question. I actually can't remember because I've had the MCP since it came out, if it asked me upon the first time that I used it what model I want to use, I imagine it would have. I think now it defaults to, I'm pretty sure it defaults to GPT image two for me

00:23:09.000 --> 00:23:12.000
But I can't remember if it

00:23:12.000 --> 00:23:29.000
like, if it asks me up front, like, what image model you want to use? I think it does, but I could be wrong. Regardless, once you choose your model, it's gonna use that, it's going to assume that for all chats, or at least it did for me. If I wanted to change it, I could just say in the chat, okay, now I use Nano Banana

00:23:29.000 --> 00:23:35.000
Pro instead, or I could even say in this chat, now I want to split test

00:23:35.000 --> 00:23:47.000
Now I want to split test these outputs in different models. Give me a HTML doc of these statics in Gpt image 2 versus Nano Banana Pro versus Nano Banana 2.

00:23:47.000 --> 00:24:02.000
If I wanted to do that, that could be something that's worth doing. I'm pretty happy with GPT image too. You may want to do some testing and figure out what you like

00:24:02.000 --> 00:24:15.000
Haz asking about a format folder. That's actually what we're going to go into now. This is, like, the simple ad hoc version. The format folder is, like, the system for the skill. So let's have a look at that.

00:24:15.000 --> 00:24:24.000
Okay, I want to… I actually didn't ever check how our apology ad was doing. Okay, so it made the copy. We're going to see.

00:24:24.000 --> 00:24:28.000
I actually haven't checked the full wellness

00:24:28.000 --> 00:24:31.000
I haven't checked the

00:24:31.000 --> 00:24:40.000
The assets that it's making it based off of. So this could go or it could not go well. But we'll see. Okay, so let me show you

00:24:40.000 --> 00:24:53.000
The system for the skill, like if the ads that I showed you at the beginning, they were all built through the process that I'm going to show you now. If I go into this chat, okay, this is where it might get a little bit

00:24:53.000 --> 00:24:59.000
more advanced because we're going to talk about how to build a workflow rather than just like how to do it ad hoc

00:24:59.000 --> 00:25:04.000
Okeyoke. Let's go into here. Let's go into the latest version.

00:25:04.000 --> 00:25:11.000
So this is my workflow for the static skill. This is the exact process. Can I

00:25:11.000 --> 00:25:29.000
Perfect. This is the exact process that my static skill goes through every time that I run it, whether it's the offer-based static skill, the general evergreen engine, and different variations that we've got off the back of that. So, I'm gonna talk you through this process, then I'm gonna show you this process.

00:25:29.000 --> 00:25:31.000
Okay, so

00:25:31.000 --> 00:25:48.000
It's all based on the swipe file. So actually go back. I'm going to come back to this graphic in a second. It's all based on the format folder, as Hannah's saying in the chat, there are format folders that I've built or like templates that I've built for each

00:25:48.000 --> 00:26:06.000
skill that I have, okay? So, for example, I wanted to build that offer static skill, because I wanted to make ads for our clients on, for Black Friday. So I built a folder, a swipe file of templates to go off of and I handpicked these templates. I'm going to show you how I did that in a minute

00:26:06.000 --> 00:26:22.000
I've got this folder of all of my different templates, and this is what my skill is looking at every time that it generates ads inside of this skill. So the format folder is the first thing that you want to have

00:26:22.000 --> 00:26:27.000
Now, once you've got that in place

00:26:27.000 --> 00:26:37.000
Let's go back full screen again. Let's go through the process. And this is going to be not something that's unfamiliar to any of you guys because this is literally the process that you go through without AI. So

00:26:37.000 --> 00:26:47.000
I'll run through this research, conduct research on the brand. Do the copy. I then approve the copy. Again, I'm a big proponent for keeping human in the loop, especially if you've never done this before

00:26:47.000 --> 00:26:51.000
Then it will go and build the prompts, then it will go and,

00:26:51.000 --> 00:27:03.000
generate the ads, and then it's going to give me a board of 100, 200, 300 ads. Then I will pick from that board which ones I am happy to

00:27:03.000 --> 00:27:21.000
have, because, you know, no matter how good this skill is, you're still gonna get some duds, that's perfectly fine. You're not gonna get to the point where 100% of the ads you make are great, but the great news is, generations literally cost, you know, sub 10 cents, so even if you make 100 ads, and 50% of them suck.

00:27:21.000 --> 00:27:33.000
50% of them work, you still have spent 10 bucks on 50 ads, which is a great deal, and way, way cheaper than if you'd gone and done without Claude Code.

00:27:33.000 --> 00:27:40.000
We're going to pick which ones we like and then we're going to ask the variations and extra

00:27:40.000 --> 00:27:49.000
Extra ones like the ones that we like and then we're going to make our final picks and that's how you end up with the final board that we have that I've showed you.

00:27:49.000 --> 00:28:00.000
And the whole thing is built in a way where we can give feedback so it gets better and better and better. And the exciting thing is, like, this… these things that I've showed you here, like, they were built off of a generic skill that I threw together

00:28:00.000 --> 00:28:15.000
You're going to be able to build a skill that's tailored for your brand. So it should be even better than mine because the feedback will be specifically on your brand versus me. I'm trying to make something here. It's like, you know, agnostic enough to work for all of you if you just go and run it in your Cloud Code or hope it

00:28:15.000 --> 00:28:41.000
Anyway, as I said, this system is built off of the prompt document that I gave away in a video that I did months ago now, which, if you haven't seen it, may be worth a watch. If you want to see, like, the manual version of this process, if what I'm talking about today is a little bit too intimidating, I'd recommend going to watch this video on YouTube. I uploaded it six months ago, and it basically goes through how to do all of this in the Higgsfield web app

00:28:41.000 --> 00:28:45.000
By literally copying the prompts. So all of the prompts are inside of here

00:28:45.000 --> 00:29:03.000
You take them, you copy them, you paste them in Hicksville, you make the ad. This is, like, the pre Agentic version of this system. What I'm going to be showing you now is the claw code version of this literal system. And as you can see here, this is the template. This is the template folder or the swipe file. I literally have everything here

00:29:03.000 --> 00:29:18.000
And instead of me taking the prompts and putting them to hix field, I just have the folder inside of my grand brain and then Claude Code executes on the folder with the Hicksfield MCP. So what does that actually look like in

00:29:18.000 --> 00:29:24.000
Practice.

00:29:24.000 --> 00:29:30.000
So as we said, we've got our

00:29:30.000 --> 00:29:37.000
Swipe file. This is where we need to start. We need to start with our swipe file of ads that we want our

00:29:37.000 --> 00:29:57.000
skill to look at, whether it's offer-based statics, here is my one for just normal evergreen statics. You want to compile a swipe file of all of the templates that you want to build. Now, if you have a swipe file of statics already, great. You have somewhere to start with. You can literally, whether you use the Parker

00:29:57.000 --> 00:30:11.000
whether you use Parker and you have a smart final side there, whether you use foreplay, H3, whatever you have, you can ask Claude Code to basically just look at that and pull it into your folder, so that you can build that swipe file.

00:30:11.000 --> 00:30:27.000
If you don't have a swipe file, you can build one pretty easily. So here is the prompt that I ran to try and build my swipe file. I said I've got nothing, like, no swipe file, I've got no templates, I need to go and find me some templates

00:30:27.000 --> 00:30:42.000
So what I said was I'm creating a new static skill that's going to be based off of a swipe file of winning top static ads. I want you to look into the entire Parker database, and this is where you will need an MTP because or look at the ad library, but that's not going to help

00:30:42.000 --> 00:31:01.000
too much, you want to pull an MCP like a Parker MCP, and look at the entire database of static ads, and then generate me a HTML doc of different templates that I can pick from. So the idea here is that I literally got it to give me an entire

00:31:01.000 --> 00:31:04.000
folder of top static ads based on

00:31:04.000 --> 00:31:20.000
ads that are top by impressions from the entire database of millions and millions of ads, and now I get to pick which ones I want inside of my folder. Again, if you've got your own templates, or your own folder of static ads, you don't need to do this part, I'm just speaking to people who don't have anything or want to create something new from scratch.

00:31:20.000 --> 00:31:23.000
So Parker went and generated me this

00:31:23.000 --> 00:31:36.000
I did with the Parker MCP and now I've built this as an artifact, so I'm literally just going to pick the ones that I want. And again, you can just say, build this in a way where I can select the ones I want for my folder.

00:31:36.000 --> 00:31:51.000
All of this is built in natural language. I'm just literally describing the workflow to Claude Code and it's going and building things for me. And by the way, sorry, I should have explained this. This is an artifact inside of Claude. You can now have them pop up instead of open up in a new

00:31:51.000 --> 00:32:04.000
In a new window, and I use that all the time now. So, I built this here, and then it just popped up on the right-hand side. So, let's just say I like these templates.

00:32:04.000 --> 00:32:16.000
I'm going to go through this whole list. I see someone asked like, what makes a good template? A good template is something that is clear, not too clever

00:32:16.000 --> 00:32:29.000
Easy to replicate design-wise. Let's actually have a look through some of these, and I'll show you what cosmplets are, because I don't love many of these. This one… can I zoom in

00:32:29.000 --> 00:32:31.000
Very good. This one

00:32:31.000 --> 00:32:36.000
I like this because it's clear. It's a clear design wise

00:32:36.000 --> 00:32:38.000
I have a headline at the top

00:32:38.000 --> 00:32:47.000
I have a product, and then I have features popping out. I can easily see how I can replace my product in here

00:32:47.000 --> 00:32:58.000
And I can replace the headline and it's not going to create a lot of issues with AI messing up or hallucinating. It's a pretty versatile template, I would call it. So this is something that I'd be looking for is like, this is a good template.

00:32:58.000 --> 00:33:04.000
This, I would say, is also a good template, for the same reason you have, I mean, is that… that toilet

00:33:04.000 --> 00:33:07.000
Maybe.

00:33:07.000 --> 00:33:17.000
But still, yeah, oh yeah, it is. Headline, product, features popping out. I'm happy with that. This is a good template.

00:33:17.000 --> 00:33:22.000
Products in the middle before after, I can see how I can apply that to my product. And again, you will know your brand

00:33:22.000 --> 00:33:34.000
the best, so you will know which of these templates you can easily see your product fit into. You want to pick the ones that you think you can see your product fitting into. This one, again, I like this one too. So, you're just going to go through here, pick all of these.

00:33:34.000 --> 00:33:40.000
And again, I've just said to Cold Code, build this in a way where I can just copy the list of ones I like

00:33:40.000 --> 00:33:53.000
Like that. And now I can literally go in here and say, thank you for this. I now want you to take this artifact and build me a swipe file

00:33:53.000 --> 00:33:59.000
Of just the following ads, the ones that I have saved inside of here

00:33:59.000 --> 00:34:01.000
Now I'm going to paste

00:34:01.000 --> 00:34:05.000
I don't know why it's giving me the links. I actually would just prefer the numbers.

00:34:05.000 --> 00:34:09.000
But you get the point. I don't know why I said that.

00:34:09.000 --> 00:34:14.000
go and do that. I'm not going to run this prompt because I'm low on credits.

00:34:14.000 --> 00:34:18.000
But then basically what you would get after you do this

00:34:18.000 --> 00:34:37.000
is that you would get just this document, but the ones that you've picked. And this is now your hand-picked swipe file that you get to start with. And you can always add to this later, so don't worry about making it perfect now, but just pull in a list of a group of templates from Parker, from Atria, from

00:34:37.000 --> 00:34:53.000
foreplay from building something like this, you want that folder of templates to be the basis for what your static skill is going to be generating off of. And the more good templates you have in here, the better ad you're going to be able to make, and I can't stress this enough

00:34:53.000 --> 00:35:05.000
If you pick bad templates, it will be very difficult for you to get good outputs. If you pick good templates and you have a lot of them in your swipe file, you will be able to put out a lot of good and different static ads, because this is the way that this system works.

00:35:05.000 --> 00:35:23.000
Alex, few things that I'm seeing come up within or I guess, how would you, and we can keep this within Parker for simplicity, find ads that aren't just product related. Like if you are, you know, a service-based company or

00:35:23.000 --> 00:35:29.000
Something along those lines, like, are you able to add some of that within, within Parker

00:35:29.000 --> 00:35:50.000
Yeah, I mean, we've got industries here, so you can filter for the industry that you're looking to get the ads from. And also, I mean, sometimes it's a little bit less reliable, but even in the MCP, I have queried things that are not explicitly listed in the filters here, and it's done a pretty good job of finding it. So I'd be curious to see if you just queried

00:35:50.000 --> 00:36:13.000
I'm looking for ads made by enterprise brands or ads made by local businesses or roofers or whatever it is. And see how good it gets, even if the filters are not like specifically listed on here and you can't drill down to the exact ones you want. I also wouldn't be surprised if it did a very good job on that. I've done that a couple times before

00:36:13.000 --> 00:36:26.000
And, you know, some of them are going to be misses, but, like, that's why you go through this process of, like, given all of the different options and then picking the ones that you want to come up with your templates.

00:36:26.000 --> 00:36:41.000
B2B restaurant? Yeah, I mean, whatever you've got, I mean, if it's looking at the whole database of millions of ads, there will be, there will be ads from every type of business in there. So try and query it. I'd imagine you'll get quite a few that come back from that and

00:36:41.000 --> 00:36:57.000
If you can't for whatever reason, then the backup would be to just pull them in manually. If you've got them to hand or just look through ad libraries. But like, I mean, if you're looking through a database of millions of ads, then you're going to find some, no matter how niche your query is

00:36:57.000 --> 00:37:02.000
Janitors maybe I don't know. I haven't dried it.

00:37:02.000 --> 00:37:05.000
Anything else, Jimmy, as I'm going through this because I appreciate them.

00:37:05.000 --> 00:37:26.000
A few different things. So number one, where do you save your swipe file? Like, do you do that within Parker? Is that just a local folder that you have? Can you just tell Claude to like create a new folder with all the ads that you've saved in your swipe folder

00:37:26.000 --> 00:37:27.000
Yeah

00:37:27.000 --> 00:37:28.000
Locally, like, walk us through what you, what… or where you save your

00:37:28.000 --> 00:37:29.000
swipe file

00:37:29.000 --> 00:37:45.000
Good question. So we're gonna get into this like the the rest of the process, and guys, I apologize if we go over here. We might do, because this is quite a complex workflow, and I'm trying to get through it without sacrificing any detail. So, recordings will be made available if you do have to jump at the hour

00:37:45.000 --> 00:37:52.000
If I go into my Doc Claude, this is where the skills are stored.

00:37:52.000 --> 00:38:00.000
The skill that we're looking at now is the offer based

00:38:00.000 --> 00:38:03.000
Oh, hang on a second, I was in the wrong one

00:38:03.000 --> 00:38:19.000
Is the offer-based static skill. So, this is where my swipe file is stored. As you can see inside of here, I've got all of my ads as it's actually stored as a HTML document. Again, you can just say, once you're… as you're building this, like, we're gonna show… I'm gonna walk through building the skill here

00:38:19.000 --> 00:38:34.000
But you can just say, now put my stole my swipe file and everything relevant inside of the skill. I'm pretty sure that actually when it builds the ads, Claude made this JSON file that

00:38:34.000 --> 00:38:50.000
It actually uses instead of the swipe file itself, although I'm not 100% sure to be honest, you can, I'd have to ask Claude. But just to be safe, I just say, like, once… once I go through this entire chat, at the end of it, what I say is, like, now turn this into a skill.

00:38:50.000 --> 00:38:56.000
I can use on a repeated basis. I want you to save everything that

00:38:56.000 --> 00:39:11.000
Everything that is relevant about this skill, include my swipe file, anything that needs to go in the skill for it to be run on a repeated basis by my team, put that in the skill folder for me to access. It should be easy for me to add, update, edit, etc. And it's done that, so

00:39:11.000 --> 00:39:27.000
I don't know exactly whether it uses its wiper or the JSON file. I feel like it's a JSON, but like I like to have the swipe file in there just so everything's in one place.

00:39:27.000 --> 00:39:33.000
Oops. Okay.

00:39:33.000 --> 00:39:44.000
Yeah, so I did that. That is the one for the top of funnel static ads. Yeah, top of funnel static ads. I also ran another one for

00:39:44.000 --> 00:39:57.000
The exact same prompt, but for offer-based static ads, here's my swipe file for that. And again, these are just, I've just asked it to go and find this was not something you can specifically query for, but

00:39:57.000 --> 00:40:12.000
I just said, offer-based or Q4 ads. Go and build me an entire doc of, like, hundreds. You see there's a 350 ads that I can pick from, and I can literally pick which ones I want to turn into my… my swipe file

00:40:12.000 --> 00:40:14.000
Copy the pick list

00:40:14.000 --> 00:40:23.000
That's what I was trying to do earlier. And then I just say, now build me my swipe file for my skill using the following numbers.

00:40:23.000 --> 00:40:38.000
And you can literally have your swipe file. I have 50 to 100 in mine. If you want to categorize them by certain ad format, you can. I don't, although I think I have one, one of the skills I have does

00:40:38.000 --> 00:40:54.000
But I don't personally have mine categorized by like, oh, before and after or comparison. I just have like the visual swipe file because I just like to look at the visual and then go, these are the ones I want to pick.

00:40:54.000 --> 00:41:06.000
Yeah, so I would place a lot of emphasis on making sure your swipe file is good because that is going to dictate the quality or at least largely impact the quality of the designs that

00:41:06.000 --> 00:41:09.000
That you're going to make with Claude

00:41:09.000 --> 00:41:26.000
Brand assets, we've already covered. Let's now look at the next part of the process, which is the research and copy. Now, honestly, I wish I could do an entire session on this on its own because it does deserve it

00:41:26.000 --> 00:41:41.000
I'm not going to do it justice in, you know, the time that we have today, so I'm going to briefly give you an overview of what I have done here, because I do want to get to the rest of the process before people have to jump off at the hour. So

00:41:41.000 --> 00:41:52.000
Some of you here were in our course last year, and a big focus of our course last year was context engineering. And

00:41:52.000 --> 00:41:58.000
Content engineering, if you're not familiar, is just basically the process of teaching

00:41:58.000 --> 00:42:13.000
AI or core code, or whatever, is how to do a task, or, like, giving it the right context to make sure that it gives you the best output possible. So what we need to do here is we basically need to teach you how to do research and copy, which is, as you guys know, not an easy task

00:42:13.000 --> 00:42:30.000
So I'm just going to do like a light version of this and then you guys can hopefully take, you know, the ball and run with it. What we're going to do is basically just build a context document together on how to talk about research and

00:42:30.000 --> 00:42:40.000
Copy so that we can drop it into our skill, and then Claude can follow those instructions when it goes to actually

00:42:40.000 --> 00:42:57.000
perform this skill. So, I might say, and again, I'm just gonna… I'm just gonna basically try and brain dump everything that you know about static ad headlines, or writing copy for static ads here. So I might say, different ways to,

00:42:57.000 --> 00:43:09.000
Find inspiration slash write static ad headlines.

00:43:09.000 --> 00:43:14.000
Look for inspiration in the swipe file

00:43:14.000 --> 00:43:22.000
Look in our customer reviews or ad comments or Reddit forums or any customer voice for

00:43:22.000 --> 00:43:26.000
Phrases that are emotionally loaded that people are using about our ads

00:43:26.000 --> 00:43:30.000
But about our product, sorry

00:43:30.000 --> 00:43:34.000
Look into the ad account for

00:43:34.000 --> 00:43:39.000
angles that we have not yet tested, but show up a lot in our customer voice.

00:43:39.000 --> 00:43:43.000
For new potential opportunities

00:43:43.000 --> 00:44:02.000
That we have not yet explored. I'm just going to go in, I'm just going to talk about different ways that you can find Saturday headlines. I could put winning examples of static ad headlines in here as well. You also don't have to do this all yourself. Like you can literally go and take transcripts from YouTube videos or tweets that you want to put in here. Again, I made a video

00:44:02.000 --> 00:44:21.000
Over the last 4 years, this one, a year or two ago, about static ads, there was very DR focused, and you can literally take the transcript for this by using Glass or any tool, and say to Codex

00:44:21.000 --> 00:44:37.000
I am creating a context doc about static ads. It needs to have everything that it needs to know to make the best static ad headlines possible. Look at this YouTube transcript and turn this into a context document that I can plug into my static ad generator skill

00:44:37.000 --> 00:44:53.000
I probably should have done that in project rather than a chat, but I can go and paste that and have it generate that. Another thing that I can do that all of you here should be able to do is just say this is Codex, by the way, this is ChatGPT's equivalent of Claude code. So exact same process as we've just been going through here

00:44:53.000 --> 00:45:06.000
I said here, look at the top performing static ads for all the ad-grade clients in the last year, and analyze why they've worked extensively. So you can literally say, look at all of my winning static ads from the last year

00:45:06.000 --> 00:45:22.000
and analyze why they worked. Study them. Then based on this, produce a document on how to create great static eyes, so basically reverse engineer the process. I'm going to feed this to my new static creator skill, and I said anonymize it. I can show this if people find it interesting

00:45:22.000 --> 00:45:31.000
But, like, this is literally just basically reverse engineering what's worked about the task ads that we've created inside of our client accounts over the last 12 months. And I can take that

00:45:31.000 --> 00:45:43.000
put into my doc. Again, I wish I could go a little slower here, but I do want to get on the rest of the process and I'm happy to answer any questions about this at the end.

00:45:43.000 --> 00:45:48.000
Oops, that was the transcript. I meant. I meant to paste in the

00:45:48.000 --> 00:46:01.000
Commence pace in this. Anyway, I'd paste that in. I would have this document that now is basically a reflection of what I believe to be true about research and copywriting for static ads.

00:46:01.000 --> 00:46:03.000
Then I can take that

00:46:03.000 --> 00:46:19.000
And I can come back to my skill and I can say, okay, now you have this white file. This is a context document on how to do research for and write copy to create static ads. When

00:46:19.000 --> 00:46:37.000
are going through the process of generating me new ads. You're going to go through this process and you're going to abide by these rules to go and create me a draft copy for the static ads that you create. Once you draft the copy, after I've picked the templates

00:46:37.000 --> 00:46:54.000
You're going to give it to me for approval, and then once I approve it, you're going to actually generate the ads with one per template from my swipe file. Again, I am literally just explaining the process here. That's all I'm doing. You don't have to do anything fancy, and you can literally, if you want.

00:46:54.000 --> 00:46:56.000
Give it the

00:46:56.000 --> 00:47:12.000
Give it this. I mean, you can have my skill anyway, so you don't need to necessarily do it, but you can just, like, you can just give it this 9-step process and say, build this. Build this for me and help me fill in the gaps where you need me to fill in the gaps

00:47:12.000 --> 00:47:22.000
So that's what I'd go and say. And again, I know I've completely speedran the copy there, but you're going to want to make this document good

00:47:22.000 --> 00:47:37.000
Talk about the different ways that you actually that you actually go about doing research when you write copy. Actually, this is probably the part of the process that I try and keep the most manual. There's a reason why I still manually review the copy every single time

00:47:37.000 --> 00:47:50.000
That we run one of these statut things is because it's just really hard to make great copy with AI consistently, and you're just going to waste credits on Hicksfield if you just completely automate it, unless you have a really dialed-in

00:47:50.000 --> 00:47:57.000
Copy skill or copy component to the skill itself. So literally just

00:47:57.000 --> 00:47:59.000
Voice dictate, here's exactly what I do.

00:47:59.000 --> 00:48:06.000
And then, here are a bunch of resources that I like. Use this to go and make static ads, or at least static copy

00:48:06.000 --> 00:48:08.000
Okay

00:48:08.000 --> 00:48:21.000
Where are we up to now? We're up to research the brand has done. Oh, this is obviously assuming that your brand brain is set up. So we're doing all of this work inside the brand brain. So the brand brain covers the research part.

00:48:21.000 --> 00:48:28.000
I just covered the copy part there with the copy part, with the copy process. Then I approve the copy. So let's actually look at a chat where we did this

00:48:28.000 --> 00:48:43.000
Again, this is probably going to have a lot of stuff in here that we don't need to cover, but, like, this is literally me using this, like, in the field. So I said, take the offer-based static skill, and run it, or I could have just done this offer-based statics

00:48:43.000 --> 00:48:51.000
Run it. It went and did the research for me. This is part of my process, and then it came to me with the copy.

00:48:51.000 --> 00:49:00.000
I consolidate it in the next prompt. So let's do that instead. Yeah, okay. So basically, so you can either set it up. So you pick the templates every time or

00:49:00.000 --> 00:49:21.000
For me now, I'm happy with my templates, I just have the… I just have Claude Code pick the relevant templates. So as you can see here, I've gone straight into step 3, and it's just generated me the copy for the ads that it's gonna pick, and it's gonna pick these ones. If you really wanted to see a visual with the copy, so you can review it together, you can ask for a HTML doc or an artifact that does that

00:49:21.000 --> 00:49:25.000
I'm fine with that, I just want to check the copy quickly

00:49:25.000 --> 00:49:29.000
Normally, I go in here and I'd make some changes

00:49:29.000 --> 00:49:36.000
As I said, I like to keep this part human in the loop, but yeah, I go through the copy. If I'm happy with it

00:49:36.000 --> 00:49:47.000
As you can see here, there's a lot of different ads, and this is, like, what it's like making ads agentically. You can literally generate, like, 30 ads at a time. As I said, approved, go and make them.

00:49:47.000 --> 00:49:58.000
And off it goes, it goes and makes the ads, and let's see the first version of them come out

00:49:58.000 --> 00:49:59.000
So.

00:49:59.000 --> 00:50:16.000
You know, not mad on these. There's some pretty decent ones. There's a lot of ones that like one shot runnable already here. So basically what we've got here is the document of the as I am to review. And the cool thing about artifacts

00:50:16.000 --> 00:50:37.000
is you can literally say inside of your skill, I want you to deliver it in a way, like, present it to me however you want. I've asked for a grid where I can give feedback, and this is where it gets really interesting. So, when it goes and generates my ads in Hicksville, because once we've done the research and we've done the templates, and we've done the copy, we've done most of the hard work, it's now just generation

00:50:37.000 --> 00:50:51.000
It now goes and generates all my ads, and it delivers me an artifact like this, where I can literally give it feedback, because I can see, like, this is the… if you remember my template folder earlier, this is the one that it's based on. I can just toggle between them.

00:50:51.000 --> 00:50:55.000
Which is pretty cool. And you can literally ask it to

00:50:55.000 --> 00:51:10.000
Deliver you your statistics however you would like to. I prefer it like this. I can give feedback on this specific ad if I want to regenerate it. I can give it, I can say, if I don't like the logos in the bottom here, I can say, from now on, I never want you to

00:51:10.000 --> 00:51:17.000
Include the logo for this template in the bottom right ever again, and I can click save feedback, or I can give feedback on the whole skill and say

00:51:17.000 --> 00:51:36.000
never use discounts. We only want to do buy one, get one offers if we're doing offer-based ads. Or whatever. And that's going to apply to the wholesale intertality. Again, you don't need to do this, this is just a… the feedback loop part that I was showing earlier on how you get better over time, and you give the skill feedback, and it improves

00:51:36.000 --> 00:51:39.000
The more that you use it.

00:51:39.000 --> 00:51:45.000
So what I would do here is I would just say, these are the ones that I want to keep

00:51:45.000 --> 00:51:56.000
And if you remember, the next part of the process, once we have generated, is, like, we pick which ones we want to keep, then we generate variations

00:51:56.000 --> 00:52:12.000
So for me, I said I'm happy with all of these for now. Just go and generate the variations. And then it went and did that. And for my skill, because it's an offer based one, I just said make it more Christmassy in the variations

00:52:12.000 --> 00:52:25.000
You know, these I was pretty happy with. I think there's quite a lot of ads here that I think are good to go, and some of them still, you're going to get issues with the generations of the product. So, like, this one here, you can see the product doesn't look as good as it does in other ones

00:52:25.000 --> 00:52:38.000
So you're still going to get hiccups, especially if you've got a more difficult product, but again, we're not trying to get 100% here. If we spend 10 bucks on 50 usable statics, that is way better than

00:52:38.000 --> 00:52:54.000
Doing it outside of Claude code and you can you can see maybe you can't make the like the really flashy like O positive style of static ads where they really get technical with the design, but like 98% of statics can be recreated to the same level of

00:52:54.000 --> 00:53:09.000
quality with a good skill, with a refined copywriter, and good templates. And again, this is built off of a generic skill. You guys are going to make this custom to you, so you should be able to get a higher hit rate, per se, than I can

00:53:09.000 --> 00:53:16.000
when I'm trying to build something that everyone here can use

00:53:16.000 --> 00:53:31.000
I know this is a lot of information, but are you starting to see how the process comes together now? Like, are you starting to see the 10 steps, nine steps, or whatever it is, like swipe file first, research, copy

00:53:31.000 --> 00:53:58.000
Copy approval, generation, like, pick the ones you like, variations, final picks. Like, regardless of how you build it and how you want to present it, and you can decide that yourself, this is just what works for me, that is the structure that I feel pretty confident about. And if you want to, over time, make it more agentic or more automated, if you want to not approve the copy, or if you want to literally get to the point where you just backslash statics and it generates 100,

00:53:58.000 --> 00:54:00.000
go for it. It's possible.

00:54:00.000 --> 00:54:15.000
But I would do this first. It's more time intensive, but it will lead to you having better overall statics and having a better understanding of the process on how to make these, rather than just trying to, you know, fully automate it from day one.

00:54:15.000 --> 00:54:31.000
Yeah, the interactive output is a really great hack. Artifacts became interactive recently. And actually like now if I click keep on here, it might not work because I'm out of credits. If I click keep and I click save

00:54:31.000 --> 00:54:34.000
It will actually, like, trigger

00:54:34.000 --> 00:54:54.000
the chat. It'll go, oh, I've seen you've saved number 5972, 72, 93, 93, and 99. So they're not just static documents, they're actually interactive boards, almost, where you can… you can get it to, you can give feedback inside of here, you can… you can get it to give you the numbers of all the templates

00:54:54.000 --> 00:55:09.000
You can get it to do more like this, see the original ad. I mean, I just think that's so useful to see, like, what's actually based on, and then you can actually look and see which templates are giving you good outputs, and you can try and get more templates like those templates.

00:55:09.000 --> 00:55:13.000
So yes, great point.

00:55:13.000 --> 00:55:36.000
Again, I'm giving away… I'm giving away this skill. So maybe it doesn't work for your brand. I hope it does. I've tried to make it brand agnostic. It works for a lot of our brands, but even if it doesn't, you shouldn't just be relying on my skill. I want you guys to go and build your own version of this. And you may have a different process to me. You may… you may have a different process. I mean, you probably do to going out and writing copy or the research you want to do or how you go about getting templates

00:55:36.000 --> 00:55:42.000
But, like, I feel pretty good about this overall structure

00:55:42.000 --> 00:55:49.000
And if you want to compress it because you start to give feedback and you start to get better and better, then

00:55:49.000 --> 00:55:53.000
then that's something that you can do over time, but like make it

00:55:53.000 --> 00:55:58.000
Simple to start out with. And you can build on it. You can always make it more complex.

00:55:58.000 --> 00:56:05.000
Alex, one quick question just to clarify, are you going to be sharing the skills that you talked about here?

00:56:05.000 --> 00:56:15.000
Yes, everything's going to be shared. I'll share these documents. I'll share, heck, it'd be useful to people, I'll share our internal

00:56:15.000 --> 00:56:26.000
Our swipe files that we use to build our skills. I mean, you'll get that with the skill anyway, but, like, I can share those too. If you've seen something here today, I'm going to share it with you.

00:56:26.000 --> 00:56:39.000
Try and run it for your brand. But again, I would encourage you to understand the process and try and build up something yourself because that's where you'll really build something cool. I've got like other skills for our brand where you can literally get to the point where it can put out hundreds

00:56:39.000 --> 00:56:44.000
A week with this process once it's fine tuned

00:56:44.000 --> 00:57:00.000
Cool. One other question, too, I've been seeing a little bit just on best practices to make sure like products or apparel where there's like specific logos doesn't get distorted as you go through, you know, more and more conversations

00:57:00.000 --> 00:57:16.000
Or making the product bigger and smaller, or just, like, small text on the product images. Have you found anything to help with the, product consistency and quality to make sure that

00:57:16.000 --> 00:57:20.000
It stays the way that you want it to be presented

00:57:20.000 --> 00:57:35.000
Yeah, what's interesting is I actually haven't stress tested this too extensively with products that are super difficult. I haven't ran into any products that I haven't been able to generate or at least ones that

00:57:35.000 --> 00:57:36.000
One's

00:57:36.000 --> 00:57:45.000
struggle most of the time, like, I get ones that will sometimes struggle. I'd use… if I did have a

00:57:45.000 --> 00:58:01.000
a product like that. I'd use GPT Image 2. I think that's the best at not messing up the product as the model that you use. Also, it really is going to come down to the templates, and you want to maybe be, like, really selective about the templates you use. If you have a

00:58:01.000 --> 00:58:19.000
a product that's difficult to get, just select, like, really clear, like, easy-to-replace. You can see how you would replace your… the product in the image with your product, if you can find competitors or brands that have products that, you know, like, other fashion products, for example.

00:58:19.000 --> 00:58:36.000
Just so, like, the reason hallucination happens is because you're making the image model do, like, too much thinking, or like too much design work, as it were. Like, try and make the model not have to do a lot of hard work and thinking

00:58:36.000 --> 00:58:44.000
it should just be able to go, oh, pick that product out, put your product in, which is not always easy, and there are still some products that it can struggle with

00:58:44.000 --> 00:58:49.000
But I don't think there's any, at least that I know, like prompting hacks that you can use to

00:58:49.000 --> 00:58:50.000
One

00:58:50.000 --> 00:59:05.000
Yeah, one thing that I have found to be helpful is within the skill, you can essentially add a review agent where the only thing you're looking at is, okay, is this product the exact same as what exists within the folder?

00:59:05.000 --> 00:59:22.000
It will then come up with, like, the first pass of generations, and you can essentially just have a review agent go back and look at it to make sure that the consistency and the text and all of that is the same. Just note you're going to go through two times the amount of credits then, because

00:59:22.000 --> 00:59:40.000
Odds are it will find something that is not identical, unless your product is very simple. But if you are very cautious about making sure that everything is the exact same, adding a review agent is a pretty good trick that you can implement for just reviewing the creative.

00:59:40.000 --> 00:59:59.000
Yeah, that's a good shout. And then you could even say like when you get that folder or that artifact of ads back, you could just say like, separate this into the ones that pass through review agent versus the ones that didn't or only give me the ones that passed the review

00:59:59.000 --> 01:00:02.000
And then maybe you find that certain templates are struggling, or I don't know. That's a good time.

01:00:02.000 --> 01:00:18.000
Yeah. Okay. We are at time just to be cognizant of everyone, and quickly just going over what you guys can expect coming up. So obviously this is week four. Alex, do you want to give a quick overview on what we're going to be covering next Thursday

01:00:18.000 --> 01:00:38.000
Yeah, week five is going to be some more non like creative strategy use cases. So we'll be looking at sourcing creators agentically, possibly get time for some media buying landing pages as well. So it's going to be a bit of a mismatch next week

01:00:38.000 --> 01:00:39.000
Cool.

01:00:39.000 --> 01:00:44.000
But it's going to be a really good session. So, like, we're trying to pull in that entire Figma diagram that we showed a few weeks ago, trying to show use cases from every part of the process.

01:00:44.000 --> 01:01:03.000
Yes, and as a reminder, this upcoming Tuesday, you're going to be hearing from Manish on Hermes, Grokbot, Mew, some of these new true agent tools. So if you are interested in those, make sure you attend Tuesday's session. That is where you'll be able to learn how to get them set up, how to get them started, especially for

01:01:03.000 --> 01:01:25.000
Marketing creative strategy purposes. So, thank you everyone for being here. Alex and I are going to be continuing into this process, but if you do have to jump, we appreciate you. Reminder, if you want to test out the Parker MCP, just go to HeyParker.ai, sign up, use Parker Course to be able to renew a free month, and then remember, you can just refer friends

01:01:25.000 --> 01:01:40.000
And, get an extra month free. So, make sure you test it out. We are super excited. There's a lot of cool changes coming, soon, and I think you guys are going to really enjoy them. So

01:01:40.000 --> 01:01:43.000
Yeah, I don't know, Alex, anything else before we keep diving deeper?

01:01:43.000 --> 01:02:06.000
No, I think that was a good summary. And again, like you can do everything that we went through today without the Park MCP. It just does make it so much easier though, especially when you're building those swipe files up front just to have a library of ads, AI tagged and sorted by impressions

01:02:06.000 --> 01:02:07.000
Yeah.

01:02:07.000 --> 01:02:10.000
To go off of either in the web app or through the MCP. We built webinar swipe files for it as well. So, you know, I would highly recommend it. It's worth the price of subscription alone.

01:02:10.000 --> 01:02:32.000
Yes, and just a reminder, we'll be sending out a follow-up email either some point today or tomorrow, just depending on when we can get all the links in one spot, and we'll be adding all of that to Notion, so the Notion homepage that you guys have been seeing everywhere, that will have the recordings, that will have everything that Alex talked about and shared. So don't worry about about that.

01:02:32.000 --> 01:02:48.000
Awesome. Okay, let's go to the Q&A because I haven't been checking the chat honestly, but I'm sure there's probably a few questions inside of here. By the way, guys, like, how did you find that session? Was that helpful? Was it too much? Was it

01:02:48.000 --> 01:02:58.000
Too quick because I won't show the whole whole process, but it's also quite a loaded workflow, and it's not easy to cover and like half an hour.

01:02:58.000 --> 01:03:03.000
So people generally did like the screen shares last year, but I don't know how did it land

01:03:03.000 --> 01:03:07.000
Okay.

01:03:07.000 --> 01:03:08.000
Nice.

01:03:08.000 --> 01:03:10.000
Good stuff.

01:03:10.000 --> 01:03:11.000
Yeah.

01:03:11.000 --> 01:03:21.000
Yeah, I appreciate that. It probably does need to be slowed down. I wanted to make sure that everyone had to jump at the hour still got to see kind of the whole workflow.

01:03:21.000 --> 01:03:22.000
So

01:03:22.000 --> 01:03:29.000
I'm happy to go deep and talk about whichever part you guys want to talk about in extensive detail for the next hour.

01:03:29.000 --> 01:03:39.000
Okay, do you have any examples of local service or home improvement to hand? No, because we don't work with any. But

01:03:39.000 --> 01:04:01.000
Again, if you just query the Claude code with the Parker MCP, there will be some in there. We've got millions of ads in there, all of them are AI tagged, categorized by industry, by ad format, all sorts of different tags. So if you query that and ask it to put together a sprite file, you will find some

01:04:01.000 --> 01:04:03.000
What else have

01:04:03.000 --> 01:04:15.000
One thing that I've been seeing is someone was asking about how you are able to switch between cloud code and codecs and maintain context. So that is everything around the brain.

01:04:15.000 --> 01:04:25.000
When we are showing this, just so… so you can see, if I go here

01:04:25.000 --> 01:04:38.000
And I go to a new chat, the whole idea is when you're using Codex and Claude Code, you get to pick a folder. So in this case, this is our internal Parker brain, so this is our company brain, and that is the one that I am

01:04:38.000 --> 01:04:41.000
Sorry to interrupt, Jimmy, I'm not sure if you're sharing another screen, but we can see Slack

01:04:41.000 --> 01:04:47.000
Oh, got it. Okay, let me share the right screen then.

01:04:47.000 --> 01:05:06.000
There we go. So when I am in Codex, you can see here, I get to select this file, Parker Parker Brain. So this is our internal company brain that we get to get to use. Now, if I go to Claude and I pull that up, let me just get

01:05:06.000 --> 01:05:10.000
So if I pull this up

01:05:10.000 --> 01:05:28.000
As you can see here, I can essentially select that exact same folder. Now, our desktop app that we are coming out with, which you can see right here, is essentially the version of that. This is like the home base that keeps everything saved. And so this is where we can have all of our files

01:05:28.000 --> 01:05:43.000
that when I'm working out of it, and if Alex is working out of that, all of that is being updated on the back end automatically and making sure everything is synced. So that way, it doesn't really matter where we want to use, or what model we want to use

01:05:43.000 --> 01:06:02.000
Everything is just being synced and saved inside of this, this brain. So that's what's really helpful for us as just an organization. Whatever, if you want to use HQ, if you want to use GitHub, if you want to use Parker, like, honestly, I'm not too, too, like, obviously, we want you to use Sparker, but

01:06:02.000 --> 01:06:24.000
The most important thing is just use a brain in any way, shape, or form, because that will be such a big unlock for your team, and just you as being able to not worry about, like, feeling locked in to just, you know, Codex or cloud code. It really allows you to, like, own all of your intelligence, which is a common phrase, but just wanted to go over that one more time.

01:06:24.000 --> 01:06:26.000
Yeah.

01:06:26.000 --> 01:06:42.000
And we, like, if I was working on, say, Honey Love, for example, in Claude Code, I would have the Honey Love brain, loaded, or just the ad create brain, and just tell it to work on Honey Love, and port code would understand, which brain to look inside of, and then I just had that exact same brain loaded on Codex

01:06:42.000 --> 01:06:57.000
So there's very little switching cost when you're working on the shared brain. So couldn't plus one that enough. Someone asks, do you have again, do you have the swipe file organized by different types of ads? You can do. I don't

01:06:57.000 --> 01:07:01.000
So again, this is the one that I have

01:07:01.000 --> 01:07:17.000
for the offer based ones again. You could, you could easily have this categorized if you want, because all of these are already AI tagged by Parker anyway, so it really wouldn't be difficult to get it categorized into different types. If you prefer that, I don't think it's meaningfully going to make a difference to the outputs, because it just looks at this entire

01:07:17.000 --> 01:07:19.000
Boulder and

01:07:19.000 --> 01:07:21.000
Decides which one of the things is best

01:07:21.000 --> 01:07:28.000
But if you want to do that, you can. I personally don't know.

01:07:28.000 --> 01:07:42.000
Following up on that, and so just so you guys know as well, it's actually not just contacts that syncs. So if you go to the brain

01:07:42.000 --> 01:08:07.000
These are all of our team skills as well. Some of these are from the Parker Brain that you have seen within the within the GitHub repo. If you've gone and check that out. But actually we like this is our entire organization when it comes to our skills. So anytime that someone creates a skill, it will automatically get synced within here. If you want to know where that is, you can just go to dot cloud

01:08:07.000 --> 01:08:24.000
And then you can go to skills, and again, this is where we have all of our skills internally. So even when you're creating skills, it will be able to automatically go and add them to add them to your brain.

01:08:24.000 --> 01:08:39.000
Yeah, Joe asked if we want, like, if we wanted on-brand ads, we can upload previous brand ads to our swipe file. Yeah, I mean, just query it. Again, I don't think we have like a filter for brand versus direct response. That's a cool idea, actually. We should add that to the web app

01:08:39.000 --> 01:08:55.000
Go and query that for more on-brand ads, and then you can, if you struggle to get results, if you query that through Claude Code, you can give some examples, but again, you don't have to go and go through the process that I went through to create the swipe file. If you've already got a swipe file, you can just

01:08:55.000 --> 01:09:02.000
put that through Claude code and say, hey, here's a link to my Parker board, go and

01:09:02.000 --> 01:09:10.000
create a local… go and create a folder of every ad inside of this board. That is my swipe file.

01:09:10.000 --> 01:09:23.000
So, it doesn't matter how you get there, it's just that the important things that you get to a swipe out of solid templates that you can run off of.

01:09:23.000 --> 01:09:27.000
Oops.

01:09:27.000 --> 01:09:38.000
What have we not hit?

01:09:38.000 --> 01:09:55.000
Alex, that's actually a question I'm really interested in. So say that we are getting to a world where you could have 500 static ads generated every day and upload it to the ad account. I know you're less on the media buying side, but how do you even begin to structure that

01:09:55.000 --> 01:09:58.000
within a meta account

01:09:58.000 --> 01:10:15.000
Yikes. Yeah, this is another conversation. I actually probably think it's best to cover next week because next week we have the session with my session that's going to do landing pages

01:10:15.000 --> 01:10:37.000
Creators, and then media buying and then the Tuesday after that, we have Andre coming on who is more of a media buyer than I am. It's going to be different for different accounts. I don't want to, you know, prescribe advice for a brand launching 500 ads that they've spent in 20K a month versus one spending, like, 5 million a month. So

01:10:37.000 --> 01:10:54.000
I will probably put something together before next week's session to give a better answer to that. But it is interesting. I thought you were going to go a different way. I thought you were going to go like, how do we stand out if everyone's got AI ads? Which is also an interesting question. I think the answer to that is ugly ads, honest

01:10:54.000 --> 01:11:01.000
I don't think that this is going to be as much of an advantage in 6 to 12 months as it is today, because now

01:11:01.000 --> 01:11:07.000
You know, small percentage of people can do very high volume without sacrificing quality, but, like, soon

01:11:07.000 --> 01:11:14.000
Everyone will be able to do this in 6 months, in 12 months, you'll either be able to do it yourself, or you'll just be able to use a tool

01:11:14.000 --> 01:11:16.000
that turns out

01:11:16.000 --> 01:11:22.000
A ton of high-quality statics. So it won't be as much of an arbitrage. But

01:11:22.000 --> 01:11:25.000
That's why you should make all the ads

01:11:25.000 --> 01:11:38.000
For AI statics, Alex, at Ad Crate, are the strategists the ones that are going in and making these, or is it like an editor or designer that's in charge of making them?

01:11:38.000 --> 01:11:42.000
Good question.

01:11:42.000 --> 01:11:45.000
So we spoke about the concept before of like a

01:11:45.000 --> 01:12:01.000
Creative Strist engine. If you think about all of the different, this is how I'm looking at it internally. If you think about all of the different roles in the creative team, you have the Strategist, you have the designer, you have the media buyer, you have the editors. I think that, and we've been saying even since the course last year.

01:12:01.000 --> 01:12:19.000
They are all merging into one role. Call it, you know, whether you call it creative engineer, growth marketing engineer, you know, that role is going to merge eventually from five to one. And the way that we look at it internally is, like, I'm trying to

01:12:19.000 --> 01:12:31.000
Enable everyone on the team to become, like, whether they are a Strategist or an editor, or a designer, enable everyone to become a growth marketing engineer.

01:12:31.000 --> 01:12:36.000
Because I think that the ones who get it, who are good marketers and

01:12:36.000 --> 01:12:51.000
are smart enough with AI to be able to understand how to orchestrate different agents. I will have a huge amount of leverage of the five roles or the however many roles are on the creative team, the best place

01:12:51.000 --> 01:13:06.000
role to step into that new role is the creative strategist because they are the ones who have the DR knowledge and are generally the best marketers. So in our organization, to answer the question, it's the strats

01:13:06.000 --> 01:13:12.000
Who do this. But we're trying to have everyone step into that

01:13:12.000 --> 01:13:23.000
growth engineer, growth marketing engineer, because it's all going to be Agentic soon. Like, it's all gonna be… as we were talking about at the top of the session, like, video editing

01:13:23.000 --> 01:13:45.000
It's not long until I think it's not long at all until at scale video editing is done through prompting or through skills. And you're just going to be QCing and go and make these cuts here or like edit this in my organic style, whatever it be. So the strats do it, but I'm trying to enable everyone to become that. And honestly that just more than anything, that's just a lot of

01:13:45.000 --> 01:13:52.000
Marketing and DR training, because, I mean, even though we're in a court code and codex, course now

01:13:52.000 --> 01:14:07.000
By far the most important skill today and increasingly in the next few years is going to be actually being a good marketer, like, alongside being actually good at AI. So, if you're good at that, then… and you get somewhat dangerous with

01:14:07.000 --> 01:14:11.000
orchestrating agents, you're going to be very

01:14:11.000 --> 01:14:16.000
Very so often

01:14:16.000 --> 01:14:22.000
Another question, Alex. So just to kind of summarize

01:14:22.000 --> 01:14:37.000
What is actually included in your skill? Is it is it just the instructions to go and do all of those things? Like, the graphic was super helpful to be able to, like, kind of see how you think about it, but when it comes to the actual

01:14:37.000 --> 01:14:50.000
you know, skill.md. What is, like, in there, just so people can kind of get a good understanding of that, or like, you know, how do you get it to even look at the swipe file?

01:14:50.000 --> 01:15:00.000
You know what's funny? I actually have never, and this is probably a terrible answer, I've actually never gone inside the skill itself and looked through everything that's in there

01:15:00.000 --> 01:15:05.000
So let's check and see what was in there.

01:15:05.000 --> 01:15:09.000
I've built all of my skills from natural language

01:15:09.000 --> 01:15:23.000
And I just like say what I want in the chat and like go and go and build this and turn this into a skill. So the reason that I show it like that instead of the way that I did, instead of starting the chat by saying, I'm building a skill where I do da-da-da-da, is because

01:15:23.000 --> 01:15:40.000
Especially when you're starting a new skill, like you don't necessarily know where it's going to take you. So I'd much rather do the task in the chat first, like you saw me here, you know, build the swipe file first and then go and generate the copy and then go and generate the ads. And then at the end say, okay, turn this into a skill with everything that I need

01:15:40.000 --> 01:15:59.000
I'd much rather do it that way than try to dictate the direction that it goes by saying, build a skill that does this, this, and this. Regardless, I haven't actually checked inside this hole, so I don't know what's inside of here. It's just gonna be a, you know, combination of everything that I've said in chats to add into this skill. So.

01:15:59.000 --> 01:16:02.000
You guys are gonna get the skill, but it's just

01:16:02.000 --> 01:16:10.000
I guess a description of what it does and how it works. The swipe file is in here.

01:16:10.000 --> 01:16:13.000
So here you can see all of my different templates

01:16:13.000 --> 01:16:29.000
The JSON file, which I believe is what it looks at when it actually generates the ads. And then there's a bunch of different process files. So this is, like, from my… like, some of these are from my context doc that I built, some of these are just from feedback that I've given

01:16:29.000 --> 01:16:54.000
Or just, like, the actual process it takes to go and execute on the skill. I don't know, I wish I had a better answer to this, honestly, but I don't… I haven't looked inside the skill to see what it's made up of, because I just make everything through the chat

01:16:54.000 --> 01:17:00.000
Okay, good question here from someone on Anonymous.

01:17:00.000 --> 01:17:09.000
Is it possible to generate these images into editable layers for designer in Figma? I actually haven't

01:17:09.000 --> 01:17:14.000
Tested this where it generates

01:17:14.000 --> 01:17:33.000
Them in Figma versus in Hicksfield or at least takes the Higgs field file and turns them into Figma files. I don't know. I'd be curious to test that. If I do want to make edits to the file, which is not as often as you might think it would be

01:17:33.000 --> 01:17:40.000
if it's a simple fix, I just regenerate it because it's so cheap to do

01:17:40.000 --> 01:17:49.000
And I don't have to, you know, do any editing. If it's like a… like a nuanced edit, or it's something that is not going to be easy for Claude Code to do

01:17:49.000 --> 01:18:04.000
All I feel to do in a regeneration. Then I use Canva's magic layers, which is just a tool that you can drop any image in, and it will turn it into editable layers, and then you can just edit in Canva. I don't know if Figma has a version of that, maybe it does

01:18:04.000 --> 01:18:19.000
But I haven't actually tried that. But then again, like, again, if you use the right templates, for the most part, you shouldn't have that many ads that you need to take out and then actually work on the project file and change things around.

01:18:19.000 --> 01:18:20.000
So

01:18:20.000 --> 01:18:22.000
I don't know

01:18:22.000 --> 01:18:38.000
Also, on top of that, I will say is browser control gets better, it will be a very… even if the Figma MCP wouldn't be able to do it, I do think if you have something generated, you could literally say, hey, go and recreate this exact same thing

01:18:38.000 --> 01:18:46.000
Using my browser inside of Figma, and within the coming months, like, I think it will be

01:18:46.000 --> 01:19:04.000
pretty good at being able to do that extremely well. So, that's one other way that you could go about it, too, because I know the MCP hasn't been… the Figma MCP, from what I can gather, has not been, like, a, you know, absolute game changer, and still seems like it's pretty elementary.

01:19:04.000 --> 01:19:15.000
Yeah, I saw a Cody tweet yesterday that he was building landing pages with it and it looked decent. But I don't know, I actually haven't played with it that much

01:19:15.000 --> 01:19:32.000
Sommer says, I'd like to express my gratitude. I've literally just created static ads for my new business. Wow, that is incredible. Thank you so much. I'm glad that you found this session somewhat valuable. That's what we love to see.

01:19:32.000 --> 01:19:39.000
Simon says, can we find the skills shown today in the GitHub you shared before? It's not in the Parker brain currently, I don't think.

01:19:39.000 --> 01:19:47.000
But I can get in there, but again, you guys are also gonna get the scale sent out probably tomorrow, whenever the email goes out.

01:19:47.000 --> 01:19:56.000
I don't think it's currently in the Parker brain, but we can also get it in there. Do you use codex to generate static ads ever, or just chord code?

01:19:56.000 --> 01:20:05.000
Honestly, I… anecdotally, I haven't done too much testing on codecs, but whenever I have, I've just found Claude Code to be better at

01:20:05.000 --> 01:20:11.000
Using the Higgs for MCP. I don't know if that even makes any sense because in theory, it should just be

01:20:11.000 --> 01:20:18.000
Choosing the same MCP, unless Jimmy, like, does it… does it, like, like, pipe a different prompt

01:20:18.000 --> 01:20:20.000
To

01:20:20.000 --> 01:20:21.000
The only

01:20:21.000 --> 01:20:23.000
To Hicksfield, if it's core code or codex

01:20:23.000 --> 01:20:42.000
And this isn't confirmed, but this is my best guess of what OpenAI is doing because OpenAI has an image gen model, I would strongly bet that if you connect the Higgs field MCP to Codex.

01:20:42.000 --> 01:21:01.000
That it is going to, on the back end, essentially say, hey, unless directed otherwise, always use the, you know, image gen model in Higgs field compared to Claude. I'm guessing it's gonna most likely not be that. I don't know which one it would point to, since obviously Anthropic does not have an image gen model

01:21:01.000 --> 01:21:10.000
But that would just be, like, one thing to note if you're using Higgs field in both of them.

01:21:10.000 --> 01:21:20.000
Yeah. I don't know. Anecdotally, I've found that Claude code tends to be better at using the hexode MCP.

01:21:20.000 --> 01:21:28.000
Although I haven't done too much inside because I'm being totally honest.

01:21:28.000 --> 01:21:40.000
The static ads in the swipe file somehow organized by funnel, top of funnel, middle funnel, bottom funnel? No. So what we have is, like, the actual skills that we have, like the

01:21:40.000 --> 01:21:58.000
Like OG evergreen static engine just basically does top of funnel. So when I say like static ad, like our static ad skill, it's pretty much exclusively top of funnel. And then we'll have a separate one specifically for bottom of funnel. So I mean, they're not the swipe files are not organized by

01:21:58.000 --> 01:22:20.000
By, like, top of funnel, middle funnel, bottom funnel, because we just have different skills. We have different swipe files for top of funnel versus, like, offer-based ones. You can if you want. If you wanted to do it all in one skill, you can have it be, you know, prospecting and retargeting, I guess, and then have it say, like, 80% of the ads must be prospecting ads versus 20% retargeting

01:22:20.000 --> 01:22:34.000
Absolutely nothing wrong with that. We just prefer to have them in separate skills, because there are some, like, principles for top of funnel ads that I want to maintain, you know, for example, assume no one knows or cares.

01:22:34.000 --> 01:22:49.000
That obviously is a lot more applicable at top funnel than at bottom of funnel, so I just keep them as separate skills, and every week when we run the static generator, it's like, okay, our evergreen ones, our top of funnel ones, that's the big one that churns out a lot, and we also have another one that churns out a bunch of

01:22:49.000 --> 01:22:51.000
Offer-based discount bottom funnel ones

01:22:51.000 --> 01:23:06.000
Yeah, one other thing too is we actually go through for every ad and tag it by the awareness level. We do not go off of top, middle, bottom. We go more off of it's Claude Hopkins, right? Five stages of awareness, Alex.

01:23:06.000 --> 01:23:08.000
Eugene Schwartz

01:23:08.000 --> 01:23:36.000
Eugene Switch. Yep, yep, Eugene Schwartz is five stages of awareness. So that's what we go off of. And so even within ad libraries, you can actually see and filter by the different tags. So if you wanted to go by awareness level, you can come here. Most aware problem where unaware. So if you wanted to just see unaware ads, you could come into here, select that, and then have that. So when you're using the Parker MCP

01:23:36.000 --> 01:23:39.000
You can just natively ask, you know

01:23:39.000 --> 01:23:54.000
Claude Code, Codex. Hey, can you just pull in unaware ads, to this white file, and it would be able to do that for you. And you could create this white file just all through natural language.

01:23:54.000 --> 01:24:12.000
Maggie asked, do you use this static generation skill for iterating on winning ads? Here's where I'd encourage you guys to you can create different skills. Like I would, again, just in the like following on of that idea of keeping things simple and not trying to do too much upfront

01:24:12.000 --> 01:24:37.000
You don't have to create one master tactic skill that does everything. It does top of funnel, bottom funnel, iterations, new ads. Like, just keep them as separate skills. And then you can have a different skill that instead of starting off with the swipe bar, it could start off by looking at the ad account and looking at the ads that are working and iterating on those ads. That is a great idea for another skill that everyone here should go and build. I would actually recommend having that as a separate skill

01:24:37.000 --> 01:24:45.000
Versus trying to do everything in one. So it's the same process, post

01:24:45.000 --> 01:25:00.000
you know, getting to the like actual template that you work off of is just the template would be something from the ad account that's pulled in from the Parker MCP versus something from the swipe file of templates that we have.

01:25:00.000 --> 01:25:01.000
Great question.

01:25:01.000 --> 01:25:21.000
Yeah, and what I would say is just remember, go back to the simple versus complex skills. So AI static ad generation. If you wanted that as the parent level skill, you can have a bunch of processes below that. So if you wanted every process to be a different format of how to go and execute that, then it'd be really easy. Then you wouldn't have

01:25:21.000 --> 01:25:38.000
When you do the backslash, you know, dozens and dozens of skills for each different format, and then it just kind of gets overwhelming, you can just have an AI static ad generation complex skill, but then within that skill, you have the processes which lay out the step-by-step of like, here's how to best

01:25:38.000 --> 01:25:48.000
Create an offer-based skill, or a sticky note static skill or whatever. And you can organize it that way.

01:25:48.000 --> 01:26:05.000
For sure. Brent asks, how do you go about creating a new skill for a different format? Let's just say it's us versus them. Do you just collect us versus them info ads and ask Claude to create a skill based on that? This is a really interesting concept. So again, there is no right or wrong way to

01:26:05.000 --> 01:26:27.000
You can create one master skill that does everything. You can create you can even go as granular as creating one skill per ad format as Brent suggested here. If that is a format that absolutely crushes for you, like us versus them, for example, it could be worth creating a specific us versus them skill so you can load it just with context about us versus them

01:26:27.000 --> 01:26:44.000
You know, this is what we compare to. We compare to our competitors, we compare to previous states, we compare like zero versus 30 days, zero versus 120 days. Like, if that's something that really works for your brand, then maybe you go and create a skill specifically for that format.

01:26:44.000 --> 01:27:04.000
Personally, I just have, like, the evergreen top of funnel one that has all my different formats in it, and if I want to add a new format, I might just say Parker MCP, go and find me, 20 us versus them ads, and let me pick the one, like, that I want to use as a template, and then once I pick that one, you're going to add it to my

01:27:04.000 --> 01:27:12.000
top of funnel, evergreen static skill. Like, that's how I would do it, but if you wanted to go and create a specific skill for that ad format

01:27:12.000 --> 01:27:19.000
You can also do that. There's no like regardless of how specific or

01:27:19.000 --> 01:27:31.000
broad you want to go with your skills. Not only work, and it's easier to build something that is more niche and more specific, than building one master.

01:27:31.000 --> 01:27:39.000
overall scale

01:27:39.000 --> 01:27:49.000
Yeah, yeah, that's the other thing. I mean, I don't know. I haven't actually tested this, but it does feel like now when

01:27:49.000 --> 01:28:03.000
when I run my skill, because it's got a lot in there, I do feel like it uses… it uses… it's quite token intensive, because there's a lot of context inside there. So maybe that's a reason for me to,

01:28:03.000 --> 01:28:05.000
For me to

01:28:05.000 --> 01:28:14.000
start making my skills more specific, rather than, like, obviously the bigger your skill is, the more token intensive it's going to be to run.

01:28:14.000 --> 01:28:15.000
So

01:28:15.000 --> 01:28:27.000
I don't know, I don't have any data for that though. I just I just see my little usage thing going up and up and up when I use it. But I'm also getting a lot of good ads, so I don't care.

01:28:27.000 --> 01:28:28.000
Yeah, that's the other thing

01:28:28.000 --> 01:28:29.000
Other questions? I'll go for it.

01:28:29.000 --> 01:28:41.000
No, I just want to say the other thing, Jeff's comment in the chat, you can build something simple to start off with and you can just add to it over time. You can just add new formats, you can give it feedback, it'll get stronger and stronger. So you don't have to

01:28:41.000 --> 01:28:43.000
worry about making things super complex up front

01:28:43.000 --> 01:29:01.000
Yeah. What other questions do you guys have? Anything about Alex's workflow that you want us to dive deeper into or I mean, throw out anything that you guys got. We are here to stay on as long as there are still good questions coming through

01:29:01.000 --> 01:29:18.000
Gonzalo says, awesome knowledge. Thank you very much. You're giving some super helpful ideas. How would you go about creating variations for each static you create at scale? Yeah, so what I actually haven't done this yet, but what I what I should do is

01:29:18.000 --> 01:29:30.000
that document that we built… let me pull it up again, I mean there's not much here, but the document that we built

01:29:30.000 --> 01:29:34.000
Say this was a finished document about static ad

01:29:34.000 --> 01:29:36.000
Copy

01:29:36.000 --> 01:29:45.000
In theory, we should be building another one for variations. Like everything, everything context wise about how to

01:29:45.000 --> 01:30:00.000
Like, how to create variations. For example, internally at Create, we have a process for creating different variations, where it's almost like a playbook, like, sometimes we will, sometimes we'll create, like, variation A will be one persona, and then we'll use different personas, sometimes we'll use different, like.

01:30:00.000 --> 01:30:06.000
hook templates on the copy. So, you'd want to write all of that down. I actually don't have that in my skill currently.

01:30:06.000 --> 01:30:15.000
For example, I actually can't remember how like in which chat I set this up originally, but I think in one of

01:30:15.000 --> 01:30:31.000
in one of the chats here, where you saw the originals, this is the variations, you saw the originals, this is the variations. I literally just said to Claude, like, when I was building the skill, I'm making these, like, these are offer-based

01:30:31.000 --> 01:30:46.000
So I want your variations to be more Christmassy and more like holiday themed, and then, like, you already know the ones that I like, go and be creative and create some different variations with it, even a different copy or different design. I know that's probably not good advice.

01:30:46.000 --> 01:31:06.000
But if you wanted to do it by the book, you should technically put in the variations context here and talk about how you create variations, like, without AI. Or you can just, if you're happy with the outputs, you can say, I like these. Go and give me variations that you think are good to go, either design or copy wise. And I'm pretty happy with like some of these, I didn't get these Christmassy ones in the first batch

01:31:06.000 --> 01:31:11.000
And I think they're pretty good for, you know, offer based statics. So

01:31:11.000 --> 01:31:15.000
It depends how strange you want to be on it.

01:31:15.000 --> 01:31:16.000
But

01:31:16.000 --> 01:31:39.000
I usually just let it go, and sometimes if I don't like it, then that's when I jump in and say, okay, this is my exact process for variations, and you've got to follow this structure

01:31:39.000 --> 01:31:54.000
So this has been asked before, is the top of funnel skill also accessible to us, or just the offer skill? They will be both. They'll be both. I think I might need to do a little bit cleaning up of the top of funnel one, because it might be tied to some of the ad creep brain, so I need to pull it apart from that, but, like

01:31:54.000 --> 01:32:13.000
the offer-based one will definitely be in the folder tomorrow, maybe Saturday or Sunday before the other one is, but I can get it in there. But again, just to emphasize, like, the templates that you use will be important, and make sure that it works for your brand. Like, if you have a product that's not easily gonna fit into

01:32:13.000 --> 01:32:15.000
The template

01:32:15.000 --> 01:32:29.000
then it's… it's gonna struggle to give you good apples, because it's always gonna be a ceiling on how good they can be. But yeah, I can share ours

01:32:29.000 --> 01:32:45.000
Mark, I can dive into your question. How do you provide design feedback on your different batches, having the brand designer, marketer, QA, your assets? This is what I was talking about when you can just at the end of the skill, add in a review agent

01:32:45.000 --> 01:33:01.000
And you can give it context to specify really what you want to look at. So, for example, just so you can have an understanding of like what this could look like, we have a

01:33:01.000 --> 01:33:06.000
Let's see here… where is that? Okay.

01:33:06.000 --> 01:33:29.000
So we have a context doc. This, I think, was based on something that Sarah Levinger came up with. If you're familiar with her, she's really great at psychology-based design. And I think she had a YouTube video that she had come out with, which is really just, like, the psychology of good static ad design

01:33:29.000 --> 01:33:51.000
And you essentially tell it, like, hey, I want you to look at the ads that you have generated, and essentially QA it off of this material, and let me know where there could be some feedback or room for improvement. This is obviously more from, like, a direct response psychology design, but you could also have something that's like your brand guidelines of like the must haves

01:33:51.000 --> 01:34:21.000
The font rules, the design rules, the logo rules, you know, all of this that you could be looking at. And it's to set that up at the end of your skill, like, literally just within Claude Code, or wherever you have your skill, you could essentially just be like, you know, hey, for the static ad skill that we created today, I want you to add one extra step, which is to spawn a review agent, and I want this review agent to look at the different static ads that were generated and evaluate it based on this criteria.

01:34:21.000 --> 01:34:44.000
Yeah. And you could then just paste in, you know, something along the lines of, like, this at the very bottom, and then boom, you have essentially a QA slack or not slack QA agent that would go within Cloud Code and review the design and give you feedback.

01:34:44.000 --> 01:34:55.000
Just quickly, I should have asked this when everyone else was on. Is any… by any chance, is anyone going to Commerce Roundtable on Monday and Tuesday in San Diego? Is there anyone here in the chat who is?

01:34:55.000 --> 01:35:01.000
I'm just curious.

01:35:01.000 --> 01:35:07.000
No. Okay, what's worth asking.

01:35:07.000 --> 01:35:09.000
Vijay

01:35:09.000 --> 01:35:11.000
As a really interesting question.

01:35:11.000 --> 01:35:22.000
Is there a way to AB test results for a static ad campaign and let Claude understand the analytics to revise the new batch of creatives? This is why

01:35:22.000 --> 01:35:34.000
We built the system in a way where, like, it can take on feedback and it can get stronger. Here's where it becomes really interesting. If I go back to that graphic

01:35:34.000 --> 01:35:38.000
This graphic yeah

01:35:38.000 --> 01:35:41.000
Of the nine step process

01:35:41.000 --> 01:35:44.000
You could easily say

01:35:44.000 --> 01:36:01.000
If you wanted to add on to this or like amend the first step or add a step before it, it could be, you know, this runs every week, say it runs on a Monday. The first step could be check the ad account using the Parker MCP for things that have worked

01:36:01.000 --> 01:36:06.000
And based on that, select the correct templates

01:36:06.000 --> 01:36:13.000
or add new templates to the swipe file based on literally what's working. Sorry.

01:36:13.000 --> 01:36:30.000
So that's where it's really interesting because then it's like a self-improving loop. It gives itself feedback based on what's worked inside the ad account. So yes, to answer your question, that's more of an advanced thing, and you can absolutely get a lot of statics without doing that. But like that's how you can get to learn from what's happened in the ad account if you have this run on, say, like a weekly basis.

01:36:30.000 --> 01:36:49.000
Yeah, and even building on top of that, I mean, this is where you can really have a lot of creativity. You could create a hypothesis tracker inside of your notion or not Notion, sorry, Claude or Codex or wherever and essentially just say, hey.

01:36:49.000 --> 01:37:11.000
We want to take the performance, so say you have the Parker MCP that can pull in the performance of different statics, and we want you to build a hypothesis tracker that is looking at these different variables that we're really interested in testing to see if they move the needle, and for any ads that involve those elements, we want you to add them to the hypothesis tracker, and we want that to then

01:37:11.000 --> 01:37:15.000
I guess, like.

01:37:15.000 --> 01:37:32.000
Provide feedback and kind of ideation for future batches. So you could have an entire system and set that up as a routine where every day you're going in, you're pulling the metrics from Parker or whatever, you know system you've used to get the metrics from Meta

01:37:32.000 --> 01:37:53.000
Into a Google Sheet or Notion tracker that is then going to say, okay, if, you know, these statics are performing well, you know, around these hypotheses, add them here and let that dictate what we should do in the future. So what I would say to that is, whatever you're dreaming up in terms of this, like, A-B testing idea, just like spend 10 min

01:37:53.000 --> 01:38:09.000
describing the ideal state to Claude Code or Codex, and odds are it will be able to build that for you as long as you have some way to connect to the meta ad account to be able to track whatever hypothesis you want to

01:38:09.000 --> 01:38:14.000
So yeah, it's definitely possible.

01:38:14.000 --> 01:38:30.000
Shazaf asks, how do you think the future creative strategy is after AGI takes this over to? I'm actually so bullish on creative strategy and, like, being a marketer right now. It is the most exciting

01:38:30.000 --> 01:38:43.000
Period of all time. Like, it's… I mean, I'm not coach actually hasn't been around for, like, what, a few years, but, like, it's never been a better time. If you can understand how to use these tools, and how to orchestrate agents

01:38:43.000 --> 01:38:59.000
You will be, and you are a good marketer, you have… you can do anything. Literally, I think I saw a tweet the other day from someone saying, like, you can build an e-com brand with, you know, 3 or 4 really good AI pilled people now. I think it's so true. Like, you can be a one-man creative team

01:38:59.000 --> 01:39:10.000
And I do think that the last thing that AI will get great at, if it ever does, is human judgment. That's why we looked at earlier the templates like

01:39:10.000 --> 01:39:26.000
80 to 85% of them would not have been good templates, but it wouldn't have known that if I'd asked it to go and pick the ones that it thinks is best. It still needed my judgment as a marketer, having seen, you know, thousands and thousands of ad accounts, millions of ads, probably, maybe not millions, a lot of ads

01:39:26.000 --> 01:39:41.000
And knowing which ones I think would be the best for my brand. And I do think it's going to take a while before AI is truly better at humans than humans at actual judgment of something like that

01:39:41.000 --> 01:39:59.000
So look, I think anyone's lying if they tell you that they know what the future of creative strategy is for the next two, three, five years, because things are moving so quickly. But I think it's such a huge opportunity right now. And I think that regardless of what happens with AI over the

01:39:59.000 --> 01:40:09.000
You know, 3 to 5 years, if you're a great marketer, and you are somewhat capable at using AI, you're going to be really, really valuable to a lot of businesses

01:40:09.000 --> 01:40:15.000
Or your own business

01:40:15.000 --> 01:40:27.000
Yeah, this is why like Gmail, I get so passionate about this. Like we weren't going to do another course after last year. It's honestly quite a lot of work to put this together. But like we started seeing

01:40:27.000 --> 01:40:42.000
what this was doing for us internally, and we're like, oh, dude, we've got to share this. Like, there's a huge gap in education. There's no shortage of good direct response marketing content online, but there is a shortage of people who know direct response marketing, who can,

01:40:42.000 --> 01:40:45.000
who can talk about this stuff

01:40:45.000 --> 01:40:55.000
So we thought we had to share it, but yeah, I'm just so incredibly bullish on great marketers, great creative strategists, now and over the next few years

01:40:55.000 --> 01:41:16.000
Yeah, I also do appreciate that, Sandra. We'll keep it going as long as we feel like there's something actually valuable to present. But yeah, I think to Alex's point, like the worst case scenario for creative strategy is it just kind of gets bundled up inside of like this marketing engineer role

01:41:16.000 --> 01:41:37.000
Where it's almost like you need to be able to understand, like, okay, well, how does… how do you actually do media buying well too? How do you create, you know, landing pages for the different creatives? So it's like, maybe because AI is making us all so much better at whatever it is, the job, if you have the basic understanding of performance marketing

01:41:37.000 --> 01:41:51.000
Then it's like, can you just continue to have the full cycle of the performance marketing knowledge? And I think that's what's going to become more valuable over time. So it's like the idea of

01:41:51.000 --> 01:42:09.000
Becoming a marketing generalist, I actually do think is going to become more valuable because you won't need a team of strategists and editors and media buyers and designers to make it all happen. There is a world, you know, say two to three years from now

01:42:09.000 --> 01:42:32.000
Where one person could do a lot of that work. And so if that can be you, I think that becomes extremely valuable. But I still think direct response advertising to Alex's point is one of the most important skills to know. So at the very least, if you understand this, I think there's always going to be a world in which people like this are needed.

01:42:32.000 --> 01:42:49.000
Yeah, for sure. Thank you, Adam. You've done a great job not making it grifty sales hype session. Yeah, I mean, like, we try and be an open book on these sessions. We are so passionate about this stuff. And obviously we're passionate about Parker, but like actually I probably did the service. We

01:42:49.000 --> 01:43:04.000
Like, we… although the course was a lot of work last year, we actually did love. I love, I love doing these sessions with you guys, so we were super stoked to do it again this year, and we just want to keep on sharing everything that we can in a way that doesn't feel like we're trying to pitch

01:43:04.000 --> 01:43:14.000
Just a way that's educational, and, like, just showing you what we do internally, and if it's valuable, then great. And if not, then we'll stop doing them.

01:43:14.000 --> 01:43:20.000
Are you more excited about the AI piece or the marketing opportunity? What do you see yourself doing 5, 10 years?

01:43:20.000 --> 01:43:31.000
I have no idea Sandra, all I see myself doing five, ten years. You know what's interesting to think about? And this is where this is where it does come, like, become very interesting.

01:43:31.000 --> 01:43:38.000
If you had

01:43:38.000 --> 01:43:55.000
Imagine if you could speak to yourself one year ago and say like everything that's available today that you now know, here is everything that's going to be available to yourself one year ago, how far in the future do you think that will be? I think a lot of people have said two, three years

01:43:55.000 --> 01:44:09.000
But, like, here we are, 12 months later, and we have everything. This always happens in AI, always, it always does happen faster than you, expect it does. So it's so hard to predict. Like, if that's what it was like from last year to this year, what it's going to be like from this year to next year

01:44:09.000 --> 01:44:20.000
There's probably gonna be a lot of things that we haven't even considered, like, Claude code and codecs weren't even a thing until January of this year. So… I don't know. I don't know what I'm doing in 5 to 10 years. Probably something around

01:44:20.000 --> 01:44:35.000
Educating people have to be great marketers, or building tools or agencies that help people with their marketing. It's always, always, always going to be a massive pain point. There are always going to be businesses who want growth and are not good marketers, because most people are not. So.

01:44:35.000 --> 01:44:53.000
I don't know what I'll be doing, but something in this space. And again, I am very, like, very strongly in the camp of all this AI stuff is great, but if you're not a good marketer, it doesn't matter how good you are at AI. Like, you're just going to be amplifying average work

01:44:53.000 --> 01:44:55.000
So

01:44:55.000 --> 01:44:56.000
Yeah.

01:44:56.000 --> 01:45:12.000
Yeah, if you want to be great at marketing, there's a million resource out there. I've been uploading YouTube videos for the last three years on that topic specifically. And if that is something that you feel like you can improve in, I would encourage you to do a lot of work on that and then come through a course like this

01:45:12.000 --> 01:45:31.000
Yeah, yeah. You know, I think if you think about the one thing that AI is going to do regardless is it's going to make more entrepreneurs. It has never been easier to build a product that you could in theory turn and sell. It's never been easier to delegate all the work that you previously had to do to start a company

01:45:31.000 --> 01:45:53.000
And so… and on top of that, I think there's going to be less companies where you have tens of thousands of employees in the future. And I think all of that is just going to create, like, this sort of renaissance of entrepreneurship. But the one thing that it is clear that AI cannot do on its own is just grow a company. Sure, it can build software. Sure, you know, it can

01:45:53.000 --> 01:46:08.000
invest money better than humans can, but up to now, we have not seen anything that indicates that AI alone is going to become a better marketer than, you know, than humans. And so

01:46:08.000 --> 01:46:16.000
I truly do believe that the demand, to Alex's point, the most valuable

01:46:16.000 --> 01:46:36.000
currency is going to be attention in the future, and that's only going to get more and more, you know, important. And so, if you are someone that can create a sense of attention and demand to a product, you are going to be in a really good spot for the future. So, who knows exactly what we're going to call the rolls? I mean, it's still funny to think here, and

01:46:36.000 --> 01:46:39.000
you know, pre-2

01:46:39.000 --> 01:46:59.000
7, or whatever it was when Facebook was created, none of us would have a job, you know, that was 20 years ago. And obviously the pace of technology has scaled significantly since then, but no one would be here right now if Facebook was never created. And so it's

01:46:59.000 --> 01:47:15.000
it's impossible to know what 5 to 10 years is really going to look like. There will be more, tools, there'll be more platforms, there will be more AI advancements, but the one thing that I can guarantee you that has been true since the beginning of time is if you are able to

01:47:15.000 --> 01:47:28.000
Figure out how to convince people to buy something. There will always be a role that exists for you in the world, and I just don't think AI is going to be able to do that out of the box.

01:47:28.000 --> 01:47:39.000
By the way, thank you so much, all of the 160 of you who are still here. Means a lot. I know that we're doing two of these sessions a week now

01:47:39.000 --> 01:47:57.000
4 weeks in, so we're talking about 3 hours a week. It's such a huge commitment, and we really appreciate everyone taking time on their busy schedules to come and hang with us, and we find these, like, extremely fulfilling to do, so just want to shout out to you guys, and thank you for staying on, especially you guys and the OGs.

01:47:57.000 --> 01:48:11.000
staying on for the full second hour as well. Let's go over a few more questions. I've noticed, Maggie asks about a question about the Parker brain. I've noticed now with some of the brain, some of the things take a long time to run, even for more simple questions.

01:48:11.000 --> 01:48:23.000
Is that common? Do you guys notice this as well? If you use the Parker brain, I don't know, Jimmy, you want to try and pull up the GitHub or show something. If you use the Parker brain

01:48:23.000 --> 01:48:31.000
It is quite token intensive to run, especially initially, and then also on the

01:48:31.000 --> 01:48:52.000
On prompts, I mean, it's not too bad. When you… once you've got it set up, but, like, a true brand brain is going to be quite token intensive. Hard to comment on Maggie, or, like, on your specific, because I don't know if you're using the Parker brain or not. But yeah, we are trying to find a way to bring out, like, a light version of the Parker brain, so it's not as intensive if you don't have

01:48:52.000 --> 01:49:09.000
Or if you're an agency that doesn't have, like, a ton of tokens to spend on generating 20 brains, or you just don't have tokens in the first place. But yeah, you can also create your own version of it, like, without using our version. Or I wonder if you've got a Parker brain set up, if you can say.

01:49:09.000 --> 01:49:17.000
What would a light version look like this… look like this, and then build it for me for a client. I don't know, I haven't tried that myself. But I don't know. Show me what you think

01:49:17.000 --> 01:49:35.000
Yeah, so there's two things that we have implemented inside of the brain, just so you're aware. You can turn these off. Just tell Claude, like, hey, I don't want these. The first one is essentially like a creative voice review, which is really this idea of how can we avoid AI slop within the writing

01:49:35.000 --> 01:49:51.000
So when it generates a script or a headline, it's gonna automatically spawn this agent that will go and review it to look for any AI isms. And so if you want to turn that off, if you want to have your own, you definitely can, but that is probably what is leading to some things. And then the other one is just the context. So

01:49:51.000 --> 01:50:13.000
It's looking at like, hey, you know, go and look at this brand and make sure the ideas that you're coming up with are reflective of the strategy of this organization. And so go and look through, you know, the audits, go and look through the competitors, those sorts of things to just make sure that like this is actually a sound creative strategy concept and not just something that it pulled out of the blue

01:50:13.000 --> 01:50:29.000
So those two agents exist, and so if you're just asking for creative strategy things, those may be what is causing you, especially if it's Fable or yeah, especially if you're using Fable or like GPD-6 Astra.

01:50:29.000 --> 01:50:41.000
Because those models are really good at, like, listening to instructions and actually going and doing it and trying to do it to the best of its ability, you'll see those two start to take longer to just properly go through.

01:50:41.000 --> 01:51:00.000
Yeah, that's the other thing, it's also the model you're using. I'm finding myself using medium or low for a lot of tasks now and only using high or anything above that when it's like really, really necessary because that has a big impact on it as well.

01:51:00.000 --> 01:51:15.000
Another question here, what was the prompt to deliver the static grid that we showed? You literally just say that. Like, again, everything that I've, showed you here today, nothing was built from an elaborate

01:51:15.000 --> 01:51:39.000
multi-paragraph prompt. I literally just voice-dictated and said exactly what I want. So I literally just said, go and create these ads, deliver it to me as a HTML doc or an artifact in a grid style, and then if you wanted to, you could say, with, a way for me to toggle between the original ad and the new ad and way for me to add feedback

01:51:39.000 --> 01:51:51.000
I would literally say that and I'd run that. No prompts from this. You can literally just explain with voice dictation exactly what you want, and it will go and build it.

01:51:51.000 --> 01:52:14.000
One person asked if Parker has a built-in system that logs every ad, test, diagnosis and learns automatically as I run them so it compounds over time. We don't. The main reason why is because we would love for you to just build that functionality because it's going to be different for everyone. It'd be really hard for us to have like an out-of-the-box solution of like

01:52:14.000 --> 01:52:29.000
This is exactly what you're going to be looking for to test, and that needs to then, you know, go into the learnings of our next batch. I'm telling you that it's not hard to set up inside a Cloud Code. If all you… like, like what I said before on the AB testing, is go inside of Claude Code

01:52:29.000 --> 01:52:48.000
Use Whisper flow or just the built-in mic and voice dictate exactly what you want. You can say, I want you to look through every single ad. These are the main tests and hypotheses that we have as an organization. I also want you to try and find new tests or hypotheses that we should be tracking as well.

01:52:48.000 --> 01:53:07.000
And every day, I want you to go and pull the Parker data, find any new ads that have been launched, and update the metrics of the ads that we are tracking within these tests. And, you know, give me a summary every week of what you are seeing or what are you learning around this.

01:53:07.000 --> 01:53:23.000
If you just do that, and I mean, you can ask for a visual format of that, a text-based, you know, like, straight to Slack, whatever it is, I'm telling you, it will not be that hard to set up, and then you can have it exactly how you want

01:53:23.000 --> 01:53:43.000
all Parker is then there for is the data to come in, you know, every day from the meta API and being able to go and validate with like other sources like customer reviews or competitor ads, or whatever. So yeah, go and build that in Claude code, because then it can be exactly how you want it, and not something that, like, we have to try to figure out

01:53:43.000 --> 01:53:48.000
How would this work for a brand that, you know, has

01:53:48.000 --> 01:53:58.000
is spending 10 million a month in ads versus this brand that's spending 10 grand, which is going to be totally… two totally different testing experiences.

01:53:58.000 --> 01:54:16.000
Questions about the recordings. They sometimes go out same day, sometimes the day after, depends how quickly we can turn it around. So it will be there by tomorrow, guaranteed. Not sure will be there by today, but it will be going onto YouTube and then eventually into Notion in the unlisted

01:54:16.000 --> 01:54:27.000
YouTube videos. And then Afanasi, sorry if I've got that name wrong, asks where should the Parker brain be in the folder structure? Let me briefly show you

01:54:27.000 --> 01:54:29.000
This

01:54:29.000 --> 01:54:34.000
This is the ad crate brain, like the actual one that we use

01:54:34.000 --> 01:54:38.000
We covered this briefly last week in the Thursday session

01:54:38.000 --> 01:54:53.000
Basically, every… so I've seen in your question here, you said, like, should I have Parker, then brand one, then brand two? The Parker brain in itself is like a template for you to then go and create your

01:54:53.000 --> 01:54:58.000
brand brain or your client brains. So every single one of these

01:54:58.000 --> 01:55:14.000
Or a Parker brain but like this is the Parker brain of 1440. This is the Parker brain for honey love. So all of these are actually Parker brains, which is like you take that GitHub repo and then you say, make this Parker brain for 1440. Make it the honey love, make it all of these clients

01:55:14.000 --> 01:55:31.000
So it's not like the Parker brain is one folder and then the client brains are separate folders, but more so the Parker brain template is what you use to build all of the client brain folders. And then we just have a folder outside of that called company for all of our other company things that are

01:55:31.000 --> 01:55:35.000
Specific context to, a client

01:55:35.000 --> 01:55:42.000
So that's how we've got it set up. Again, like, you can do it differently, but, like, the Parker brain is not a folder in itself.

01:55:42.000 --> 01:56:00.000
That you want to have in your brand brain. It's just how are you set up the… like, our recommendation and our template on how you can set up your brand brain, then you can add… you can edit on top of that

01:56:00.000 --> 01:56:04.000
Yes, there is a

01:56:04.000 --> 01:56:19.000
Oh, yeah, yeah, do you guys download client meeting transcripts and the repo? Each client… yeah, yeah, absolutely, as Jimmy said. I thought you were asking if this course is going to be turned into a repo, which it will be. But yeah, yeah, yeah. All the contacts that we need, remember domain context, travel context

01:56:19.000 --> 01:56:24.000
or tribal knowledge, as Jimmy covered in Session 1 or 2.

01:56:24.000 --> 01:56:38.000
I believe. Do we have a homie session? Yep, that's coming up on Tuesday with Manish, who is another one of the co-founders or founder here at Parker. That's going to be a good one. So make sure you're here for that. Next week is like non

01:56:38.000 --> 01:56:50.000
Strategy slash ad-specific use cases, like create a source in landing pages, maybe a bit of media buying time. In the final week, I don't know what I'm gonna do the final week yet. It's gonna be a kind of, like, putting it all together.

01:56:50.000 --> 01:57:00.000
Session or, like, whatever we haven't covered, I'll do for that. I know that my teaching style is a little different from Jimmy's, I'm just… I'm a little bit more frantic, and I just

01:57:00.000 --> 01:57:23.000
Go into Claude Covid, the whole thing or Codex and just screen share for the whole thing but hopefully it's still in a way that is digestible. So I'm going to kind of see where we are after week five and then I'll put together a scope for the final week.

01:57:23.000 --> 01:57:34.000
Okay. Couple more

01:57:34.000 --> 01:57:43.000
What do we want to hit? Can you explain the difference between Parker

01:57:43.000 --> 01:57:52.000
I'm assuming you mean difference between Park and other tools or using a different ad spy tool

01:57:52.000 --> 01:58:01.000
Yeah, so first of all, if you have the Parker brain installed everything inside, or not everything, but a lot of the stuff inside the Parker brain is built

01:58:01.000 --> 01:58:19.000
To work with the Parker MCP. So it's going to take a little bit of rewiring or quite a lot of rewiring, actually, if you want to use this with another ad spy tool or do it directly with Meta. What you get with Parker is you're going to get all the different data sources that we saw earlier. So if I just

01:58:19.000 --> 01:58:37.000
Super quickly ball them up again. A more extensive data sources less than you're going to get anywhere. So inside of here we have customer reviews, post purchase service, customer reviews that are brought in in real time. So you don't have to connect that MCP or API

01:58:37.000 --> 01:58:59.000
Add comments are brought in, we get more ad comments than at least anyone else that I've seen by quite a magnitude. Tiktok's brought in. Ad libraries, of course, millions of ads brought in from here, the discovery feed. Reddit, I don't think is accessible to you guys yet, but I'm not aware of anyone else who has read access. Some of our beta users have access to this now, and it's pretty cool.

01:58:59.000 --> 01:59:14.000
And then all of the ads here are going to be AI tagged. So they're going to be AI tagged, but with ad formats, awareness levels, all the stuff we spoke about earlier, and sorted by impressions, so you can pull that straight into core code. So, I mean, I'm not aware of another tool that has

01:59:14.000 --> 01:59:31.000
as many integrations as we do, and we're in the process of adding more as well, so it's just more extensive than you can get from elsewhere, or doing it manually yourself. And again, if you're using that Parker brain, I don't think that there's another tool out there that's come out with a recommended brain structure that you can

01:59:31.000 --> 01:59:46.000
that they've open sourced that you can use yourself, but that's built to work alongside the Parker MCP. It still will work if you don't use the Parker MCP, but just not as well as it would, if you do have the Parker MCP. So, that would be the reason to use Parker outside of,

01:59:46.000 --> 01:59:50.000
Well, instead of other tools. Is there anything I've missed, Jimmy

01:59:50.000 --> 02:00:10.000
No, I think that's pretty good. Fun fact, too, we are going to be coming out with an MCP only package. So if you don't necessarily want the brain or the desktop app or any of that, like you strictly just want kind of the ad spy functionalities, we are going to be coming out with a new pricing tier for that, which is much cheaper than

02:00:10.000 --> 02:00:21.000
the current pricing that you see on the website. So, if all you want is to pull in the data from Parker, we are coming out with that soon. So stay tuned. You guys will definitely be in the loop on it.

02:00:21.000 --> 02:00:37.000
Final question, Matti says Maggie says, how's it get on the Reddit beta? I would have to check if we need more slots. I have to check with Tana. If we can, Maggie, we'll get you access to that. I'm not sure what the state of play is. So we will

02:00:37.000 --> 02:00:45.000
Check, and if we can, we will. If not, it will be, I imagine, not too long until it's in your hands.

02:00:45.000 --> 02:00:50.000
Yeah. Awesome. Thank you so much, guys. Jimmy, anything else you want to hit before we wrap?

02:00:50.000 --> 02:01:04.000
I don't think so. This has been fun as always. Let us know if you guys have any questions. I'm always happy to hit you guys up. So make sure that you can email us however you can communicate with us

02:01:04.000 --> 02:01:21.000
Like, seriously, we love to hear feedback. We love to hear ideas on how we can make it better. We're always open to try to make these as valuable for you guys. So even if you like Alex's style more, whatever it might be, just hit us up, because, yeah, the remaining sessions we want to have as valuable as possible. But

02:01:21.000 --> 02:01:22.000
Yeah, thank you guys

02:01:22.000 --> 02:01:32.000
Okay, thank you guys. Tuesday session is going to be with Manish on Hermes. Make sure you're there. And next Thursday we're going to carry on with some more use case stuff for non-ads

02:01:32.000 --> 02:01:40.000
work. So thank you very much, have a great rest of your week, and we will see you next week.
```
