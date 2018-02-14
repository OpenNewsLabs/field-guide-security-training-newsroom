# Physical Custody of Electronics

## Overview

What happens to your data if your device is seized or stolen? How should you prepare to cross international borders safely? Full disk encryption can

This module makes a few assumptions about your threat model. It is written with American journalists in mind -- if your work puts you in conflict with hostile state actors, you should seek out more specialized training.

## About This Lesson Plan

**Review date:** June 5, 2017  
**Lesson duration:** 30 minutes  
**Level:** Intermediate  
**Preconditions:**

**What materials will participants need?**

They should bring their Android / iPhone and laptop.

**How should participants prepare?**

Participants will need administrator access to their machines.

**How should the instructor prepare?**

Touch base with IT staff to talk through your plans for the workshop -- you may need their support in actually enabling disk encryption.   

Read through the material carefully and think about what will work for you, as a facilitator and instructor.

## Lesson Plan

**Groundwork**

Digital security isn't just about encryption and data and metadata. The physical security of data and devices is also paramount: What happens to your data if your device is stolen? What's at risk if a border agent or other adversary takes your laptop for 30 minutes?

Physical custody issues generally boil down to two categories: permanent loss of your device, and temporary custody.

**Theft or Permanent Loss** You leave your backpack in a taxi. Your laptop disappears from your hotel room. A thief swipes your phone when you're standing on the sidewalk. What are the risks:

*Activity:* Have participants spell out their concerns. Capture them on a white board or sticky notes. If someone malicious takes your laptop, what do you need to worry about?

You're looking for things like:  

+ Someone else has your documents, password, address book, calendar.
+ You don't have them anymore, unless they're backed up.  
+ Sensitive work information, including documents, e-mails, communication about your reporting, communications from anonymous sources could be compromised.
+ You can't do your work because your hardware is gone.

**Seizure or Temporary Custody** Border agents seize your computer, but eventually return it to you. Your laptop is seized in a police or FBI investigation, and subsequently returned to you. You leave your laptop unattended -- in a hotel room, or office -- and someone tampers with it.

*Activity:* Again, have participants spell out their concerns. Capture them on a white board or sticky notes. If someone malicious takes your laptop, what do you need to worry about?

You're looking for most things from the first list, as well as things like:
+ someone can make a complete copy of the disk.
+ they can tamper with your device or install malware on it

**So what can you do?**
You can mitigate what is available without your permission. But "mitigation" is a key word. You don't know, not really, that it can't be decrypted. The strategies that make sense vary a lot with your threat model.   

Mitigation:

-   Mitigate the data available without your permission:

    -   Full disk encryption. (Note that at a border you may be detained
        > indefinitely or refused entry if you refuse to unlock
        > your device.)

