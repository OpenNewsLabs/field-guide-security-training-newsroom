# Physical Custody of Electronics

## Overview

What happens to your data if your device is seized or stolen? How should you prepare to cross international borders safely? This session will talk about ways to approach border crossings, as well as walk through the process of enabling full disk encryption, which can help ensure that someone who has your physical device doesn't necessarily have all your data.

This module makes a few assumptions about your threat model. It is written with American journalists in mind -- if your work puts you in conflict with hostile state actors, you should seek out more specialized training.

## About This Lesson Plan

**Review date:** June 5, 2017<br />
**Lesson duration:** 30 minutes<br />
**Level:** Intermediate<br />
**Preconditions:** Participants should know how to back up their devices and how to choose a strong passphrase.

**What materials will participants need?**

They should bring their Android / iPhone and laptop.

**How should participants prepare?**

Participants will need administrator access to their machines.

Everyone should read [Digital Privacy at the U.S. Border: Protecting the Data On Your Devices (EFF 217)](https://www.eff.org/wp/digital-privacy-us-border-2017).

**How should the instructor prepare?**

Touch base with IT staff to talk through your plans for the workshop -- you may need their support in actually enabling disk encryption. <br />

Read through the material carefully and think about what will work for you, as a facilitator and instructor.

Assume that no more than 50% of participants will actually read the EFF guide that you sent around.

**Follow up**

Because most participants will not actually turn on full disk encryption during the session, set a deadline for everyone to do it and then be sure to follow up.

## Lesson Plan

**Groundwork**

Digital security isn't just about encryption and data and metadata. The physical security of data and devices is also paramount: What happens to your data if your device is stolen? What's at risk if a border agent or other adversary takes your laptop for 30 minutes?

Physical custody issues generally boil down to two categories: permanent loss of your device, and temporary custody.

**Theft or Permanent Loss** You leave your backpack in a taxi. Your laptop disappears from your hotel room. A thief swipes your phone when you're standing on the sidewalk. What are the risks:

*Activity: Have participants spell out their concerns. Capture them on a white board or sticky notes. If someone malicious takes your laptop, what do you need to worry about?*

You're looking for things like:<br />

+ Someone else has your documents, password, address book, calendar.
+ You don't have them anymore, unless they're backed up.<br />
+ Sensitive work information, including documents, e-mails, communication about your reporting, communications from anonymous sources could be compromised.
+ You can't do your work because your hardware is gone.

**Seizure or Temporary Custody** Border agents seize your computer, but eventually return it to you. Your laptop is seized in a police or FBI investigation, and subsequently returned to you. You leave your laptop unattended -- in a hotel room, or office -- and someone tampers with it.

*Activity:* Again, have participants spell out their concerns. Capture them on a white board or sticky notes. If someone malicious takes your laptop, what do you need to worry about?

You're looking for most things from the first list, as well as things like:
+ someone can make a complete copy of the disk.
+ they can tamper with your device or install malware on it

**So what can you do?**
You can mitigate what is available without your permission. But "mitigation" is a key word. You don't know, not really, that it can't be decrypted. The strategies that make sense vary a lot with your threat model. The EFF's [Border Privacy Guide](https://www.eff.org/wp/digital-privacy-us-border-2017) is a great resource -- encourage folks to lean hard on it.

+ Reduce the amount of data you carry across the border, or don't carry sensitive data across borders at all. This is in some ways the easiest solution, at least as far as border search is concerned. It is also, obviously the hardest.

  + If you have access to a secondary laptop and you're planning a trip, consider taking something other than your primary laptop to use. If you do use an alternate "travel device" and make sure that it doesn't contain your password manager, SSH keys or e-mail client.

  + Do you need a smart phone on your trip? Or would a feature phone with longer battery life meet your needs?

  + Consider backing up, and completely wiping your phone before you leave on a trip. You can restore your device either after crossing or when you're back home.

  + Government authorities in particular, may be able to modify the physical hardware of your device. Restoring software from a backup won't protect against hardware modifications.

+ Use a "travel mode": 1Password offers a [travel mode](https://www.theverge.com/2017/5/23/15681990/1password-travel-mode-feature-added-security) that won’t allow you to access your passwords while traveling.

+ Minimize the data available without your permission with full disk encryption, but know that you may not always be able to cross international borders without unlocking a device. The EFF has a good overview of [your rights at the US border](https://www.eff.org/wp/digital-privacy-us-border-2017#part-2). *Trainer Note: it is easy to slip into a debate about what the border patrol is likely to do, or a story swapping session about horrible things that have happened. Try to "park" those stories in a "parking lot" for discussion another time.*

+ Call a lawyer. If your newsroom has staff attorneys, touch base with them before you travel.

  + Some attorneys recommend telling the border agents that your device contains trade secrets and you're not authorized to authorize a search. That obviously only applies if it is true, but if you have company correspondence or documents on your phone it probably is true. <br />

  + Carry key phone numbers outside your phone: if you find yourself in a situation where you are able to contact an attorney but don't want to power up your phone, make sure you have their number written down somewhere. Business cards are excellent for this purpose.

  + Even if you don't have a staff attorney, do make sure you have someone you can contact if you get into a stand off over your electronics at the border. And make sure that you have their number somewhere analog.

### Walkthrough: Full Disk Encryption

What does full disk encryption protect: disk encryption protects data against being read when your computer is off, or newly powered on.

What does it not protect: if your device is already powered up, the drive is decrypted, even if the screen is locked. Once you enter your passphrase, the disk is decrypted.
If someone has your passphrase, either because it was guessable or because you gave it to them, full disk encryption won't protect you.

**Important**: the process of enabling FDE can take many hours, and if you interrupt it you will lose access to everything that was on the disk. So show participants how it works, but **do not have them start the process** until they're sure that a) they have backed up the machine and b) they can live without it for 10-12 hours. Generally that means leaving it over night.

Make sure everyone knows where to find the disk encryption settings on their devices and has a plan to actually enable it when they can do so safely.


#### MacOS:

Use [FileVault](https://support.apple.com/en-us/HT204837).

In `system preferences > Security > FileVault` you should see a toggle labeled `Enable FileVault`. When you are ready to actually encrypt the disk always write down the recovery key on a piece of paper and store it somewhere safe.

Depending on your threat model, you might want to decline the Apple iCloud recovery method, as it may leave your data vulnerable to state actors.

#### Windows (Pro, Ultimate, or Enterprise editions):

Use [BitLocker](https://technet.microsoft.com/en-us/library/cc731549(v=ws.10).aspx).

Users that only have  Windows "Home edition" can look into Veracrypt.

#### iOS:

iOS has built-in device encryption ([see page 10](https://www.apple.com/business/docs/iOS_Security_Guide.pdf)) -- but it is only as good as your passphrase.<br />

#### Android:

Options will depend on the Android device. Nexus/Pixel devices have full disk encryption enabled by default, but you can double-check by going to `Device Settings > Security > Encryption` -- select `Encrypt phone` to start the process, and be sure to set a strong passphrase.

### Recommended Reading

**Links in the news**

+ [U.S. border agents stopped journalist from entry and took his phones (Washington Post, Nov 2016)](https://www.washingtonpost.com/news/the-switch/wp/2016/11/30/u-s-border-agents-stopped-journalist-from-entry-and-took-his-phones/)
+ [Department of Homeland Security detains journalist returning from Beirut (The Guardian, July 2016)](https://www.theguardian.com/media/2016/jul/21/homeland-security-journalist-maria-abi-habib-detained)
+ [A US-born NASA scientist was detained at the border until he unlocked his phone (The Verge, Feb 2017)](https://www.theverge.com/2017/2/12/14583124/nasa-sidd-bikkannavar-detained-cbp-phone-search-trump-travel-ban)
+ [Secret Service laptop containing Trump Tower evacuation and floor plans stolen (CNN, Mar 2017)](http://www.cnn.com/2017/03/17/politics/missing-secret-service-laptop/index.html)
+ [Privacy Complaints Mount Over Phone Searches at U.S. Border Since 2011](https://www.nytimes.com/2017/12/22/us/politics/us-border-privacy-phone-searches.html)
+ [“Dehumanized” at the Border, Travelers Push Back (Just Security, Feb 2018)](https://www.justsecurity.org/51759/dehumanized-border-travelers-push/)

+ [Digital Privacy at the U.S. Border: Protecting the Data On Your Devices (EFF 217)](https://www.eff.org/wp/digital-privacy-us-border-2017)

**More training resources**

+ [Digital Privacy at the U.S. Border: Protecting the Data On Your Devices (EFF 217)](https://www.eff.org/wp/digital-privacy-us-border-2017)
