There's a third, related issue that is worth touching on as well: external drives. 

**External Drives** Someone gives you a USB drive with leaked files on it. What can you safely do with that drive?

Tip: think hard before you plug anything into your computer. 

No matter how hot it is, that free USB fan that Donald Trump and Kim Jong Un distributed to the press corps is probably a bad idea.

<blockquote class="twitter-tweet" data-conversation="none" data-lang="en"><p lang="nl" dir="ltr">13/ Handig. In de persmap voor de <a href="https://twitter.com/hashtag/KimTrumpSummit?src=hash&amp;ref_src=twsrc%5Etfw">#KimTrumpSummit</a> zit een mini usb fan. Handig om koel te blijven tijdens het schrijven. Het is hier in Singapore idd vrij heet. 33°C of zo. Maar haalt het niet bij Dubai, koning van de oven. <a href="https://t.co/6tQd5d7gCW">pic.twitter.com/6tQd5d7gCW</a></p>&mdash; Harald Doornbos (@HaraldDoornbos) <a href="https://twitter.com/HaraldDoornbos/status/1005746788303867905?ref_src=twsrc%5Etfw">June 10, 2018</a></blockquote>
<script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

https://twitter.com/HaraldDoornbos/status/1005746788303867905

https://twitter.com/UID_/status/1005795008581169152

# \[ Lesson Plan Name \]

## Overview
A lot of laptops nowadays have full disk encryption by default, but most external harddrives and USB keys do not. This lesson will go over the common security pitfalls and best practices, whether it's a free branded USB device from a conference, a 1TB hard drive bought on Amazon, or a harddrive of state secrets sent to you by a dubious hacking organization.

## About This Lesson Plan

**Review date:** \[ When was the last time this was reviewed or updated?\]  
**Lesson duration:** \[ Roughly how long should it take to lead participants through this lesson plan? 20 minutes? An hour? More? \]  
**Level:** Introductory 

**Preconditions**  
Passwords training

**What materials will participants need?**  
- Laptop (Windows, MacOS, or most Linuxes)
- Empty USB key

**How should participants prepare?**  
No prior preparation necessary.

**What materials will the instructor need?**  
- Projector
- Laptop 
- Blank USB key

**How should the instructor prepare?**  
The presenter would do well to go through the [full-disk encryption tutorials](https://github.com/OpenNewsLabs/field-guide-security-training-newsroom/blob/master/docs/Chapter02-09-Physical-Security.md) and understand the overall concepts.

**Advance email**  

TBD

\[ At least one possible email that a could send out to participants or crib from so that they come prepared. Eg. "Folks! On Friday in our weekly brown bag, I'm going to answer all your questions about making peanut butter sandwiches. Please be sure you've at least tasted peanut butter by then. You will need to bring two slices of bread. I'll have epi-pens and whole wheat bread. Please be sure to tell me if you can't eat wheat. If you have time I encourage you to read at least one of these excellent articles about why everyone should know how to make a peanut butter sandwich." \]

**Followup email**  

TBD

\[ at least one possible email that an intructor could follow up with. It should include:

+ a recap of the key points so participants can refer back to it,
+ some outside reference links for context
+ a followup exercise. Eg. "Thanks for coming to the peanut butter sandwich brown bag session. I'm attaching a link to an excellent YouTube video about spreading techniques. We talked about using a knife, choosing jams that spread well, and how to think about bread. Your homework is to make at least one sandwich with creamy PB and one with crunchy and report back to me by Tuesday on how that went." \]

## Lesson Plan

**Icebreakers/activities**  
- If you have the budget, get a USB key for each participant. Leave one on each desk, chair, or a pile on tables with a sign saying "one per user." To start the session ask people, "OK everyone, you each have a USB key. Did anyone try and check what's on it?"

- Review the [Stuxnet](https://en.wikipedia.org/wiki/Stuxnet#Natanz_nuclear_facilities) transmission story as an example of danger.

**Walkthrough or Active Lesson**  
\[ A hands on activity that will help participants either implement the tool -- ideally with some notes about stumbling blocks - or drive home the concept in a useful way. If you're installing or demonstrating a specific tool, make sure there's enough information here to get around potential roadblocks. \]

### Common Mistakes Make
- Laptop is encrypted but the backup is not.
- Received a free USB device at a conference or meeting and you plug it in to see what it does.
- Received a USB cable and just used it without thinking that it might have a surveillance device in it.
- Your phone is running low and you plug it into a random USB power port, not knowing what *that's* plugged into.

Have the group run the above scenarios discussing in just a few minutes what could be wrong with each situation.

Ensure that the following is hit on by the students:
- Backing up data is great, but if you encrypt your computer but not your hard drives the data is still insecure.
- Back up drives are easier to lose, steal, or forget about.
- USB keys can contain malware set to automatically run, and then hide itself as well
- USB cables can have chips hidden in them that can do the same as the previous point
- Ports that advertise as "power only" may not in fact be so.

### Mitigation Strategies

Disucss with students possible mitigation techniques for the above problem. The following points should be discussed if not brought up by the students themselves:

- Don't use USB keys you don't buy from a reputable store.
- Carry your own cables for your devices.
- You can buy "power only" USB cables. If you don't have one, use a power adapter and outlet instead of the port.
- Choose backup solutions that automatically encrypt your data (For instance, MacOS's Time Machine can be set to encrypt automatically)

### Practical Discussion

Explain to students that there are safe ways to share data using USB keys.

TD: explain and set through veracrypt.

## Recommended Reading

**Links in the news**  
\[ As many links as are useful to illustrate this concept or need for security. \]

* [Title of News Story (Outlet, Date)](URL)


**More great lesson plans**  
\[Links to as many other curricula and How-to articles that cover the same material as we can fit.\]