-   Mitigate what data you carry on you in the first place:

    -   Border crossings: Consider using an alternate "travel device"
        > that does not contain things like passwords or keys or
        > sensitive work-related data. (SSH keys, GPG keys, password
        > manager database, work documents, e-mail client.)

        -   This is constrained by economics of the audience.
            > Organizations may have "travel devices" or may have easy
            > access to such infrastructure, but individuals may not
            > have the resources to have extra devices on-hand.

    -   1Password offers a [*travel
        > mode*](https://www.theverge.com/2017/5/23/15681990/1password-travel-mode-feature-added-security)
        > that won’t allow you to access to your passwords
        > while traveling.

    -   Send your data to a trusted party (friend, coworker, lawyer),
        > delete it from your device, and only receive access to it
        > again after you are in a safe situation. (Alternatively,
        > encrypt your data with a random key or password and give that
        > key or password to your contact.)

-   Mitigate risk of being affected by malware placed on your device
    > after it has left your custody.

    -   (Note that there are many levels of paranoia here, including
        > modification of the physical hardware of your device.)

    -   See entry about "travel devices" above.

    -   Border crossings: For smartphones, consider backing up your
        > device ahead of time and planning to wipe and restore your
        > device after crossing.

        -   (This can also be used to mitigate the amount of data you
            > carry back up & wipe your device ahead of time, only
            > maintain a minimum amount of information (important
            > contacts and immediate travel information) rather than all
            > of the data you would normally carry. Then restore your
            > "full" encrypted backup after a crossing. However, you may
            > be compelled to provide access and having such little data
            > on you may be a red flag.)

### Walkthrough: Full Disk Encryption

Disk encryption protects your data from being read if your device is
stolen. It only works when your device is turned off. It does not
provide protection if the adversary knows your device password.

< NOTE: Don't have participants enable FDE during your workshop. On a
smartphone it could take an hour or so, and on a laptop it could be take
as long as ten hours. Start the process in the evening and let it go
overnight. >

macOS:

Easy to turn on if you use
[*FileVault*](https://support.apple.com/en-us/HT204837)

-   In system preferences

    -   Security

    -   FileVault tab

    -   Enable FileVault

        -   Write down the recovery key on a piece of paper and store it
            > somewhere safe.

        -   Depending on your threat model, you might want to decline
            > the Apple iCloud recovery method. (State actors, targeted
            > attempts at your data,

Windows (Pro, Ultimate, or Enterprise editions only):

-   BitLocker
    > [*https://technet.microsoft.com/en-us/library/cc731549(v=ws.10).aspx*](https://technet.microsoft.com/en-us/library/cc731549(v=ws.10).aspx)

-   

Windows (alternative; if, for example, you only have Windows "Home
edition")

-   Veracrypt

    -   TK instructions / tutorial link

iOS

-   iOS has built-in device encryption as long as you have a
    > passcode enabled. (p. 10,
    > [*https://www.apple.com/business/docs/iOS\_Security\_Guide.pdf*](https://www.apple.com/business/docs/iOS_Security_Guide.pdf))

-   Pick a strong device passcode!

Android

-   Depends on the Android device. Nexus/Pixel devices have it on by
    > default (but you can double-check by doing the following
    > steps anyway).

-   In device settings:

    -   Security

    -   "Encryption" subsection

    -   "Encrypt phone"

        -   If given a "Secure start-up" option, choose to require it.

-   Make sure you have a strong passcode.

-   Your device is only secure as long as it is powered off, so


https://www.justsecurity.org/51759/dehumanized-border-travelers-push/

### Recommended Reading

**Links in the news**

+ [U.S. border agents stopped journalist from entry and took his phones (Washington Post, Nov 2016)](https://www.washingtonpost.com/news/the-switch/wp/2016/11/30/u-s-border-agents-stopped-journalist-from-entry-and-took-his-phones/)
+ [Department of Homeland Security detains journalist returning from Beirut (The Guardian, July 2016)](https://www.theguardian.com/media/2016/jul/21/homeland-security-journalist-maria-abi-habib-detained)
+ [A US-born NASA scientist was detained at the border until he unlocked his phone (The Verge, Feb 2017)](https://www.theverge.com/2017/2/12/14583124/nasa-sidd-bikkannavar-detained-cbp-phone-search-trump-travel-ban)
+ [Secret Service laptop containing Trump Tower evacuation and floor plans stolen (CNN, Mar 2017)](http://www.cnn.com/2017/03/17/politics/missing-secret-service-laptop/index.html)
+ [Privacy Complaints Mount Over Phone Searches at U.S. Border Since 2011](https://www.nytimes.com/2017/12/22/us/politics/us-border-privacy-phone-searches.html)
+ [“Dehumanized” at the Border, Travelers Push Back (Just Security, Feb 2018)](https://www.justsecurity.org/51759/dehumanized-border-travelers-push/)

+ [EFF 2017 Report on Digital Privacy at the US Boarder](https://www.eff.org/wp/digital-privacy-us-border-2017)

**More training resources**
