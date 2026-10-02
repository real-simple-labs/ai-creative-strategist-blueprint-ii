---
title: "Parker course — Bonus Session 2 transcript"
date: 2026-09-29
session: "Advanced agentic performance marketing with Andre Lunev and Ruslan"
source_type: "Uploaded VTT transcript"
source_file_name: "GMT20260929-160023_Recording.cc (1).vtt"
source_provenance: "File supplied directly by Alex"
---

# Parker course — Bonus Session 2 transcript

Verbatim caption export from the September 29, 2026 Parker course guest session. Captioning errors and timing are preserved.

Transcription artefacts noted for retrieval only: “Cloud Code,” “clock code,” and similar variants likely refer to Claude Code; “codes/codecs” to Codex; “Matta” to Meta; “Bright data” to Bright Data; “Whisper flow” to Wispr Flow; and “Tegra/Takra” to the guests' business or system name. The source has no speaker labels, and the second guest's surname is not recoverable from the captions. No corrections were made to the transcript body.

```vtt
 WEBVTT

00:00:09.000 --> 00:00:11.000
What's up, guys?

00:00:11.000 --> 00:00:13.000
Happy Tuesday.

00:00:13.000 --> 00:00:15.000
On Tuesday

00:00:15.000 --> 00:00:18.000
If you're American.

00:00:18.000 --> 00:00:23.000
Hope you've had a great weekend. Ready for another week

00:00:23.000 --> 00:00:27.000
I am now officially a Floridian

00:00:27.000 --> 00:00:28.000
I'm literally in my office, my

00:00:28.000 --> 00:00:29.000
office that

00:00:29.000 --> 00:00:37.000
signing today, that I actually might be getting with Jacob from HQ. So I'm super excited about that.

00:00:37.000 --> 00:00:41.000
Good day. Good day, Cindy. Today's gonna be a fun one, guys.

00:00:41.000 --> 00:00:58.000
We have someone who I have learned a lot from when it comes to AI and Agentic creative. Someone who is more advanced than Jimmy or I. And, you know, this session is going to be technical if you

00:00:58.000 --> 00:01:09.000
are more… like, if you are newer to this stuff, and this course was your first taste of working agentically in Cloud Code or Codex, just to pre-warn you, like, this stuff

00:01:09.000 --> 00:01:26.000
is going to get pretty advanced today. I went to go and watch a talk of this guy, in Greece at Greek out a few months ago, and I was sitting there like, whoa, I didn't even know some of this stuff was possible. He is gonna show you how he's pushing the limits

00:01:26.000 --> 00:01:30.000
With

00:01:30.000 --> 00:01:45.000
with his Agentic work, and some of the workflows he's built, you know, they are really, really impressive, to the point where, like, I question, you know, am I doing enough? Should I be building more, of my system in the way that he has set up his

00:01:45.000 --> 00:01:47.000
Stuff. So

00:01:47.000 --> 00:02:03.000
I assume they are in the room now. Andre and Ruthland. If you guys want to just raise your hands just so Melody can bring you up on stage, then we can get

00:02:03.000 --> 00:02:07.000
started

00:02:07.000 --> 00:02:11.000
Will we be in the terminal? It's a question for Andre.

00:02:11.000 --> 00:02:14.000
What's up, Kat?

00:02:14.000 --> 00:02:21.000
From what I remember from the talk, Andre did a lot of his work in the Claude Code desktop app.

00:02:21.000 --> 00:02:23.000
But we will see.

00:02:23.000 --> 00:02:27.000
Andre is here. What's up, guys?

00:02:27.000 --> 00:02:35.000
Hey, thank you for the warm intro. Like, I'm excited. All good. Russ is also here and thanks for having us.

00:02:35.000 --> 00:02:38.000
Yeah. Hey, Alex, how are you doing

00:02:38.000 --> 00:02:39.000
Good. How are you?

00:02:39.000 --> 00:02:54.000
Yeah, it's good, man, it's just been super busy today, but yeah, we'll try to do our best. Yeah, we just had, like, lots of calls before, and have some after, but we will try to, you know, collect push and initial share as much as we… as much as we can.

00:02:54.000 --> 00:03:10.000
Guys, Andre and Russ are absolute killers. Like I said, I've learned so much from them agentically, and this is going to be an advanced technical session where they're going to show you their entire process and how you can start to be more agentic work inside of Claude Code and Codex. Now, as always, if you have questions.

00:03:10.000 --> 00:03:30.000
Put them in the Q&A, and we will get to them at the end. Guys, if you want to answer questions from the chat as you go, feel free to. Otherwise, people normally put questions in the Q&A box, and we can just spend 10 or 15 minutes at the end, if we have the time going through them together. I imagine there will probably be a lot of questions, because I know there's a lot of sorts that you guys are going to share

00:03:30.000 --> 00:03:34.000
So without further ado, Andre and Russ, take it away.

00:03:34.000 --> 00:03:47.000
Okay, sounds good. I know that Andrey prepares a little bit of a presentation. I will show something like live as well, like on the Agentic stuff that we are running, but let's just start with Andre's slides and move on from there.

00:03:47.000 --> 00:03:55.000
All right, we positioned it like that. So it's right out of the oven. All right. And actually

00:03:55.000 --> 00:03:59.000
In the last second. So

00:03:59.000 --> 00:04:09.000
What's the hardest part in building the agents? So from my perspective, the hardest part is to breaking down the

00:04:09.000 --> 00:04:24.000
process in place and then orchestrating the agent so that we could have the consistent output for each part of the process, right? So the attempts to make the one shot

00:04:24.000 --> 00:04:42.000
created from are designed to fail. Why? Because the creative itself is a very complex thing that has multiple layers. And we, me and Russ, even though we run a little bit different systems because I

00:04:42.000 --> 00:05:00.000
metam and Ruslan runs Google, the approach to the breakdown is very similar. So it all starts with the research, because we make the creative not out of the thin air. So we just dump the customer persona and tell the agent, all right, let's build this

00:05:00.000 --> 00:05:06.000
This kind of Pixar ad, Pixar style. Yeah, so it all starts with

00:05:06.000 --> 00:05:21.000
With a resource, right? And we can find out the code agent that has the web fetch tool that will mine the data through the APIs like Bright data, for example

00:05:21.000 --> 00:05:26.000
To mind the voice of the customer, right? The phrases that

00:05:26.000 --> 00:05:36.000
Your potential customers can say the YouTube comments, the Reddit comments, and so on and so on, right? And we have the huge, massive

00:05:36.000 --> 00:05:45.000
volume of data that is stored in some kind of a shape. Usually the shape is the JSON file or the MD file. So agents are

00:05:45.000 --> 00:05:50.000
Like this is the best way to

00:05:50.000 --> 00:05:57.000
To make the agent to consume the data, right? The the JSON file, then the Md file.

00:05:57.000 --> 00:06:11.000
At the end of the day, we have some kind of the deliverable that has some kind of a shape that has the fields, that has the phrase itself and so on and so on. So based on this thing

00:06:11.000 --> 00:06:17.000
We can feed it to the agent that is the underlying instruction

00:06:17.000 --> 00:06:24.000
instruction, right? So for example, based on the region, based on the voice mining, we can

00:06:24.000 --> 00:06:31.000
extract customer personas from from this volume of of the data right? And

00:06:31.000 --> 00:06:47.000
At the end of the day, after we feed, the result of the previous agent to the deeper one, to the persona mining agent, we can save this data as a JSON files. And this is how it trips down down the system, goes down the system

00:06:47.000 --> 00:06:55.000
Then, based on the customer persona and the voice of the customer persona, we can generate the angles.

00:06:55.000 --> 00:06:57.000
And

00:06:57.000 --> 00:07:10.000
Based on the angles, we can then generate the concepts and how, for example, we have the customer persona of the car owner, and we need to sell this customer persona

00:07:10.000 --> 00:07:15.000
The car coating, right? And the agent found in the

00:07:15.000 --> 00:07:25.000
Testimonials or in the research that, for example, this coating consists of graphene, which is the material that was designed by NASA

00:07:25.000 --> 00:07:43.000
That is 20 times harder than steel, right? So the angle becomes the hardest material on Earth, and then we can unwrap this kind of thing into a script, and the script also, it, like, doesn't come out of the thin gear. We have

00:07:43.000 --> 00:07:55.000
Around 50 templates, 50 MD files that have a certain structure, right? So it has the hook, it has the lead, it has the body part, which is… which consists of multiple layers

00:07:55.000 --> 00:07:56.000
And

00:07:56.000 --> 00:08:07.000
Then I will be slightly moving to the presentation itself, because I've already explained the concept of the files traveling down the system, and

00:08:07.000 --> 00:08:12.000
The concept is that we

00:08:12.000 --> 00:08:28.000
Maximally have to avoid the repeating actions on one entity. So what it means for us, we don't want to repeat our job every time we start working with the same client. So all the data is being stored on the local computer

00:08:28.000 --> 00:08:30.000
Right? So

00:08:30.000 --> 00:08:40.000
Nothing is in the cloud, we are using Cloud Code for this, and Claude Code operates naturally with the files on your local computer.

00:08:40.000 --> 00:08:46.000
So let's go

00:08:46.000 --> 00:08:55.000
Let's break down the stages of how agents solve the problems in general. So we have the objective and problem that we

00:08:55.000 --> 00:09:04.000
need to solve. So, for example, let's come up with one hundreds of creators. Then the agents try to understand to break down

00:09:04.000 --> 00:09:10.000
this problem into how, like, what are the steps to

00:09:10.000 --> 00:09:17.000
making this kind of creative, and it understands like it has the instruction in the system that

00:09:17.000 --> 00:09:27.000
We need to first read this file, make this kind of actions, then write the script, then animate it, then

00:09:27.000 --> 00:09:30.000
Voice over it and

00:09:30.000 --> 00:09:38.000
Then glue everything together. So how it looks in the system itself. So

00:09:38.000 --> 00:09:42.000
Alex mentioned that we are

00:09:42.000 --> 00:09:48.000
Doing a ton of technical stuff. And let me show you what I'm actually talking about

00:09:48.000 --> 00:09:53.000
So we are talking about the skills.

00:09:53.000 --> 00:09:58.000
And let me open some of those just a sec

00:09:58.000 --> 00:10:01.000
Ross, in the meantime, maybe you will

00:10:01.000 --> 00:10:05.000
Jump in

00:10:05.000 --> 00:10:17.000
No, of course. I mean, like, I try to engage, you know, people in the comments as well. You know, I'll just drop, you know, the message in here. Just feel free to ask any questions like while you, Andre, you know, just, you know, kind of like present

00:10:17.000 --> 00:10:24.000
We'll just do a little bit of a Q&A in the chat as well.

00:10:24.000 --> 00:10:25.000
All right.

00:10:25.000 --> 00:10:30.000
Guys, while those come through, guys, I'm just curious, can you guys, like

00:10:30.000 --> 00:10:45.000
paint the picture for everyone here. When you implement a system that you guys have implemented, I mean, from what I understand, it is fully Agentic is creating you, you know, hundreds of ads, thousands of ads a week

00:10:45.000 --> 00:10:59.000
What has that meant for your business and your clients? Like, what material has that done for you in terms of the results you've been able to get, or the amount of ads you've been able to produce, or the amount of time that you've spent on making creative?

00:10:59.000 --> 00:11:16.000
Yeah, I can ask this one. So just to give you a little bit of backstory and also like a little bit about us with Andre is that we are, you know, in the marketing in online advertising since 2017. So we joined our forces in 2020. Before that, we were working separately

00:11:16.000 --> 00:11:32.000
And at some point in 2022, 2023, we were 40 people team. So we are essentially a performance marketing team. We're working with, you know, big brands, small brands, we work with some big ones like Onet, Goalie. We work also with smaller brands too

00:11:32.000 --> 00:11:52.000
They're just getting started, so essentially, and our bread and butter is e-commerce. So we're doing a little bit of lead gen, but majorly, it's just e-commerce. So the brands are coming to us just to Andrea, someone is asking to open the seven step slide, please. So

00:11:52.000 --> 00:12:22.000
So essentially what we're doing is that the brands are coming to us and they want to get better return ad spend. They want us to run the Google ads and Meta ads. So we were 40 people in 2023, and we started to do like that was like when ChatGPT 3.5, I remember that moment, like when ChatGPT 3.5 was there. And I was like, okay, so maybe we can use like this and just automate some of this stuff. And I remember like I tried to write the titles and descriptions for shopping listings, you know, back then. So it wasn't like

00:12:22.000 --> 00:12:39.000
non-agentic or something. It was just chat back and forth, local files I was sending to the chat, I was getting back, you know, like, the optimized titles and descriptions based on whatever, you know, ChatGPT I fitted to ChatGPT. And since then, we started to, okay, so this is cool

00:12:39.000 --> 00:12:55.000
Then Cursor came out and I have the development background. Andre is PhD in math and also had, you know, prior marketing, a lot of experience in development. And we were like, okay, so, like, cursor, this is pretty cool. This is, like, looks more like the Agentic

00:12:55.000 --> 00:13:09.000
You know, collect system, there is a file system, you know, the file stores are stored in the in the on the local machine, and we can ask, you know, the agents to do, you know, some stuff. So it was no clock code, you know, back then, and so on.

00:13:09.000 --> 00:13:37.000
So, and it started to become, like, more agentic, so we started to automate some of the things. Okay, so the copywriting, just a little bit here, you know, just storing the results a little bit here. Then we started to connect Meta and Google through the Api. Okay, so we can do stuff now directly from agents to the account. So we don't have to do it manually. So and by doing like this, you know, little by little, we kind of like eliminated

00:13:37.000 --> 00:13:53.000
At first, some of the manual stuff we had to do, for example, we've had a couple of people in our team who were explicitly were doing uploading the new ads and the new campaigns into meta account. And then we had… so it was, like, way before, you know, it was

00:13:53.000 --> 00:14:13.000
Popular, like, on Twitter, and people started to build, like, the specific, you know, tools for uploading, you know, in Agentic mode. And the same for Google. I mean, right now we are, you know, like, we spend maybe, like, 5% of the time in the actual ad account, and 95% of the time in the terminal with clock code and codecs

00:14:13.000 --> 00:14:41.000
So essentially we started to eliminate, you know, like people, you know, like the tasks inside that were repetitive and not interesting. So like uploading of this stuff, you know, managing of the campaigns, checking the budgets and so on and so forth. And then the credit work. Obviously, we were doing already a lot of creative work, but the models were becoming better and better in the copywriting. And then, you know, there was this nana banana moment when the first one came out when, oh, wow.

00:14:41.000 --> 00:15:04.000
Like you can now actually print some static creatives that are actually pretty decent, you know, and they, you know, we started to play with it, combine it with the copywriting skills that our agents could do at that moment, which were relying a lot still on the on the skills that you're building or commands like back then

00:15:04.000 --> 00:15:32.000
So then the copywriting colleague. Okay, so the copywriting, now the agents can do copywriting really well, and now they can do the image printing really well, and then the models for video generation started to become, you know, better, but it was still, like, you need to generate, like, the separate pieces, and then you need to stick them together, you need to have editors in place to actually, you know, produce somehow, you know, good looking video creative, even though some portions of that video creative were AI generated and some of

00:15:32.000 --> 00:15:52.000
Those were real shots, for example. And now, you know, like with the video generation in Andrea will show like some of the examples, what he's doing is that like you can, and you guys also, you know, learn this from Alex too, is that like how you can actually end to end to produce like really nice video creatives and you don't need even editors in place quite often just to

00:15:52.000 --> 00:15:54.000
Just to do that

00:15:54.000 --> 00:16:09.000
And we shrink. So from 40 people in 2023, now we're just 3 people, 3 person team. It's me on Google. Andre is on Matta, and we have Alex, who's working on the retention side of things on email and SMS for the brands that we work with.

00:16:09.000 --> 00:16:24.000
And if we would compare, like, the output, like, how much we do right now, being three person people compared to 40, I think we do, like, maybe 5 or 10 times more than how much we were doing when we were 40, and everything was manual.

00:16:24.000 --> 00:16:43.000
So that's kind of like how much of a difference it made, you know, as the company for us and personally, like, to be honest, like, I never been like a big fan of just managing a lot of people. I remember it was a nightmare when we had like almost 40 people to manage with Andre, all of these sync, you know, calls and everything

00:16:43.000 --> 00:17:08.000
Now it's just awesome. Like, I'm running, you know, 20, 30 agents, you know, clock out sessions, codec sessions at the same time. Andre is running the same thing, and Alex is doing the same on email SMS, and our output is, like, 10 times more compared to 40 people team. And we don't have to hop on a call every time, because you just explain, you just open your whisper flow, and you just talk with the agents and they execute everything, and everything is kind of like

00:17:08.000 --> 00:17:27.000
They're, like, the agents are learning and you accumulate all of the data inside what's working, what's not working. The agents start to understand better, like how you work, how you do things. So we collect the proper Agentic setup where, you know, everything is stored for every brand for all of these skills are in place, etc. So it's been, you know, personally dramatic change

00:17:27.000 --> 00:17:48.000
And it's been, you know, for the company, also dramatic change how we operate and how pleasant, you know, and how much fun we have, you know, with the marketing now compared to the management hell that we've had previously. And now the output, you know, answering the question in regards to the output, I mean, for the statics, it's just an enormous amount. Like for some of the brands where we have, you know.

00:17:48.000 --> 00:17:54.000
quite significant budgets to spend. I mean, we launch sometimes thousands of the credits per week

00:17:54.000 --> 00:18:17.000
Because we can print that that much. And it's not just the same thing, and I will show you, like, what kind of tools we're using just to get the real, like, verbatim and real world data, like what these creatives are printed based on. So it's not like just AI agent is imagining, oh, this will be cool to launch. This will be good way for us to sell this product and so on. But how we can get like real world data

00:18:17.000 --> 00:18:32.000
and give all of this array of the data to the agents to analyze, find some commonalities, what's working, what's, you know, how people speak about the problems that they have with this product, how people speak good about this product. And based on this, you know, do the copywriting, then do the printing of the image ads

00:18:32.000 --> 00:18:51.000
And for video ads, I know that Android is launching, I'm not launching that much of the videos on Google. Quite often they just take like what Andre is making because he's doing some better stuff. I'm Google is a little bit different, like from that perspective, there are other placements that need a little bit separate attention, not necessarily just video printing

00:18:51.000 --> 00:19:16.000
But, you know, it can be hundreds of the videos per week as well per brand. So overall, like our output probably, you know, we measured it once in a while. There are some months where we, you know, we do like 20,000, 30,000 credits plus per month of the aesthetics and thousands and thousands of the videos of

00:19:16.000 --> 00:19:20.000
Per month of video credits.

00:19:20.000 --> 00:19:21.000
Yeah, someone is asking

00:19:21.000 --> 00:19:29.000
So you guys see… you guys can see why I wanted to get Russ and Andre on like we spoke about the idea of a one-person creative team

00:19:29.000 --> 00:19:33.000
last week, like, they are the embodiment of that, and they are, like.

00:19:33.000 --> 00:19:39.000
What you can do if you push to the max, like, that is a level of

00:19:39.000 --> 00:19:54.000
Automation that I have not got to and makes me feel quite uncomfortable, to be honest. But like it's so I find it so interesting to learn from them like what happens if you if you really do go all out with this process. So I'm so curious guys to hear exactly how you built

00:19:54.000 --> 00:20:13.000
Yeah, but it's just like we just, you know, build out the processes from, you know, for everything that we're doing. And essentially to keep up, you know, to get there right now is so much easier compared to how much time it like how much harder it was like two years ago, one year ago with the models that are available right now

00:20:13.000 --> 00:20:28.000
You just need to, like, essentially, like, I'm as a developer, I just understand, like, everything that has the API and everything that you can pretty much imagine, like, digital, can be done by AI at this point. It's just a matter of the tokens. And I see this, there is a question how you

00:20:28.000 --> 00:20:44.000
Do you keep control over costs? I mean, it's not really hard. I mean, we're running, you know, I'm running for clock code subscriptions. So it's $800. I run two codec subscriptions. It's another $400. I run one Grok

00:20:44.000 --> 00:21:00.000
Which is $300, and all of the rest is the API cost that we're using Kai, and for printing, or OpenAI directly for printing the statics, because we're using GPT image 1.5

00:21:00.000 --> 00:21:15.000
And now, GPT image 2 and 2.5, it just recently released, and I will tell you a little bit of, I don't know if I should, you know, tell that hack, but maybe I will, you know, in regards to the subscription, maybe some folks already understood what I mean

00:21:15.000 --> 00:21:20.000
But for the image printing and for video printing, we primarily using chi

00:21:20.000 --> 00:21:37.000
And for limiting our costs, we know, like, because we paid by performance, by the ad spend that we're doing. So we do not kind of like limit ourselves in regards to the spend on these things, because we know it will pay out.

00:21:37.000 --> 00:21:57.000
Like we print lots of the queries, we find what's working, what's pending with the big caps, what's spending on Google, etc. We know that it's, like, the brands that we work with will make more money with it. We will make also money with it. So we kind of, like, do not limit that part.

00:21:57.000 --> 00:22:08.000
But in regards to the hard cost, like in the subscriptions, it's not that much, it's like $1,000, maybe $2,000, you know, to operate all of that, and you can work with, I don't know, like, 15 brands, and that's

00:22:08.000 --> 00:22:27.000
very much enough, especially, you know, with the recent models. I know that, you know, like with when Fable came out, like it was eating the limits really fast. Astra is eating limits like super fast, but now Opus 5.5 released, so it's kind of like I have hard times actually to spend all of the weekly limits

00:22:27.000 --> 00:22:34.000
And with the GPT-6 SO as well, so it's super efficient too.

00:22:34.000 --> 00:22:49.000
Yeah, another question was regarding what is an MD file. It's basically the markdown. MD comes from Markdown. It's a text file. And for example, here is how angle looks like as an MD file. This file was generated by

00:22:49.000 --> 00:23:06.000
The agent by the call, like, based on the product that I passed to the to the agent, and based on the product description. For example, this one, we have the certain templates of how we think about angles and how we think about

00:23:06.000 --> 00:23:20.000
finding the customer personas, like this is the internal process, but the outcome, I can surely show. So, for example, angle is called angle 42 watch water bid off, right? Information go up

00:23:20.000 --> 00:23:35.000
Plus superlative credibility right? So who is that for segment that status linear the system set this up afterwards after some span right? And it has the big idea

00:23:35.000 --> 00:23:49.000
Like coating your car with the hardest control creates an information gap so powerful that you must watch to see what happens. What happens to your car when you coat your car with the hardest material on Earth? So, basically, this is the show, don't tell

00:23:49.000 --> 00:24:01.000
Thing, right? And we also have the mechanism in the angle so that we could deliver this mechanism downstream in the video. And what can

00:24:01.000 --> 00:24:02.000
come after

00:24:02.000 --> 00:24:13.000
the angle. After the angle, we can write down the script, and let me show you the how how the final creatives may

00:24:13.000 --> 00:24:19.000
may look like just a sec. Here we go.

00:24:19.000 --> 00:24:29.000
So all of the folders here generated by the by the AI. So I will show you the latest creators on this angle, right?

00:24:29.000 --> 00:24:37.000
Let me play this one. This is the Yapper ad, which is made in one shot by the sequence of agents

00:24:37.000 --> 00:24:48.000
If your car lives outside, give it the hardest material on Earth before anything else. It costs about as much as a tank of gas. Look, how many Saturdays a year does your car get?

00:24:48.000 --> 00:24:57.000
Ours used to get every single one of my husbands, and by Wednesday, it looked like he never touched it. So when he came home with the hardest material on Earth.

00:24:57.000 --> 00:25:09.000
I went out to watch. He poured a whole jug of water across the hood, and it did not spread. It pulled into beads and rolled straight off the paint. Dirt slid off like it had nowhere to hold on. The coating is resist

00:25:09.000 --> 00:25:14.000
So, yeah, these are all one-shots, and you see 100 of those

00:25:14.000 --> 00:25:17.000
were generated in just

00:25:17.000 --> 00:25:33.000
One day, in 20, 30 minutes. So how do we approach this kind of forum? Like, first of all, it's the modular approach, right? So we have the hook, lead, and the body part. Hook is the first 3 seconds of the video lead is the part that is coming right after the hook

00:25:33.000 --> 00:25:39.000
And the body part is the explainer part with its own argument and so on and so on. So when we have 10 hooks

00:25:39.000 --> 00:25:49.000
10 leads on one body part, we can mix and match, basically multiply 10 hooks by 10 leads, and we can have 100 creatives in here. So, for example, hook 10, lead 10, or

00:25:49.000 --> 00:25:54.000
Lead 7, right?

00:25:54.000 --> 00:26:10.000
Washing your car every single weekend is a waste of a good Saturday. I have told my husband that a hundred times. Have you… So, but this creative doesn't come out of the thin air. So the entire folder is the sequence that is produced

00:26:10.000 --> 00:26:12.000
produced by the

00:26:12.000 --> 00:26:28.000
Agentic flow. So, one agent does the script, right? So it wrote the script and writes it down into this kind of a document. So, Yapr matrix, blah blah blah. So, the script, belief ledger protecting the paint, ordinary coatings promised the protection, so we have the skeleton of the ad

00:26:28.000 --> 00:26:34.000
And the agent came up with following the certain structure. Then it has the

00:26:34.000 --> 00:26:51.000
hooks that were written, then the leads. Then the type repeats and so on and so on pictures. So you saw the overlays, and it also comes up with the overlays that you saw on the video

00:26:51.000 --> 00:27:01.000
Then it goes to kai.ai and animates. So each scene is the animated thing, right? Animated short clip

00:27:01.000 --> 00:27:19.000
It is $59.99 for a bottle that covers three or four cars and right now it is buy two, get one free. Tap below and get resist. So this is the short clip that we afterwards glue together. So how do we come with the overlays?

00:27:19.000 --> 00:27:31.000
We have a certain procedure for that that generates first the JSON files with a description that goes to the GPT image tool with a short, very short

00:27:31.000 --> 00:27:45.000
description was of what needs to be depicted in the image. So, for example, phone photo of dozens of dried white hardwater spot rings covering a dark blue car hood in low sun. And it comes with the catchy

00:27:45.000 --> 00:27:51.000
images, right, that we overlay on top of the video, depicting the husband, the problem

00:27:51.000 --> 00:27:53.000
The sport

00:27:53.000 --> 00:27:55.000
So there are certain types of those.

00:27:55.000 --> 00:28:11.000
overlays, and then we just by using FFmpeg library, which cloud code knows, we bake it in. But it all starts with the script, then we generate the character, then we pass the character to the model animated based on the script

00:28:11.000 --> 00:28:17.000
Then make overlays, then, glue things together, and then caption.

00:28:17.000 --> 00:28:22.000
Any questions on that?

00:28:22.000 --> 00:28:39.000
I think there are quite a few. So I want to kind of cover what has been spoke about in the chat. I think one question, a very natural question that came up, I know at Greek out as well, Andre, and I've seen in chat in the chat a couple of times

00:28:39.000 --> 00:28:43.000
is you guys are doing so much volume

00:28:43.000 --> 00:28:44.000
Yeah.

00:28:44.000 --> 00:28:56.000
With AI, static and video, how like, how does that change how you structure an account when you're uploading this much volume and how do you do that

00:28:56.000 --> 00:29:03.000
Like, have you had any issues with being banned or upload limits with you uploading this much volume

00:29:03.000 --> 00:29:11.000
Yeah, that's a very interesting topic. So, you know, I'm the bid cap maxi and I can touch base

00:29:11.000 --> 00:29:18.000
touch base on the media buying side of the creative webinar. So, the thing is that

00:29:18.000 --> 00:29:33.000
We need to first understand before we dive into the media buying part, we need to understand what we actually pay Meta for, right? So we don't pay for sales. We don't pay for clicks. We pay for impressions. It's basically like your renter

00:29:33.000 --> 00:29:42.000
banner on the street, or show the banner to the crowd, right? And our goal as advertisers is to show the banner to the crowd

00:29:42.000 --> 00:29:57.000
Imagine you are standing on stations showing the banner to the crowd of 1,000 people, and our goal is to make the banners that will raise the hands of the potential customer. And here's the example. Imagine you have the Zipo lighter that you need to sell to a crowd

00:29:57.000 --> 00:30:13.000
Right? And you can position Zippo like a source of fire, for example, or source of fire for fishermen and for hunters or for smokers, or as a gift for the boss. And imagine you raise the banner in front of the crowd and say, okay, this Zippo lighter is for fisherman

00:30:13.000 --> 00:30:16.000
And you will raise five hands

00:30:16.000 --> 00:30:18.000
Or you will

00:30:18.000 --> 00:30:34.000
show the same manner, but say, like, this is the like 400 or for gift for the boss. So the thing is, there will be more hunters hands or fisherman hands that than those who need a gift for the boss, right?

00:30:34.000 --> 00:30:51.000
and the the point is that not every creative deserves the spend. So what's the what's the point showing the banner to that raises less hands compared to the banner that shows that raises more hands

00:30:51.000 --> 00:31:00.000
And with the automatic bidding, which is the classical media buying approach, like highest volume, lowest cost

00:31:00.000 --> 00:31:16.000
Basically, the goal of this campaign is to spend the full budget and then to deliver as many impressions as possible, always treat the efficiency goal. What it means for us, it means that if you use the classical highest volume media buying and showing the gift to the boss

00:31:16.000 --> 00:31:22.000
creative to the crowd, it will spend the full budget, but still the amount of hands that will be raised

00:31:22.000 --> 00:31:27.000
will be lower. That's why we use bid caps. Bitcaps

00:31:27.000 --> 00:31:32.000
is the bidding strategy that acts in the same lowest-cost auction

00:31:32.000 --> 00:31:34.000
And

00:31:34.000 --> 00:31:43.000
Bitcaps restricts limits the amount of impressions that we deliver to the crowd depending on the

00:31:43.000 --> 00:31:59.000
probability of the conversion. So, based on the creative, Meta can easily understand, alright, so there is a certain amount of fishermen, or the people that will react to this creative, with a certain probability, based on the CPM, CTR, and expected conversion rate

00:31:59.000 --> 00:32:04.000
Three metrics. We already remember that we pay Meta for the impressions, right?

00:32:04.000 --> 00:32:07.000
And Matt is smart enough

00:32:07.000 --> 00:32:25.000
To understand whether people click on this creative or not after a small amount of impressions, like 300, 500. And if the CTR is low, it means that people don't click on that, that the crowd is not there. So if the CTR is low, it means that our cost per click is high

00:32:25.000 --> 00:32:29.000
And Meta also knows the

00:32:29.000 --> 00:32:44.000
Conversion rate of the page, and it understands easily. So with this Ctr that leads to this CPC, with this conversion rate, will it be able to get us the conversions at or under the desired cost or above

00:32:44.000 --> 00:32:59.000
If it can project that this creative will deliver us conversions at or under the desired cost, the spend will be there. If not, so if the CTR is low and the projected CPA is higher, then your bid

00:32:59.000 --> 00:33:16.000
It will suppress the delivery. So what it means for us, we can print infinite amount of creatives with AI, and we test them literally risk free with bid caps, right? So infinite amount of creatives multiplied by

00:33:16.000 --> 00:33:33.000
bidding strategy that just eliminates the risk is the core of our media buying approach. And then, like, how we look into the into the scaling campaigns. Here's this is the visualization of our

00:33:33.000 --> 00:33:49.000
entire strategy. So this is the data visualized by the metrics that we get back from Meta into our system. And let me show you really really quick what I mean here

00:33:49.000 --> 00:34:00.000
So when we talk about the customer personas like Zippo lighter for smokers, Zippo lighter for fishermen, we talk about the angles, right? So broader strokes

00:34:00.000 --> 00:34:06.000
broader strokes, bigger strokes. And here's how we look at the angle. So we have

00:34:06.000 --> 00:34:22.000
Ethoscar here, right? And we have the certain amount of angles. Angle 42 hardest materials, hardest material on Earth, or this one winter defense. Some of the angles have more spend than the others. So, for example, angle 41, it

00:34:22.000 --> 00:34:28.000
It has protection in 15 minutes or angle 21, clip off

00:34:28.000 --> 00:34:44.000
1200 reports and never again. So it is the comparison to the detailing center that charges 1200 for the detailer. And we see that different angles have their own

00:34:44.000 --> 00:35:00.000
spend, which is the circle size, right? And they have their different profitability. So, for example, angle 21, we can unwrap that into videos and into the creative sets, or angle 42 we can unwrap

00:35:00.000 --> 00:35:16.000
into the videos and the concepts. And all of this is just coming from the data which is stored in the JSON files. And that's why we structure the account based on the angles, and the angles are based on the customer personas, right

00:35:16.000 --> 00:35:18.000
So

00:35:18.000 --> 00:35:20.000
Once we understand

00:35:20.000 --> 00:35:29.000
which customary personas and which angles get better feedback instantly, we started to, like.

00:35:29.000 --> 00:35:45.000
to use this kind of a fractal approach, double down on something that is working and avoiding something that is not working. And again, when we analyze the account with the agents, so we have multiple lenses that the agent can look through

00:35:45.000 --> 00:36:01.000
So all of this data is being prepared deterministically, right? And we can even look at this angle worked better with this hook or angle 21 works better with this kind of hook. So this is another slice of the data which our agents are using

00:36:01.000 --> 00:36:12.000
for the analysis. So this is how we approach the analytics, and when the agent… when the Agentic systems writes down the next script, it will 70%

00:36:12.000 --> 00:36:27.000
Of the cases follow something that is working already, something that is proven in the ad account and 30%. Something that we didn't test yet. So we have the this kind of fog

00:36:27.000 --> 00:36:43.000
4 area, the unknown area that we didn't test yet. And we can clearly see this into the in the picture. So we have around 100 angles, and we can come up with a new angles, no knowing something that we didn't test

00:36:43.000 --> 00:36:50.000
yet at all. So, like, did I answer how do we approach the media buying part and the scaling part

00:36:50.000 --> 00:37:05.000
Yeah, I mean, I think this is a really interesting approach to it, and something that, like, we've definitely not considered as much volume as you guys, but, like, I'm curious to have a look into this more and have some conversations with people.

00:37:05.000 --> 00:37:07.000
Guys.

00:37:07.000 --> 00:37:24.000
Let's just say that someone is sitting here watching this and they're going, wow, like this looks great. I love the idea of using AI to make hundreds of thousands of assets for me every week and launch them into my ad account, but they are, you know, they're a Claude Code user

00:37:24.000 --> 00:37:38.000
But they're not, you know, anywhere near, like, the level that of building something like this. Where would they start if they're like, this looks really cool, but I have no idea how to even start building something like the system that you're showing?

00:37:38.000 --> 00:37:41.000
I will start with

00:37:41.000 --> 00:37:44.000
Repetitive tasks. So, for example.

00:37:44.000 --> 00:37:48.000
You open cloud code right? And

00:37:48.000 --> 00:37:51.000
You can

00:37:51.000 --> 00:37:54.000
ask it something like

00:37:54.000 --> 00:37:59.000
19% of the limit.

00:37:59.000 --> 00:38:03.000
Cross, what do we start with? I think like

00:38:03.000 --> 00:38:07.000
Fine

00:38:07.000 --> 00:38:08.000
All right

00:38:08.000 --> 00:38:11.000
I mean, like, I can't tell you like what I would do like if I would just rebuild like the same system, you know, right now, if you allow me to share, you know, my screen

00:38:11.000 --> 00:38:13.000
Yeah, yeah, you will

00:38:13.000 --> 00:38:30.000
Real quick. So, actually, like, to build a system like this, you know, now is just so much easier compared to when we started to build it. Means that… because, like, the model is so much fa… like, they don't need that much of a hand-holding how much they were needed before

00:38:30.000 --> 00:38:52.000
It just really simple. Like, as soon as Okay, so you want to work like on the meta ads, like basic stuff. Like we need to create the folder where we are going to work with all of this stuff. So essentially, you know, like all of my Agentic system, which is kind of like a lot of stuff here, this is just only commands

00:38:52.000 --> 00:39:14.000
And also, like, for the brands and everything, there's so much stuff. So essentially, just a folder. Then we opening the cloud code session, and instead of clock… so I don't know, guys, maybe, like, it's super basic, maybe, like, that's not what you wanted. But, you know, kind of like, I just, you know, start the clock code, open the terminal, like, just one of the things, like, really important is that guys, just, you know.

00:39:14.000 --> 00:39:29.000
terminal. So no, like, there is there is the app. Yeah, it's somehow good, but it's like still a super basic compared to, you know, just do, like, the, the capabilities that Cloud Code or Codex has

00:39:29.000 --> 00:39:53.000
inside of the terminal. And it's not complicated. It's just opening the terminal and typing in CAIC code, and Claude, and that's it. Or you can use this, you know, CMUX, which is like a collect multiplexer for AI agents. It just makes things so much nicer. You can see all of your agents running and everything in here, and you can, you know, you can create the taps in here for different projects that you work on and so on and so forth

00:39:53.000 --> 00:40:21.000
And then inside, so this will be just an empty folder, and you just start kind of, like, just talking to it. You just, you know, just turn on Whisper flow and start talking to it like what you tried to achieve. And that's it. So essentially, like, think about it, like, from the architecture perspective. So what you want to do, like, inside this project, you want to manage your meta ads. Okay, so just tell it. Okay, so what I want to do here, I want to manage the meta ads. I want to, you know, be able to upload the

00:40:21.000 --> 00:40:23.000
my

00:40:23.000 --> 00:40:42.000
you know, campaigns to the meta directly without touching the interface. I want to work on the credits, so I want to do the static credits and video creatives, so I need the, you know, to connect to something that will allow me to do that. I want to do, like, really strong copywriting in here

00:40:42.000 --> 00:41:09.000
for the ads that I'm going to launch. I want to maybe, if you want to do this, like, I want to build the landing pages as well, so not only the creatives, but also the landing pages, the editorials and listicles. So try to kind of like, like, because, like, folks, kind of just making it super complicated, like, oh, like, there's this, you know, huge, prompt, copy and paste it, and you will get this and so on. Like, just try to talk to the agent and explain like in the simple words you what you're trying to achieve, not type because like that's

00:41:09.000 --> 00:41:25.000
Like limiting yourself to collect picking the words instead of just talk. Like, sometimes I check… when I build something new, I just sit and talk to it, like, for 5 minutes, and I mean, let me show you something. So this is my

00:41:25.000 --> 00:41:28.000
What is that? Like, the insights. So that's my whisper flow

00:41:28.000 --> 00:41:40.000
So I'm not bullshitting you. I mean, I'm speaking fast. I'm dictating lots of stuff. I wrote like 16 complete books with it. And as you can see, most of it is

00:41:40.000 --> 00:41:42.000
Cloud Code

00:41:42.000 --> 00:41:47.000
So, and I do it almost daily. You see?

00:41:47.000 --> 00:41:56.000
Just lots of the days talking to the agents. So, and this is, yeah, this is… this is like with where it started, actually, with the whisper flow.

00:41:56.000 --> 00:42:21.000
So essentially just talking to it. So now, okay, so you talk to it and then, you know, just to so you understand the concept is that like how this thing is working. So private prior, like you had to kind of hold the agent and you need to collect like you need it to, you know, build the instructions which kind of like repetitive, like, oh, don't forget to check this, don't forget to check that, don't forget and do this this way, do this, this, that way, etc. So now the agents are so much

00:42:21.000 --> 00:42:50.000
Smarter. So therefore, the skills are so much more simpler, and you don't need to, you know, build or still. And also, like, this is another thing is that, like, there are some good skills out there, but take them, but do not just inject them blindly, just feed it, like, for example, download MD file, just drop it in here and ask the agent, like, okay, so just analyze this and see how it will compare and incorporate into my system. So as soon as you have some kind of system. So now, in regards to the building this system and ask it like this thing

00:42:50.000 --> 00:43:08.000
Like, okay, so if we're building this system, how we will just convert like all of this that I just told you, like for five minutes into the skills that will be easier for us and easy for you to work with so you know like the process inside. And that's how you build this stuff, you know, something like this. So essentially, and I will try to not to

00:43:08.000 --> 00:43:36.000
Flash any API key or something in here. So this is like how my, you know, clock out. This is my… this is like the live, you know, system that I'm running. So these are the skills. So all of the skills… so these are built, like, for the past 3 years. Some of them I'm not using too much, some of them I'm using every day, and I'm and I will tell you like how to use the skills, etc, and why you don't have to remember all of them, but just to have like a little bit

00:43:36.000 --> 00:43:51.000
You know, kind of like rememberable or understandable structure and the naming for them. But like all the things brand related, all of these things, you know, creative generation, image, videos, refresh, render, etc. Then demand gen

00:43:51.000 --> 00:44:19.000
data for SEO research, then these are technical evaluations of the skills. The feed shopping feed related, you know, stuff. Hicksfield also integrated, because I got the subscription a while ago, and I'm like, okay, so I'm I paid for it, so I need to spend the credit. So I integrated it. So every month I just spend the credits. Well, I paid for a yearly plan. The meta ad stuff. This is like to pull something that is working for Andre already. So it's kind of like, okay, so I have also connection from my system to Meta

00:44:19.000 --> 00:44:43.000
And it can go and just analyze all the creatives for the past 30 days, 90 days, et cetera, and see what's performing for Andre. And I can bring it into Google and launch it inside of Demand Gen. Some other stuff. You know, this is the offer building stuff. So it's like research, then copywriting, then building, then deploying to Shopify, deploying to Cloudflare of the offer pages and the commands for optimization

00:44:43.000 --> 00:45:07.000
Then the Pmax related commands pre-sale page related commands, as you can see, you know, like, because the offer and the pre-sale page is the big part, especially on Google, where I'm testing lots of it, like the huge part of my system is, like, how we can build like really nice editorials and listicles and so on. Roasting, which is like, I will tell you, like, I responded in the questions, like in regards to this roasting sessions and panels

00:45:07.000 --> 00:45:23.000
In the Q&A session, there was the question in regards to this, or a little bit deeper into it. The search ad related, you know, the SEO. This is like when the page that we built, like, didn't work for paid, I would just promote it into SEO, and just to give some, you

00:45:23.000 --> 00:45:46.000
for the brand to get some, you know, free traffic in there, then, you know, spy tools, Taboola, I recently integrated Taboola here as well, and that's it. So these are, you know, the skills. So about 200. I don't remember every single one of them. I just name them, and I ask, like, when we create the skill, and you don't have to create them one by one. You can like again, just start with just dropping all of

00:45:46.000 --> 00:46:05.000
the stuff that you have in mind into the clock code, and asking how we will just distribute it among skills, and just ask it to build the skills. So it's kind of like you at least understand, like, which skill is, like, related to what, like, is it the demand gen? Is it creative, or etc. But I almost never, and you see, like, every skill kind of contains, you know, the skill itself

00:46:05.000 --> 00:46:21.000
And also, you know, this is the what's called progressive disclosure. So you don't have to dump like everything in one file. You can ask it to use the best practices for clock code, where it's doing the progressive disclosure, where it has like all of these phases, you know, in the separate files

00:46:21.000 --> 00:46:41.000
And I will try not to open it because I might just, you know, flash some API key inside or something. So that's it. And then so it builds you this scale. So it would be like maybe 10 skills or something in the beginning after you just drop this first message and then you will understand, okay, so, like, oh, okay, so for the credits, let's just try this creative skill

00:46:41.000 --> 00:47:00.000
And, you know, let's just build something and it will do some for you that doesn't work. And then you talk to it, and okay, so this is not good, this is better, and this is, like, you know, maybe, like, what we can improve, and here, maybe we can add, like, research phase now. Maybe, like, we… it's not for you, agent, just imagining, like, what will work, but maybe we'll

00:47:00.000 --> 00:47:09.000
give it to you a little bit of a body that you can from real world, you know, get some data, like what you're writing about, because what you're writing is bullshit

00:47:09.000 --> 00:47:34.000
So, and you just talk to it, man. That's just that's it. And then you open, like, another session in another session. So the thing about the skills and how it's done now, and how why it's super, you know, convenient to work with the Agentic systems, when I open something new, for example, I can open this session now, and I'm starting to work with the new brand. What I will do is just I would just say, okay, so we're onboarding this brand, the brand name is this

00:47:34.000 --> 00:47:48.000
The URL is, and I will pass, you know, the URL in here. I will provide, because they already shared access to the Google Ads Mcc that we have the ID of their Google Ad account and also their Google Merchant Center ID, etc

00:47:48.000 --> 00:48:03.000
And I don't need to invoke something like this, you know, like brand on board necessarily. And specifically doing something like this. Right now, the skills work in a way that they're kind of like your SOPs slash

00:48:03.000 --> 00:48:18.000
You know, processes in place, all of them have, like, their own descriptor that you… the agent that you will be talking to, like, inside of Clock Code or Codex, will understand what the skills to invoke

00:48:18.000 --> 00:48:47.000
from your… from whatever you have. So you can tell it, like, for example, here's the idea of the campaign, let's just take a look at that and analyze and optimize it, for example. And you don't have any skills for optimization. So it will do, it will try its best, like, to find… pull the data from meta API as soon as you have API connection, etc, and will pull like all of this data and will okay we'll do some optimization. You will tell it, okay, so just take a look at every single image ads, analyze it for the past

00:48:47.000 --> 00:49:08.000
30 days, 90 days, 180 days, and see the dynamic and also see compared to everything else, what's underperforming. I will pull all of the data and then you will do some other optimizations just talking to the agent, and then at the end, like, as soon as you've done that, you never had this optimization, you know, skill in place, you would ask it, okay, so now, like, what we've done today, let's just pack it into reusable scale

00:49:08.000 --> 00:49:17.000
and let's call it this or whatever. And now, you know, so we have this tool, you know, in our tool belt that we're going to do in the future.

00:49:17.000 --> 00:49:34.000
And that's it. And that's how, you know, kind of like these things is just growing and growing and growing. And at some point, you would just consolidate some things together. So it's easier, so you're not… don't have just repetitive, you know, similar kind of, like, skills in place

00:49:34.000 --> 00:49:49.000
Just once in a while, especially when the new model is coming out, I will just ask it, okay, so just go through all the skills that we have, see what's redundant now with the new… this new model that just came out, or let's consolidate something that we don

00:49:49.000 --> 00:50:18.000
We don't need like separate skills for it. We can just consolidate into less amount of the skills. And that's it. And then it grows. So there are lots of this stuff in here. Obviously, you know, built over years. And what I do now is that when I'm working with something, I just talk to it. It just invoke all these skills. As soon as we find some approaches that are better, like, for example, executed something we did something that we didn't do before, for example, in regards to optimizations, either it's me asked it to do

00:50:18.000 --> 00:50:28.000
Or it's the agent came up with something new, I will tell something. Okay, so let's just adjust our skills so we do this next time as well, like when we do this optimization flow, or we do launch something. And that's how it grows.

00:50:28.000 --> 00:50:38.000
One thing that I wanted to, you know, that I touched base on it to mention is that there was

00:50:38.000 --> 00:50:43.000
There was a question here for, let me see

00:50:43.000 --> 00:50:50.000
For the real world data and where we are getting

00:50:50.000 --> 00:50:52.000
I think it was in the chat.

00:50:52.000 --> 00:50:56.000
So in regards to, you know, where

00:50:56.000 --> 00:51:11.000
Oh yeah, this one. So what tools are you using to gather the real world data? So this is, like, very important, because you can ask the agent to do the copywriting, and now models are better at it, but what we found is that as soon as you provide, like, the best possible

00:51:11.000 --> 00:51:29.000
raw data from the real world, what people are saying when they talk about a product, why they like it, why they don't like it, you know, commentary, etc. It's better to just connect your project to some of this real-world, you know, data warehouse. I know lots of people using Apify. I honestly do not

00:51:29.000 --> 00:51:47.000
like Apify, I like, you know, Bright data. It's up to you actually which one to choose. I just find the API of Bright data so much more streamlined and convenient, and it's also super cheap. I think we're paying like $50 per month for something for all of the scraping, gathering that we're doing

00:51:47.000 --> 00:52:03.000
I will tell you, like, what I'm doing for Google Ads with Bright data. So I'm using the Trustpilot scraper. I'm using the Amazon listing every use scraper. I'm using Reddit scraper. I'm using sometimes YouTube video scraper. And

00:52:03.000 --> 00:52:15.000
That probably, especially at the Amazon listing reviews is very important. So the client that I'm working with, they're not necessarily maybe have the Amazon listing with lots of reviews, but their competitors have

00:52:15.000 --> 00:52:32.000
So what I ask it to do is that, okay, just go and find the competitors that are running on Amazon. But it also like does all of the other things too. But, you know, just do the competitor research like in my system, it's called VOC mining voice of the customer mining. There was

00:52:32.000 --> 00:52:34.000
The

00:52:34.000 --> 00:52:51.000
The, the skill for it. Yes, this one, brand PUC mining. So what this one will do, and again, like, I would love to show you, like, everything. I just want to make sure that there's no API keys everywhere, you know, just sprinkled. So what this one will do is just connect it to BrightData, and it will go to find the competitors

00:52:51.000 --> 00:53:07.000
And we'll pull all of the, you know, their Amazon listings reviews, Trustpilot reviews, you know, it will go to the Reddit relevant subreddits and parse some replies, etc. All of the verbatiming that are available for, you know, similar products

00:53:07.000 --> 00:53:22.000
or discussions about the similar products. And then we will save it, and you don't have to necessarily… this is, like, in regards to the questions about MD and JSON files, etc. You don't have to provide, like, the specific structure, how you structure your

00:53:22.000 --> 00:53:40.000
You know, your folder where your agents are working. The agents will find a way to just store it how it's convenient for them, either MD file, JSON file, you know, Json L file, whatever that will be the most convenient for them. So they will scrape all of that, and

00:53:40.000 --> 00:53:55.000
how I build that skill is that it will just go and parse through all of this data just to find what's repetitive in there, what people care about, what they say about how they like, and what they don't like, and take their exact verbatim angles, what kind of user personas told that

00:53:55.000 --> 00:54:14.000
And, you know, creative strategist can go just that much compared to how much of a data can be parsed through by the AI agents. So that's why I would I would just tell, you know, yes, human can do like good judgment, you know, when the job is done, for example, we can review the creatives and so on

00:54:14.000 --> 00:54:36.000
But sometimes, like, you cannot, you know, just go through and read, like, 10,000 reviews on Amazon listings, just to understand, like, what's what kind of angle to come up with. The agent can do that in a couple of minutes, and it can just summarize all of that and find what's repetitive, and just use that to craft the user personas and go specific

00:54:36.000 --> 00:54:42.000
For your headline descriptions, for your copy on the image creatives, and so on and so forth.

00:54:42.000 --> 00:54:54.000
So this is where you know we're using. We're getting the real world data. There are so much more of these scrapers inside that you can use not only this, but these are the ones that I'm using.

00:54:54.000 --> 00:55:09.000
So now another thing that we are using, and this is like a little bit underdog, you know, tool. I don't think that many people use this one, but I kind of like randomly just found it by using by doing Grok research on X, you know, what

00:55:09.000 --> 00:55:25.000
kind of tools that have Api relatively cheap that will allow me to scrape like thousands or hundreds of thousands of ads from Meta. And I've bumped into this one, which is like very small startup. I don't know, like, I know we later on connected with a founder through

00:55:25.000 --> 00:55:48.000
through Telegram, I'm not affiliated. There is no affiliate link or something for it just to go and use it if you'd like. So essentially, this is, like, very cheap ad spy that can be plugged in through the API key to your Agentic system, and you can ask, you know, the agents, and I have the skill for it as well. Like, just go and find all of the competitors, and just scrape all of their image ads, all of their landing pages, URLs

00:55:48.000 --> 00:56:06.000
And the videos and everything, you just save it and then analyze and see what's working for the competitors, and that's it. Or I can go even further. Just recently I built something is that like let's just replicate what they have, the full funnel. So we'll take their image ads, video ads, copy their advertorials

00:56:06.000 --> 00:56:09.000
And let's take that. So, you know.

00:56:09.000 --> 00:56:26.000
gray hat version is let's copy it and just change the product more white version of it is like, let's take that, learn from it, and just build something that will be similar to what you know we have, you know, with the product that we have, and let's launch it, because it seems like it's working for them

00:56:26.000 --> 00:56:42.000
So that's another thing that we are using and I'm trying to compact what I'm saying as much as possible. Sorry about speaking fast. And data for SEO.com. So this one, like, you can use other APIs. This is for Google, if there are guys who are doing Google, I think it could be helpful for Meta guys, too

00:56:42.000 --> 00:57:00.000
is that this is the real-world data from the keywords and the volume of the keywords on Google. So kind of like what people are searching for, what is the volume, what specific keywords they're using, what are the trends? Is it trending up? Is it trending down? So for me, it's super valuable because we're launching the keywords

00:57:00.000 --> 00:57:19.000
Obviously, on Google Ads and search campaigns and shopping, we optimize the listings for the combinations of the keywords, so it goes into relevant search terms. This one is super valuable for me because it just pulls, like, all of the data, doing the research, going through, like, tens of thousands of the search queries related to the product that I'm launching

00:57:19.000 --> 00:57:36.000
and use that as the targeting for the keywords, but you can use that as understanding the trends, what people search for right now, like in in September, like, what people search for, how many people search for it, like, using these words, and that could be the additional signal for you to

00:57:36.000 --> 00:57:43.000
you know, to see what you can, you know, use in the ads. I don't know. But for Google, it's just invaluable

00:57:43.000 --> 00:57:54.000
Yeah, that's on, you know, from the perspective of, you know, what kind of, you know, tooling we are using. There were a couple of other questions in here.

00:57:54.000 --> 00:58:01.000
Can I just jump in real quick, Russ, because I know we're going off in the hour. Are you guys good to stay on for a little bit longer to go through questions with people?

00:58:01.000 --> 00:58:02.000
Yeah, sure.

00:58:02.000 --> 00:58:04.000
Does that work?

00:58:04.000 --> 00:58:05.000
Awesome.

00:58:05.000 --> 00:58:07.000
Yeah, I mean, like I answered like as much as I could, but I see that seven more dropped while I was talking.

00:58:07.000 --> 00:58:23.000
Oh, yeah, yeah, I think people are loving this. So that's why there's so many questions. Usually that's a sign that like people are getting a lot of value from it. Just quickly though, if you do have to drop on the hour, make sure they're on Thursday is the last session of the regular sessions for the course

00:58:23.000 --> 00:58:29.000
Which I'm going to be hosting all about building landing pages with

00:58:29.000 --> 00:58:45.000
With Core Code and Codex and we're going to do a bit of, like, a putting it all together from the six weeks we've gone through. So make sure you're there. And also the recording and transcript for this will be sent out, so don't worry, I know the guys have gone through a lot of different, workflows and tools, but if you

00:58:45.000 --> 00:59:05.000
missed anything or you, you know, wanna take it down, we're gonna be sending that out and put it inside the notion doc as we have been for the rest of the session. So, if you have to drop, thanks for coming. If you're staying on for questions with the guys, keep them coming, because, there's a lot that you guys have covered here.

00:59:05.000 --> 00:59:06.000
Andre.

00:59:06.000 --> 00:59:07.000
Yep.

00:59:07.000 --> 00:59:21.000
Philip asked this question in the chat, and you did respond to it, but I'd love to hear you speak more on this. How do you ensure copy quality? I know, like, Russ touched on this briefly, like, is it… is it all purely voice of customer?

00:59:21.000 --> 00:59:36.000
pulling that data in and using that, or is there any, any additional context that you've put in terms of, like, you know, copyrighting principles or marketing frameworks to improve the, the quality of the copywriting

00:59:36.000 --> 00:59:45.000
Yeah, so we have a certain procedure, certain skill for writing the copy, and the main point is to give that

00:59:45.000 --> 01:00:02.000
That skill, the instructions of what to write and what not write. So, for example, the example of the good copy and of the bad copy. And there shouldn't be too much of the examples, like 10 to 20, you know, cook examples, 10 to 20 lead ex…

01:00:02.000 --> 01:00:17.000
The 10 to 20 headline examples, for example, for the for the static images is more than enough. So, for example, don't don't write this, do this instead right? Then you pass the voice of the customers like voice of the customers

01:00:17.000 --> 01:00:20.000
Also tied to the angles.

01:00:20.000 --> 01:00:37.000
So when I start a new session, I can say, okay, let's write the like, let's make the images for this kind of brand. The skill will be the product MD. It will read the voice of the customer for a certain angle and the example of the good

01:00:37.000 --> 01:00:50.000
In a fresh session. And that makes, like, first, it limits the number of reads that agent makes. And then, like, based on the good examples, because the reference is good, it will write the badass copy.

01:00:50.000 --> 01:00:52.000
So not that complicated

01:00:52.000 --> 01:00:56.000
So, no need to feed it with the full

01:00:56.000 --> 01:01:08.000
I'll give you a breakthrough advertising

01:01:08.000 --> 01:01:09.000
Yep.

01:01:09.000 --> 01:01:12.000
Got it, got it. And then there's a question about skills here from Jacqueline, like you guys have got a lot of skills in your library and AI has been created those skills. Are you

01:01:12.000 --> 01:01:17.000
manually reviewing those skills to

01:01:17.000 --> 01:01:27.000
fine-tune them. Like, when you go and create 30 skills at a time, or are you just, like, running them, and then if something's wrong, then you'll go back and give them feedback

01:01:27.000 --> 01:01:39.000
I'm giving the feedback, but never review them on my own. So if something is going wrong in terms of the process, I just ask the agent, like, how can we systematically

01:01:39.000 --> 01:01:46.000
fix that to avoid repeating this mistake again in the next session, and that's it

01:01:46.000 --> 01:02:11.000
Yeah, I can tell you like what I'm doing is that I'm first of all, like the new model comes out, I just ask it and I launch, you know, I launch multiple times. I run it once, I run it the second time, the same prompt, you know, and I will talk to it again and say something, you know, you know, you were the new model, Opus 5.5. Just go through everything, you know, all of the skills consecutively that we have inside of the project and see what we have redundant that will

01:02:11.000 --> 01:02:29.000
that we don't need anymore, and just cleaning up, or just provide me the plan, what you would remove, for example, and why. That's one thing that I would do. Another thing is that Claude actually has the official protocol for something like this. It's a command that's called, I think, cloud-api

01:02:29.000 --> 01:02:34.000
eval. So you run that one, and it evaluates your skills

01:02:34.000 --> 01:02:47.000
how they are good for running with the newest model. And there is, I think there is another one which Claude dash API

01:02:47.000 --> 01:03:01.000
Oh, contest or promote or something like that. So I think Tariq from Claude Code team from Entropic, he recently, you know, posted in regards to this, you can find that article, really good one. So that's another thing, because especially from

01:03:01.000 --> 01:03:03.000
Also, Rosa

01:03:03.000 --> 01:03:04.000
Yep.

01:03:04.000 --> 01:03:18.000
I have also sent the agent skills.io. That's the website basically by entropic on how to write the proper skill, the all the principles are there. So could you share, please?

01:03:18.000 --> 01:03:20.000
Yeah, what's that again, Andre?

01:03:20.000 --> 01:03:24.000
Agentic skill, urgent skills.io

01:03:24.000 --> 01:03:27.000
Yeah, yeah.

01:03:27.000 --> 01:03:41.000
I will just get in and send it over.

01:03:41.000 --> 01:03:51.000
Yeah, here we go. Just drop in the chat

01:03:51.000 --> 01:04:07.000
I open

01:04:07.000 --> 01:04:14.000
While that's loading, Russ, are there any other questions from the chat or the Q&A that you want to pick up?

01:04:14.000 --> 01:04:30.000
Yeah, I'm actually responding to some of them as well. So do you use Meta MCP to launch ads? No. I actually posted about this on X and I've done, you know, when everyone was hyping about the CLI and MCP, CLI is a little bit better

01:04:30.000 --> 01:04:46.000
MCP is like super slow. So I did a test. We at that point already, you know, were launching through the API. APIs like blazing fast seconds, MCP is like minutes, and sometimes on the bigger accounts where it's thousands of the odds, cannot even complete the request

01:04:46.000 --> 01:05:01.000
So I would just use, you know, just API. It's a little bit harder to set up if you would do it manually. If you would do it through the agents like we're talking about the AI agentic setup. So it's anyway, like, it's done through AI agents

01:05:01.000 --> 01:05:19.000
It's really the same thing. You just ask it to, you know, to just build it out with API connection instead. One of the question was, like, how you guys didn't get banned because you're launching so much. Honestly, like, we didn't even bump into this issue. I mean, Andre

01:05:19.000 --> 01:05:35.000
We're doing most of the launching, but both my system and his system, he's launching, essentially, I'm just checking and pulling the, you know, the creatives is used as it should be done with the app and the system user. So when you do it properly

01:05:35.000 --> 01:05:49.000
You know, like this, I don't think you… you will bump any kind of issues. Andre is launching, I mean, lots of stuff in there, and we never had any issue. Maybe we have Golden BM Manager business manager, but

01:05:49.000 --> 01:05:50.000
I doubt it.

01:05:50.000 --> 01:05:57.000
I understand where the question is coming from. So directly connecting

01:05:57.000 --> 01:05:59.000
Claude to

01:05:59.000 --> 01:06:15.000
To Meta's API is dangerous because Claude starts to explore and starts to bump into the API very frequently. So I built this kind of a tool that has the UX, and I also have the same one for the agents that doesn't have the

01:06:15.000 --> 01:06:19.000
UX, so the agent can

01:06:19.000 --> 01:06:36.000
can call it. So this is the layer, programmatic layer between the agent and between the meta API. So this is this is called the asynchronic infrastructure, where you have the router, which is called Redis

01:06:36.000 --> 01:06:51.000
And the workers that are working on the salary, like, this thing is called salary workers. Basically, the Python executable code in itself container. So when I need to launch the ad.

01:06:51.000 --> 01:07:06.000
I use this UI. So, for example, I use the brand like use the offer. For example, if I need to change the settings like I will select the product, and it will substitute all the text for me. So this is the first tool that I've made

01:07:06.000 --> 01:07:18.000
Because I was just bothered to upload everything through the ads manager. So I can pick any client, any offer, and at all. It already has the

01:07:18.000 --> 01:07:34.000
All the settings that I need per client, drag and drop the creators and click create the campaign. So what happens in this moment? In this model, in this moment, the task in the queue is being created, and the first worker

01:07:34.000 --> 01:07:51.000
can pick it up and start knocking the API, but with the rate limiting. So it means that it knows how to work with meta already, and I do not have to reinvestigate this path every time. So it's a fine-tuned system

01:07:51.000 --> 01:08:06.000
And if I need to launch 1,000 creatives, it will separate the work, split the work between multiple workers that will work in parallel without knocking the API meta's API rate limits. So this system is super safe because

01:08:06.000 --> 01:08:19.000
It acts like a launcher with its own safe boundaries that prevents from knocking the API too frequently

01:08:19.000 --> 01:08:22.000
Love it.

01:08:22.000 --> 01:08:35.000
Another question here from Jacqueline. Want to go back to AI generated static. Our biggest bottleneck is quality of AI generating AI generated statics. What are your

01:08:35.000 --> 01:08:37.000
Top three tips

01:08:37.000 --> 01:08:47.000
For someone who's struggling with quality, or just some of your top tips, someone who's struggling with quality of their AI statics.

01:08:47.000 --> 01:08:56.000
So I think it was an issue when GPT model one was just released. So you had to prompt

01:08:56.000 --> 01:08:58.000
In the

01:08:58.000 --> 01:09:13.000
very details, like what should be here, what should be there, from right now, how we approach the statics, Claude code, you can paste the images in there, even though it looks like a black terminal, you still can

01:09:13.000 --> 01:09:24.000
Use Common V. Common V in there, and it will copy the image that you've copied somewhere from the feed, from Twitter, whatever. And you can ask it

01:09:24.000 --> 01:09:33.000
Reverse engineer this creative by 10 parameters like the color, the headline, the layout, the whatever the fonts

01:09:33.000 --> 01:09:49.000
By 10, 15 parameters, you can even not name them. So Claude will understand like what are the possible options, right? It will reverse engineer. And then by using those parameters or using those settings that

01:09:49.000 --> 01:09:57.000
just reverse engineered and saved into the MD file in in the template. Let's come up with the prompt

01:09:57.000 --> 01:09:59.000
For the year

01:09:59.000 --> 01:10:09.000
Image generation model like GPT-2 or another banana. And let's try to generate the prompt that we will send to it afterwards. That's it. So

01:10:09.000 --> 01:10:13.000
This is the number one and the only tip I would say

01:10:13.000 --> 01:10:17.000
So make the AI reverse engineer

01:10:17.000 --> 01:10:27.000
Something that is working and then save it as a template. And then use it to come up with a new prompt for the AI models.

01:10:27.000 --> 01:10:28.000
Got it.

01:10:28.000 --> 01:10:43.000
Yeah, I would just say, like, what do you feed to Wade? Like what you will get essentially because the better input, the better output. So if the quality is the issue from the perspective that the copy is not good, the idea is not good. So

01:10:43.000 --> 01:11:10.000
Feeding it real-world data plus what I also do, like, I have the library of the design approaches for the creatives. I kind of like, as soon as I bumped into something interesting, I just send her over and to the chat, just copy and paste it, and it would just build, you know, analyze it, break it down like colors, composition, copy used, etc. Give it a name and save it in the separate, you know, folder inside of the project, which called static theme

01:11:10.000 --> 01:11:37.000
And I have like 200 plus of different themes. So as soon as you find something else, you just drop it in there. If it will qualify it as the same that you had before, it will save to the same one, and also have, like, JSON files and everything inside, outlining what is the stylist is. So, and then, as soon as you print the credits, you can just point it in the specific style or how I have it like it just go free style and take some of the inspiration from those themes as well.

01:11:37.000 --> 01:11:48.000
But for copywriting real world data, a verbatim from the customers, and as the quality of the image is concerned, then I don't know, like the latest image generation models

01:11:48.000 --> 01:12:05.000
I wanted to point this out that sometimes it's not that important. And I wanted to share the badass case that I also shown to Alex when we were in Greek. So that's a Patriot Chave thing. So the guys are selling razors

01:12:05.000 --> 01:12:18.000
Like very cheap stuff. And we compete with Dollar Shave Club, with Harry's, with Gillette. So we cannot say that we are sharper, cheaper, better, no irritation. So the only

01:12:18.000 --> 01:12:35.000
A competitive advantage is that the guys are putting the American flag into the box, right? So, and I was trying to crack that not for two or three months, something like that. So it was the last year, so, the images are pretty ugly, but I started from

01:12:35.000 --> 01:12:45.000
printing these kind of creatives like America, America First, you know, American colors yeah they're like people look like they are AI generated because it was GPT image pop

01:12:45.000 --> 01:12:52.000
So nothing of that work. So I'm just showing you the failed examples

01:12:52.000 --> 01:13:02.000
You will understand why the messaging is much more important and customer persona is much more important compared to the beauty of the creative. So

01:13:02.000 --> 01:13:17.000
Nothing of that work. So the next month, I try to try to find out like what kind of customers I'm trying to advertise to, who are the true patriots? Like, I was testing personas, hardworking men, you know, policemen, construction workers

01:13:17.000 --> 01:13:21.000
Truck drivers, Texas farmers

01:13:21.000 --> 01:13:26.000
Nothing of that worked, so tapping into different customer personas

01:13:26.000 --> 01:13:30.000
didn't help because it was like the surface level

01:13:30.000 --> 01:13:32.000
But then

01:13:32.000 --> 01:13:37.000
I was just talking to Claude and

01:13:37.000 --> 01:13:41.000
trying to understand like who like who are those patriots? And it came up with

01:13:41.000 --> 01:13:54.000
genius idea. Those who go to church on Sunday, they are patriots by definition, because they pray for the country, and that's the next layer of the psychology. So it's not, like, something that your the patriarch just because of your

01:13:54.000 --> 01:14:02.000
put on American flag on onto your card like you pray for the country, so you are patrolled for… you are the patriarch by definition.

01:14:02.000 --> 01:14:19.000
And we started to bring this kind of creatives. Our razors are meant for men who go to church on Sunday and it instantly started to show the signs of life. You see the shirt, the Bible ring, like polished shoes, the military guy. So you see

01:14:19.000 --> 01:14:23.000
by quality of the images didn't improve

01:14:23.000 --> 01:14:24.000
But

01:14:24.000 --> 01:14:26.000
The message, indeed.

01:14:26.000 --> 01:14:32.000
the seem like some of the guys recognize this chin, very famous one

01:14:32.000 --> 01:14:34.000
So, and then

01:14:34.000 --> 01:14:50.000
We started to dig deeper, what can trigger those who go to church on Sunday? Like, can we throw the stones at the enemies? And the brand founder, like, he provided me a collection of the ads that bigger brands

01:14:50.000 --> 01:14:53.000
Making to support

01:14:53.000 --> 01:15:01.000
To support the LGBT, and we've printed the creatives that changed the entire trajectory of the ad account. Which flag do you support

01:15:01.000 --> 01:15:16.000
Gillette ad features transgender teens first shape with that. Boom! Harry launches Shave with Pride set to support LGBTQ. Boom. So it instantly caused the reaction. So

01:15:16.000 --> 01:15:27.000
tapped into those who go to church on Sunday and thrown the stones to the enemies right and this is like the real facts we didn't invent so they literally

01:15:27.000 --> 01:15:34.000
Like send money to Black Lives Matter and Gillette ran this ad. And Petro Chev, yeah, Faith

01:15:34.000 --> 01:15:43.000
Family freedom, tradition, and the American flag, full package. Boom. So those who go to church on Sunday instantly started to react on this one

01:15:43.000 --> 01:15:50.000
And here's the final boss, you know, once the big idea is there, you can iterate

01:15:50.000 --> 01:16:00.000
On this big idea with enormous amount of creatives. So once I understood what the big idea is, it, like, became a no-brainer what to print next.

01:16:00.000 --> 01:16:14.000
Right? So I started to print those creatives like crazy, and we sold out the stock in a couple of weeks, and then, you know, the guys had a hard time getting new stock. So once you get that thing

01:16:14.000 --> 01:16:15.000
You know

01:16:15.000 --> 01:16:18.000
The scaling becomes

01:16:18.000 --> 01:16:23.000
minor problem, and the stock becomes a bigger problem

01:16:23.000 --> 01:16:39.000
Yeah, and also, like, in regards to the question, there's, there was this question, like, out of the 1,000 creatives, like how those are, you know, is there any that are good? I mean, the guys, like, they're… it's just, like, the creatives shouldn't be

01:16:39.000 --> 01:16:58.000
So if you do volumes, it doesn't mean that's just, you know, or something. So, I don't know, like, you know, we just print lots of them. They have, like, different kind of messaging. It's not like, you know, like, retired this Sunday vaccine here, not bidding for refund

01:16:58.000 --> 01:17:15.000
You know, there's even like a little bit more aggressive, like, sounds like a scam, it's going to the advertorial. So it's like different approaches is that there's a bottle, there is a person in it, and so on. So it's, you know, Andre just showed some of the older stuff that were generated, like, with the older models

01:17:15.000 --> 01:17:27.000
The models, you know, these days are pretty good. I mean, you probably generate lots of the image creators, so it's, it's not like, you just

01:17:27.000 --> 01:17:44.000
You know, collect read the same thing, you know, like 20 times like we're testing multiple of the different angles and launch them. And it's not like out of the 1,000 credits, you know, there

01:17:44.000 --> 01:17:52.000
You know, Tandit actually worked. No, just a lot. We just push lots of volume. You know, one of the things, you know, also to understand in regards to

01:17:52.000 --> 01:17:58.000
In regards to the, you know, how auction works for demand gen and for Meta as well.

01:17:58.000 --> 01:18:10.000
With BCAPS, just imagine this, so when you're using BCAP, so it's like the expected CPA that you want to get with your expected CPA that you want to get with your creatives.

01:18:10.000 --> 01:18:16.000
So when you launch like 20 creatives, let's say

01:18:16.000 --> 01:18:18.000
So, for Meta.

01:18:18.000 --> 01:18:38.000
you know, with with this copy, and with this new destination URL, you know the creative one has some addressable market that it can go after and get the Cpa that you're looking for for a creative tool that has just a little bit of a portion of the addressable market where Meta can actually get the Cpa that you're looking for expectedly, of course, but their algorithm is

01:18:38.000 --> 01:18:56.000
Scary good. And the creative 3, and so on. So every single creative kind of gets its own, like, bucket where there is a high confidence based on what this creative is, what's on it, based on the meta-analysis of this creative, where Meta can deploy this, deploy this creative

01:18:56.000 --> 01:19:17.000
And get the performance that you're looking for. So when you launch, like, five creatives, then you have limited buckets in there, just out of these five creatives. And if, especially if you launch it, like, on lowest cost, for example, maybe you saw this, is that, like, you launch lowest cost, you know, it can maybe perform really well, like, in the first, you know, couple of days, but then it kind of, like, dies out

01:19:17.000 --> 01:19:33.000
You do not restrict it with the we want this CPA to get. And it continues to spend the full budget that you allows this creative to spend. And then Meta is kind of like out of the addressable market where it has the confidence to show these credits to and get

01:19:33.000 --> 01:19:35.000
you know, any kind of results

01:19:35.000 --> 01:19:57.000
When you have lots of decretives, like, okay, so this messaging will go to this bucket, this messaging on the creative will go to this bucket, and with this visuals overall, and so on. And you get so much more volume going out, just the most certain volume that will get the CPA that you're looking for, especially when you're using the big caps in place

01:19:57.000 --> 01:20:18.000
So that's why you need volume, but it has to be, like, different creative with a different kind of messaging that will go into the, you know, towards people that are more inclined by meta formula, which is using the expected, you know, the expected CTR, expected conversion rate on the specific landing pages, and so on and so forth, you know, to get the conversion that you're looking for

01:20:18.000 --> 01:20:26.000
So that's why the volume is the key there. But again, it doesn't mean that your creative should be shitty or something.

01:20:26.000 --> 01:20:27.000
Yeah.

01:20:27.000 --> 01:20:36.000
How much time should we give each air to perform before deciding whether to keep or pause it? So the thing is that we… that if you set a bid

01:20:36.000 --> 01:20:53.000
And if it doesn't spend, it's a failed test. If you set a bid and it spends, it delivers you results. So the campaigns on bid caps, they don't need that kind of a babysitting, right? So I usually kill the ads if I don't have any delivery

01:20:53.000 --> 01:21:00.000
In 14 to 21 day

01:21:00.000 --> 01:21:20.000
Guys, this is so good. I mean, people are loving this. I am amazed every time that you guys, do a talk. A couple of things I want to say on the static generation process. It's interesting to see that, Russ, you have a similar process to what I do, what I think you call themes like we talk about, like, building a swipe file of, like, templates

01:21:20.000 --> 01:21:37.000
And if you… if you are curious about that, and you're watching this, like, go and watch Session 4 that I did, which is basically the same process that the rush has described, like, build all your templates, and then, have AI either go and execute on those templates or use a bunch of them for inspo to go and put out ads for you

01:21:37.000 --> 01:21:52.000
And the second thing I want to say on volume is that like who cares if the quote hit rate is lower, if the hit rate is, you know, 3% rather than 8% because you're launching

01:21:52.000 --> 01:22:02.000
20, 30, 40x more ads, so you're going to get more absolute winners. Now, you don't want to make sure that, obviously, your ads aren't, like, doing any reputational damage

01:22:02.000 --> 01:22:19.000
brand-wise, but assuming that's not the case, it's like, well, if I have ads that hit a lower percentage than my… than my, you know, ads that I make outside of AI. But I can launch 50 times more ads than, like, I'm gonna get more absolute winners, and that's gonna be better for the overall account.

01:22:19.000 --> 01:22:20.000
Yeah, sure.

01:22:20.000 --> 01:22:21.000
And it's so cheap to generate, like, why not

01:22:21.000 --> 01:22:34.000
I totally agree. And again, like, as soon as you have these processes in place, you kind of like the speed of your execution and the quality of your execution accelerates as soon as the new model is coming out.

01:22:34.000 --> 01:22:40.000
Like, there is a huge gap between the GPT image one and the latest GPT image model.

01:22:40.000 --> 01:22:53.000
So the quality is just getting better. Like those who collect used to, okay, so we're just manually doing that, we're just using Canva or something, or in Photoshop, you know, collecting all of the creatives. Yeah, I mean

01:22:53.000 --> 01:23:07.000
Man, like, probably I have a bad news for you because maybe like in one year from now, until it's just better to just start to keep up with that because then it will be really hard to compete with that. So and build the systems around it.

01:23:07.000 --> 01:23:08.000
Yeah

01:23:08.000 --> 01:23:29.000
There was a the question in regards to how do you enrich update knowledge of the product research VOC, what system do you have for that and how does it work? So you can, you know, like the all of the VOC is inside of my system, for example, it's stored inside of the ledger. So ledger is like fancy word for like, okay, so there's some files over there where it stores all of it

01:23:29.000 --> 01:23:50.000
It has the timestamp when the last VOC mining was done. And actually, this is a good idea also, like, one of the things about the ledgers is that, like, for campaigns launching, for campaign updates, like, one of the things is that, like, if you were working on the account, like, there should be timestamps for everything. You shouldn't explicitly go and timestamp

01:23:50.000 --> 01:24:11.000
You just need to want to ask the system to build this process inside of your skills that are touching something that there should be timestamps, like, because when I'm hopping on, you know, to work on the account, for example, on, you know, on Thursday, let's say, and I want to optimize, you know, like, the specific campaign, I'm just sending over the campaign ID, okay, so let's just see, like, what we can do better in there

01:24:11.000 --> 01:24:26.000
So the agent should know, like, that, for example, 2 days ago, we've done the changes already to this campaign, and what exactly we changed. So it doesn't like replace the thing that didn't get any chance to actually do anything

01:24:26.000 --> 01:24:52.000
And or it should just show me, like, okay, so it's just better not to touch it, because we just, you know, did some changes over there. The same for VOC mining, the same for other changes. So, it should be, like, the system of the ledgers with the timestamps inside, so your agents always know, like, when the change was done. And also, like, what fun thing that started to do, I didn't ask for it, it just kind of came out naturally, you know, in the in the conversations with agents is that

01:24:52.000 --> 01:25:11.000
You know, they're like, okay, so yeah, we've done through this, we did this, this, this, and this, but this is, like, we're not doing, we kind of like, you know, like, it's scheduled for, you know, like, September 31st, because we did the change to this, you know, asset, for example, two days ago, but right now it's too early to change it, and it's kind of like built some, you know, kind of like

01:25:11.000 --> 01:25:28.000
forward-looking, you know, task list that is not go… they're not going to execute right now, and I'm… we'll close this session, so it's not like it will be… I'll be keeping this session until, like, 31st or something, but it will save, like, inside of this… its notes, and it's, like, these ledgers, it's

01:25:28.000 --> 01:25:47.000
like files which they create in there. Okay, so, like, on 31st, we do… we need to do this, like, on the, you know, on October 3rd, we need to revise our post hoc test that we're doing for this, you know, advertorial A-B test, because we might have results already, and on October 7th, like, we need to check this, because

01:25:47.000 --> 01:25:52.000
It's already time, and there should be statistical significance for this.

01:25:52.000 --> 01:25:56.000
So kind of like this thing. So if that makes sense.

01:25:56.000 --> 01:26:12.000
Are these Hermes agents, I don't use Hermes. Like I have Hermes, like I try to use Hermes. Hermes is like, you know, I don't think cloud code you can use, I don't think you can use Entropic subscription on Hermes, at least

01:26:12.000 --> 01:26:33.000
As I know, on Tropic can ban you for this because they're explicitly saying nothing except Cloud Code can use traffic subscriptions. You can use API, but it's freaking expensive, like 10 times more expensive than using the plan. Codex, the OpenAI subscription you can use inside of Hermes, but it's limited context window of 29

01:26:33.000 --> 01:26:53.000
thousand tokens, I think, when the full one is 1 million, essentially, inside of Codex. So that's why it's kind of like, I'm using entropic models, and I'm using OpenAI models. So in Hermes, I can use only OpenAI and also with a limited window and there's no way to expand it. I tried to overwrite some of the, you know.

01:26:53.000 --> 01:27:11.000
config files over there, so we can use 1 million tokens. It can't. So that's why I kind of gave up. It seems like it's really good and interesting, you know, harness. It's super effective at what it does. As soon as you're working with the API, I think it makes sense to use it with the API

01:27:11.000 --> 01:27:29.000
But API is so expensive compared to weekly limits in monthly subscriptions that I just don't use it. And I don't use crons. The only one, like, on my local machine for sure, because I don't want it to be open all the time, even though it is, because agents are always working, but

01:27:29.000 --> 01:27:39.000
I don't want to kind of like be have like this, you know, asterisk over there is that I cannot close it if I want it, and, you know, travel or something.

01:27:39.000 --> 01:27:57.000
So for everything cron related, so something repetitive, for example, I'm pushing the updates of the availability and the price and the quantity in the shopping feeds on Google Merchant Center. So I have the separate railway server. So I'm also like another thing that I recommend, like everything that you need to kind of like run all the time

01:27:57.000 --> 01:28:11.000
Recurring, you know, any… anything. Just spin up, you know, ask the agents, okay, so we'll just deploy in Railway, like this, you know, function, and let it run, like, every day or every hour or something like that. It's super cheap, it's like $10 or something, and that's it.

01:28:11.000 --> 01:28:35.000
And you can always, you know, pull the data from it or send the updates and so on. That's what I do. And I'm not using routines or something because again, routines, if your computer closed, they will not fire. So it's kind of like, I don't know, just a little bit clunky. For those who are just running desktop setup that always turn on, I think it makes sense

01:28:35.000 --> 01:28:49.000
This is a question in the chat that I'm curious to get your guys' take on. What part of the process do you review often? And given that you've automated pretty much the whole process, what do you actually spend your days doing?

01:28:49.000 --> 01:28:53.000
Okay, so what part of the press do you review often? Okay

01:28:53.000 --> 01:29:10.000
I mean, it's not like they're automatically running. I mean, like at some point, maybe they will be automatically running, but you just open. So thinking, thinking and talking. So like I can spend, you know, like a time spent, you know, playing with my daughter and I will just

01:29:10.000 --> 01:29:25.000
you know, think about, okay, so very recently, like, for example, I was like, okay, so that would be cool to build a scale that will be pulling, like, every single asset from Google account, and I usually, you know, a Google account has maybe.

01:29:25.000 --> 01:29:41.000
I don't know, tens of thousands of different headlines and descriptions and image ads and video ads and keywords and search terms, and so on. So, it would just pull, like, every single one of them, put them in the Google sheet, for example, through GWS CLI

01:29:41.000 --> 01:30:02.000
just for me to review, but also analyze all of it, and just find, like, really losing across all of the account, like, really losing headlines or descriptions, or image ads, or video ads, like, some kind of, like, cleanup type of the flow that will just pull on a bigger timeframe, like 3090, 180 days, 365 days

01:30:02.000 --> 01:30:19.000
pull everything, all of the performance of every single miniscule asset inside, and just bottom like 20% down performers just remove them from the account. So kind of like unlink from the asset groups and ad groups

01:30:19.000 --> 01:30:20.000
Another one

01:30:20.000 --> 01:30:36.000
Another stuff, I mean, like, I will have the idea of something and then we'll just go and jump on Andre knows like I have no task lists. I have no dashboards, Trello, whatever. My kind of like work eth and I've been like this before, but now it's kind of like my

01:30:36.000 --> 01:30:46.000
the way I work is that, like, I have an idea, I open the laptop or jump in front of the laptop, I open the new clockhouse session, I talk to it, and I just implement it.

01:30:46.000 --> 01:31:01.000
But on the daily basis, I mean, you still need to do things, like, for example, you know, like today, I'm like, okay, so let's just go through the shopping campaigns everywhere and see what we can, you know, maybe, like, create multiplication strategy where we can get some more volume. Highlights to take a look at the performance

01:31:01.000 --> 01:31:13.000
Let's launch, you know, this… I have this idea for demand gen. So it's kind of like you… you still I've heard like I've read like on Twitter somewhere, someone written is that

01:31:13.000 --> 01:31:33.000
You know, the agents can do the work for you, but they… they… I mean, I'm, like, very loosely rephrasing it, but they cannot, you know, think of themselves like what to, you know, what kind of business to build for you, or what to do for you, you know, higher level. So essentially, we still think on a higher level, like, what we try to achieve

01:31:33.000 --> 01:31:52.000
So and then you have this unlimited workforce that you can employ for yourself, and it gets better. It learns from you, you learn from it. And if you need it just a little bit of it, you can get a little bit of it, but then if you need a lot, then you just spin up more sessions and do more

01:31:52.000 --> 01:31:53.000
Yeah, for example.

01:31:53.000 --> 01:31:54.000
What I do

01:31:54.000 --> 01:31:58.000
I just wanted to extend that. So

01:31:58.000 --> 01:32:14.000
I just spent the last month building the layer playing back and forth, building the management layer. So the thing is that every session is the ID number and each session is stored as a JSON file

01:32:14.000 --> 01:32:21.000
It means that other sessions can read what like sessions can see

01:32:21.000 --> 01:32:37.000
If you ask them what different sessions do, so it means that you can have the orchestrator that is open session that can monitor the other sessions, and this is a management layer. So I developed a certain procedure that spawns… that pushes this management

01:32:37.000 --> 01:32:54.000
Session every 30 minutes to understand, like, what is going on in the parallel sessions. And if, like, it… the main goal was to remove myself from the… from the loop, right? So, for example, like, Shelby launched the set or not. Like, I need to review it manually, but

01:32:54.000 --> 01:33:12.000
Now that management session spawns the agent, it analyzes the creative that was made and decides on its own whether it works launching the account or not. So if it works, it invokes another agent that creates the ledger, it pushes the task to the queue, and it goes live

01:33:12.000 --> 01:33:16.000
Into the ad account. Then, on a daily basis, this

01:33:16.000 --> 01:33:18.000
management session

01:33:18.000 --> 01:33:35.000
First, fetches the data from all of the ad accounts, spawns the agents that go to see the atlas that is being recalculated on a daily basis, that scheme that I have been showing you to analyze what is working, what is not working, generate ideas

01:33:35.000 --> 01:33:51.000
and then sends it to the creative agents, which are the parallel sessions. So it's the self-evolving system. And the thing is, like, sometimes this manager tries to ask questions right? And I also made the 3rd session, which is the secretary session

01:33:51.000 --> 01:34:03.000
Why? Because when the agent is using the ask tool, it stops working. So the boss sends the questions to the secretary session, which leaves only to

01:34:03.000 --> 01:34:21.000
To ask questions to me. Like I respond, send it, it sends to manager, manager sends to other sessions, and they proceed the execution. So it's the middle of the week, and I've already burned my $200 subscription, so I'm shifting to another one

01:34:21.000 --> 01:34:22.000
Right now

01:34:22.000 --> 01:34:26.000
So so yeah, management layer is the next thing

01:34:26.000 --> 01:34:27.000
Yeah.

01:34:27.000 --> 01:34:28.000
Yeah.

01:34:28.000 --> 01:34:29.000
I love that

01:34:29.000 --> 01:34:44.000
But essentially, like, this is like interesting question like, why would we still need specialist if these skills can be generated by AI and iterated based on feedback. So I mean, man, like, have you heard that you know that doomsday is coming that you know, AI is just

01:34:44.000 --> 01:34:47.000
kill all of us, and so on and so forth, so… I mean, it's

01:34:47.000 --> 01:34:50.000
Yeah, be polite with Claude.

01:34:50.000 --> 01:34:55.000
Yeah, at some point, look, I mean, at some… at some point

01:34:55.000 --> 01:35:16.000
You're right. I mean, just that kind of future that comes, it depends like how fast the acceleration would be, you know, for AI development and using AI to develop AI even faster, which will get smarter and so on. And then there is Optimus robots and other robots coming, robots coming into the market, which will

01:35:16.000 --> 01:35:17.000
Get them

01:35:17.000 --> 01:35:24.000
The physical representation. So I don't know. It's just

01:35:24.000 --> 01:35:32.000
At some point, all of these things do not matter, and everything will be handled

01:35:32.000 --> 01:35:55.000
So, I don't know, like, when you're washing your, you know, your stuff, you know, in the washing machine, you don't think, like, how about washing machine, like, is doing inside? So it's got, like, just throw it inside, and you just get this stuff out when, you know, the same with, you know, a lot of other… you don't know necessarily how your car is working, but you're just sitting in it, and it goes and you hit stop and it stops

01:35:55.000 --> 01:36:10.000
So lots of the things like in our life, just getting automated, it's just AI is a little bit different beast. Like we can see it like working in the digital. Like a lot of folks just don't get an idea like how powerful this thing is. And it's becoming and how fast it's accelerating to become this

01:36:10.000 --> 01:36:13.000
You know, like

01:36:13.000 --> 01:36:25.000
general intelligence, right? Super intelligence, but I don't know. Just… it's just, like, it would be less and less stuff for us to do, and,

01:36:25.000 --> 01:36:45.000
Until nothing. I don't know, man, like nothing. No one knows like what will be like in three, four, five years. Lots of people ringing the alarm about the things. Some of people painting a really great future that, you know, that AI is bringing us. But it seems like we just can't the only thing that we can do is just to write this

01:36:45.000 --> 01:36:56.000
You know, just do our thing, do our craft, etc. This labs will continue to, you know, to do and push their AIs to the limits. I don't know

01:36:56.000 --> 01:37:01.000
But it's just cool technology. I mean, it's pretty cool technology. Well, it will lead us. I don't know

01:37:01.000 --> 01:37:02.000
Yeah, it's

01:37:02.000 --> 01:37:03.000
I'm not trying to bring, like, a doomsday, you know, vibes in

01:37:03.000 --> 01:37:30.000
No, I know, but like we spoke about this before, it's like, okay, if that's going to happen, which none of us know what's going to happen, whether like how it's going to pan out, but like assuming that things are only going to get more advanced and systems are going to get easier, like, it's only going to get easier to build, it's like, well, you've got two options, given that that's the case and you can't change it. You can either put your head in the sand and keep doing things the current way and just saying like, this is not for me, it's too technical.

01:37:30.000 --> 01:37:38.000
I'm not interested, or you can just go, okay, this is the way the world's heading, I might as well try and be on the forefront and see where that takes me

01:37:38.000 --> 01:37:53.000
Exactly. Yeah. And also like it's cool, interesting to work with it. I never had such pleasure working in this, you know, in this niche that I am right now. It's like, we can do so much

01:37:53.000 --> 01:37:58.000
Everything is super scalable and

01:37:58.000 --> 01:38:06.000
You can be anywhere you want and do, like, really a lot of damage, as even being one man, you know, banned, essentially.

01:38:06.000 --> 01:38:12.000
Without having to manage so many people. So

01:38:12.000 --> 01:38:31.000
Yeah, for sure. Guys, anything else that you guys want to go through with Russ and Andre? I think you guys have done an excellent job clearing pretty much every question we've got here. Anything else that you guys want to say? Where do you want to send the people? Obviously, this recording is going to be sent out with the transcripts are like

01:38:31.000 --> 01:38:39.000
If there's anything else you want to cover, cover. If not, tell the people where they can find out more about you, and if people want to work with you, how they can do it.

01:38:39.000 --> 01:38:49.000
Yeah, I mean, like, X probably would be a good place to engage. I will just drop my and Andres

01:38:49.000 --> 01:38:52.000
X handles

01:38:52.000 --> 01:39:07.000
If I can, yeah. And I don't know, like we have the website, tackra.co. I don't know, if there is any brand owners that want to collect employ AI in what they're doing instead of

01:39:07.000 --> 01:39:13.000
and scale, then, you know, definitely reach out to us. We have the book a call on our website.

01:39:13.000 --> 01:39:37.000
And also someone asked, like, in regards to, you know, how to build the systems like this, we covered a little bit, but we also have our system which, like Andre was hesitant to share. But, you know, there are a couple of folks who asked us to, you know, share the systems that we have from Meta and Google. We have it at Tegra as well and Tegra Co. Just take a look at that. So it's not free, just telling you right away. But this is the system that we update, like weekly and just push

01:39:37.000 --> 01:39:52.000
Like what we do internally, we just push there too. So it's like a full clock code systems. And yeah, just anytime, just hit us like on X or something. Andre, I know like a lot pause a lot of stuff. I'm not that engaged in X, but I will try to be

01:39:52.000 --> 01:39:59.000
And if you want to, you know, chat, just reach out on X.

01:39:59.000 --> 01:40:04.000
And I would highly recommend doing that. These guys are making us feel the AGI

01:40:04.000 --> 01:40:22.000
It's coming, and I'm sure you guys see why I wanted to get them both on today. Thank you so much, guys, this was an incredible session, one of my favorite sessions we've had so far. Go and follow them on Twitter, check out Tegra, and make sure they're on Thursday for the final regular session of the course

01:40:22.000 --> 01:40:25.000
So thank you guys. Any closing words, anything you want to say?

01:40:25.000 --> 01:40:35.000
No, man, it's been great, you know, chatting here today. There were a lot of really great questions and it's been a pleasure to share the

01:40:35.000 --> 01:40:38.000
The evening with you guys, or the day, or someone

01:40:38.000 --> 01:40:39.000
Thanks for having me

01:40:39.000 --> 01:40:42.000
All right, guys, thank you so much and we will see you all on Thursday. Goodbye.

01:40:42.000 --> 01:40:49.000
Absolutely. Yeah, no, bye bye.

```

