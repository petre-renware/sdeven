*RENware Software Systems*    
**Software Development Methodology**

Version: 0.4.10    
Last update: 220415

***

# Code Review (SDEVEN.68-COREV)

**Table of Content**

[TOC]

## Preamble and goals

This section is about code review. So, **what can be expected** from a code review?

* Sharing knowledge
* Sharing responsibility
* Improving code structure
* Learning

*A good code review covers all those aspects.*

**What are the goals?**

* The main purpose is to "detect" those code parts that can be generalized and reused
* Another purpose is to check the conformity to appropriate standards and practices (for example for a Python code to check if it respects PEP indications, or for a web server front end application if HTML specifications was followed, etc)

## Tools

But code review is just a technique, if we'll use a tool for that, we can throw code review away.

## Mob programming technique as tool

***Mob programming*** means *all team members* are present in the same time in front of one screen. Or work remotely on a shared screen — that is my case.

First (the team or its leader) decide for a task (or issu*e treated as next action), and when possible we rotate in ***driving sessions***. A session means there is *a one driver* — one who types / clicks, and *one navigator* — which tells the driver what to do. The other team members **keeps attention**, and only when the navigator goes in a wrong direction, then **interrupts**. Navigator navigates for 3 (max 5) minutes and then rotate.

Rotation means that driver now navigates — should know next step, navigator takes a rest, and others of the drives but less than half of them. And after 3 minutes another rotation, and again, …

This rotation style is intense. You have to keep attention all the time, otherwise you’ll have to navigate in couple of minutes, and you’ll have no idea how to navigate (by ***you*** is meant the team leader).To stay in shape we do regular breaks for bathroom / coffee, and of course a long break for a lunch. Goals of code view are fulfilled

Sharing knowledge is instant — every team member follows the mental process, and knows why was what done.
Sharing responsibility in my opinion full — I take responsibility for everything that we produce as I can anytime say “I disagree” or “I have a better idea”.
Code structure is agreed by all team members, therefore is consistent and the best team members can do.
Learning… is again instant, and intense. If the navigator is good, they’ll not only call what to do, but also how to do it efficiently. I learn daily better software architecture, better testing strategies, how to use IDE efficiently, … just because navigators know (and share) pieces I’m missing.

--- ooo ---