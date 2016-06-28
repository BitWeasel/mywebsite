---
layout: post
title:  "The world of IT certificates in industry"
date:   2016-06-28 09:40:13 
categories: industry
---
For once, I'm going to rant and be sarcastic. I'm going to write about something that really bothers me: the need to get certified in industry in order to get ahead.
You see, I work as a consultant in the IT industry, specifically in the security branch. (You don't say...)
Part of being a consultant is to have a sales department that finds you secondments, short or long term assignments with other companies who are in need of a particular skillset.
But how do you determine who is skilled, without actually talking to the potential employee.
Enter certificates and horrible CV's.

## The CTRL+F way
You might expect that once you get your master's degree in say computer science, or information science, that you'd be set for life.
Or at the very least, companies would like to offer you a job, and you could finally stop studying and start working, paying off that student loan.
Unfortunately, you're missing a lot of practical skills, because you're a trained academic, a scientist, maybe you even finished a PhD in some theoretical crypto direction.
You'd think that having a degree would be enough.

Nothing could be further from the truth.
You see, recruiters have no idea what 'C', 'Python', 'applied crypo', or anything else means if you put it on your CV. 
All they know is that they have a list of terms that need to be on your CV, and if they can't find them, you're not being considered for the job.
Seems a bit harsh, and I know not al companies work this way, but in general, there is more truth to this than I would like.

So what happens? 
In order to get a job, you start to put everything you know on your CV, in order to make it more likely that you will pass the ctrl+f of the recruiters.
And what you end up with is a CV that contains utterly useless statements in your skillset:

+ HTML - because I work with it every day

+ SSL/TLS - again, I use this on a daily basis

+ Telnet, SSH, UDP - Look, I know technical things

+ Kali - I have a VM of it somewhere, and how hard can it be. (This was literally the comment of an coworker)

+ Windows, Linux - Because recruiters might miss the fact that you actually work on a computer and need an OS

The list of things is nearly endless once you stoop to this level.
My problem is that to me, there is a huge difference between 'I have a vague idea about this' and 'I can teach this stuff in detail'. 
I've been asked more than once to put all this useless stuff on my CV, because this actually is what recruiters ctrl+f for...

## Still not enough

Endless lists of skills are one hurdle to get past the recruiters, but there is another.
This vile thing known as the IT certificate, in all its forms.
Now I don't mean anything related to SSL certificates, but those pieces of paper that 'prove' that you know stuff.
This might start with something like CompTIA A+, and in security typically ends with CISSP or something similar.
There are dozens of them out there, and almost all of them have one major flaw: it's about rote memorisation of stuff, and being able to reproduce it on an exam.
Read the book, memorise what's in it, take the test and pass, and now you are certified. 

One of these certificates close to my current line of work is the CEH or 'Certified Ethical Hacker', and this is often a requirement to get past the recruiters.
But CEH is useless!
What you learn is the names of various tools, some basics of hacking (on paper, don't actually do it), and other simple stuff.
A skiddy knows more, and is more capable that your typical CEH. That is, anyone with this certificate that is not already a hacker or penetration tester, and needs this certificate to get their foot in the door. 

## What to learn

A few months ago, I was asked to get certified, in order to become a trainer for a certain certificate. 
On a side note: yes, you can even become a trainer, creating more people in the workforce with the same certificates, fueling the problem.
In this particular case, it was about the ISACA CSX (cyber security fundamentals) certification. 
156 pages of info to cram, and take an exam online, a number of multiple choice questions.
As I already know this stuff, I had a slight problem unlearning things, because the study guide contains some information that did not agree with my knowledge.
At the exam, it's not about what you actually know, but what they put in the study guide, even though it is nonsense.
I must note that CSX is a rather new certificate, the study guide has a copyright statement for 2014, so we might assume that this knowledge is more or less up to date.

And so, I give you a few literal quotes from the study guide:

+ DES is no longer considered a strong cryptographic solution because its entire key space can be forced when every key is tried by large computer systems within a relatively short period of time. (That's putting it mildly.)

+ One form of advanced encryption algorithm is known as Triple DES or 3DES. (Yes, this is <em>advanced</em>, if rot13 is your idea of a basic crypto algorithm.)

+ (Regarding quantum crypto) Initial commercial usage has already started now that the laboratory research phase has been completed. (You might want to check with hyperelliptic, hashbreaker, or cryptojedi.)

+ Because of the key reuse problem and other flaws, the current standardized version of WEP does not offer strong enough security for most corporate applications.(Please, name <em>one</em> corporate application where this was a good idea in 2014.)

+ <em>The commonly exploited ports table on page 75 fails to mention port 22.</em>

+ <em>There is a whole paragraph on the Wireless Application Protocol (WAP) on page 85.</em> 

These are just a few of the issues I had with the study guide, and they worry me.
IT people are studying for this certificate, and are being told that WEP might not be the best idea, that DES is not that strong anymore, that WAP is still around, that quantum computers are actually a thing already (in 2014 even!), etcetera, etcetera.
And as this is a 'fundamental' certificate, so typically one of the first people get, they already get lies planted in their brains.
To add insult to injury, I now need to teach this to other people, in order for them to pass this exam and get certified.

## The CISSP-crowd

CISSP is one of the 'end-game' certs in security. 
You can only get it with at least five years of experience in the field, and someone holding a CISSP needs to vouch for you.
Because CISSP is about so much material, it can't go into depth anywhere.
A jack of all trades, master of none, and not even a practical jack at that.

Somehow non-technical people seem to think that if you have these letters, or others like them (CISM, CISA, CEH) next to your name, that you have practical abilities.
Thankfully, I am not alone in my aversion of CISSP, and other certifications.
Just see [Veracode][veracode], [attrition][attrition], [infosecisland][infosecisland], and [this comment on security musings][secmusings] for instance. 
As one of the links states: There is a reason there are CISSP jokes.

To keep your CISSP, you need to collect points and pay.
I've been to a few meetings where people could get points, and these meetings were useless for anything but getting those points.
If the information presented at such events is the first time you ever see this information, you're hopelessly outdated. 
People there even confirm that they are only attending to get the points, and they leave as soon as possible.

Certifications are a multibillion dollar business, and for the most part it does nothing but cost insane amounts of money and time.
And still, recruiters, managers, and sales are requiring these useless pieces of paper that tell you nothing about what a person can actually do. 

## One good cert
Is it all that bad?
Well, not really, but I told you I was going to rant, so I did.
There are some that do seem to get it right: Although I have not attempted this cert yet, I am fairly sure that there is at least one real value-adding certificate out there in security: OSCP.
And there is a good reason for it.
You can only obtain this certificate when you pass a practical test that requires you to use technical skills to break machines, and then to write a report on your findings.

Yes, you could say that I am bashing certs, and then plugging OSCP as something you should do.
But that is not my intention, it's just that this cert is one of the few I know of that actually require you to have practical skills rather than just theoretical and sometimes even downright erroneous knowledge. 

Unfortunately, I don't have a solution for the certificate problem.
Sifting through applicants is difficult, and if anything can reduce the set you need to look more closely at, it must be a good thing.
But please, don't pretend that a certificate is anything but a selection tool.

<b><em>It doesn't prove that you have technical skills.</em></b>

Sorry for the rant...


[veracode]: https://www.veracode.com/blog/2008/04/not-a-cissp/
[attrition]: http://attrition.org/security/conferences/why_you_should_not_get_a_CISSP-public.pdf
[infosecisland]: http://infosecisland.com/blogview/22257-Your-CISSP-is-Worthless-So-Now-What.html
[secmusings]: http://securitymusings.com/article/3020/isc2-and-the-cissp#comment-115904
