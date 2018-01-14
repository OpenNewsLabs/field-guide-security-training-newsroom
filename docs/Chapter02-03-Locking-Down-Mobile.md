# Locking down your mobile devices

## Overview
This lesson plan will guide participants through the process of securing their mobile device by setting up a lockscreen and securing lockscreen notifications, applying system updates, and encrypting the device storage. This module is meant to act as the second in a series of three, building up a 60-75 minute training block on
secure mobile communications.

## About This Lesson Plan

**Review date:** June 6 2017  
**Lesson duration:** 30 mins (estimated),  longer if some Android phones need to be encrypted.  
**Level:** Intermediate. This session assumes participants are able to make a reliable backup of the key data on their phones and have done so very recently. If they haven't, you *should not* proceed.  

**Gotcha:** Consider how much time you have available before choosing to do this session. Are all your participants’ devices either brand new or recently [backed up](Chapter02-02-Mobile-Backups.md)? Do you have 30+ minutes and a low participant to trainer ratio? If not, you may want to either do this session in two parts on subsequent days (cover mobile device backups where you cover encrypted backups on one day, then actual encryption on the second day), *or* you share a link on backups and require participants to complete (or verify cloud backups) *before* this session.

**What will participants learn?**

Participants will learn how to set up a secure lockscreen and encrypt their mobile device storage. In conjunction with the previous lesson on [mobile application permissions hygiene](Chapter02-01-Mobile-Security-Settings.md), this prepares the device for the installation and use of a secure messaging system.

**What materials will participants need?**

They’ll need their mobile devices (iPhone or Android) and device chargers.

**How should participants prepare?**

Everyone should back up their mobile devices before the workshop. If folks haven't done that or aren't confident that they're backing up everything they need, start with a session on [mobile backups](Chapter02-02-Mobile-Backups.md).

**What materials will the instructor need?**

If you don’t already know the group well, make sure you’ve checked in about their technical capacity and check out Chapter 1 to make sure you’re planning ahead.

**How should the instructor prepare?**

You probably want participants to tell you in advance what phone OS they're using.

Read through:
<https://theintercept.com/2017/05/01/cybersecurity-for-the-people-how-to-keep-your-chats-truly-private-with-signal/#lockdown>

Consider setting a calendar appointment for a week after the training, to remind yourself to follow up with any participants who opted to put off updating or encrypting their phone. They're more likely to follow through if they get a reminder before too much time has passed.

## Lesson plan

**Introduction**  
Survey the room:

-   Who’s lost their phone before? (Bonus points for the best story! If anybody lost theirs and got it back, might be a good time to ask if they were worried about the time it spent out of their control)
-   Which device types people are using (iOS/Android/other? The "others" may need special attention)
-   How many already have a passcode or password lock screen set up?
-   How many have encryption set up?
-   How many apply updates regularly?

Spend some time on what makes a good passcode (length and randomness are good, birthdays and sequential numbers are bad). The [password](LINK TK) lesson has more great resources on this question.

**Walkthrough**  
Split people into groups by device types - instructions will differ for iOS vs Android. Everyone is going to ...

+ set a password or passcode,
+ review lockscreen notification settings,
+ check for system updates and apply them (or make a plan to apply them later). Note that system updates can sometimes take 20-30 minutes to download and install. In some cases it is more appropriate to


**Trainer notes:**
For *lock screens,* a strong password is always recommended. A PIN or passcode is an acceptable alternative, but it should be at least 6 digits long. For example, in the US you can be legally compelled to provide your biometrics to unlock a device by a court.

Biometric locking (eg. face or fingerprint recognition) is not recommended, as both are fakeable and do not offer the same degree of legal protection. For example, in the US you can be legally compelled to provide your biometrics to unlock a device by a court.

Android phones offer pattern locking, which is also problematic and not as secure as a pas

When you tackle *lockscreen notifications* keep in mind that some users may opt to keep convenient but insecure notifications coming for day to day use and change the settings when they're in more vulnerable situations or traveling.

*System Updates* can take 20-30 minutes or more to download and apply. In some cases it migth be more appropriate to have everyone check for system updates and commit to actually applying them later.

*Encrypting* a phone's hard drive can take even longer than a system update and this **should not** be undertaken unless the user is 100% confident that their data, settings, and authentication codes are backed up.

#### For iOS:

**Set a passcode:**

-   To set a passcode, open `Settings > Touch ID & Passcode` (it’s a little red icon with a fingerprint on it)
-   If you already have a passcode in place, you will be asked to re-enter your existing passcode.
-   Click "set passcode" to reset your passcode or create a new one. The default is a 6-digit code, but if you click "passcode options" you can also choose Custom Alphanumeric Code, Custom Numeric Code, and 4-Digit Numeric Code.
-   Enter your new passcode twice to verify it
-   You will also be asked for your Apple ID password to verify your new passcode
  -   The default setting for an iPhone with a passcode is that it is required "immediately" after locking the phone.
-   iPhones offer an "Erase Data," option. If you select it, __all data on the phone will be wiped after 10 failed passcode attempts__. This is strongly **not recommended** for clumsy people or people with small children.

**Secure lockscreen notifications:**
-   Open Signal and select the gear icon to open its settings
-   Select `Notifications > Background Notifications > Show`.
-   The "No name or message" option will ensure that Signal lockscreen notifications will not include  the senders name or message content.
-   To completely disable Signal notifications, or any other sensitive notifications, open the iOS Settings app, select `Notifications`, and change the notification settings for Signal and any other sensitive apps.

**Apply system updates:**

- Make sure your device is fully charged and connected to its charger. It’s also a good idea to backup your device data before applying system updates.
- Updates can take 20-30 minutes to download and install, and during that time the phone will be unusable.
- Open the Settings app and go to "General". If a software update exists, there will be a small, red circle with a 1 inside of it.
-   When you click through, choose "Software Update," > "Install Now," enter your passcode and let it run.

**Encryption**:
iPhones are already encrypted. Congratulations!

#### For Android:


**Set a passcode:**

-   Open the Settings app and select `Security >  Screen Lock`
-   Select a lock screen type. A strong password is the most secure option.
-   Depending on Android version, you may also be prompted to enable a setting called "Require password to start device" -- this setting will lock your device on startup, preventing it from receiving calls or messages until the password is entered. It’s recommended but not required.
-   Memorize and enter your new password or passcode.

**Secure lockscreen notifications:**
-   Open the Settings app, select `Sound & notification` and look for an option called `When device is locked`.
-   Select `hide sensitive notification content` (or `don't show notifications at all`). These options work, more ore less, as described.

**Apply system updates:**
Have everyone open the Settings app and check  `About Phone > System Updates`. If you do have an update waiting...
-   Make sure your device is fully charged and connected to its charger. It’s also a good idea to backup your device data before applying system updates.
-  Follow the on-screen instructions to apply any available updates.

**Encrypt your device:**
The process of encrypting a phone can take an hour or more. You should make sure that participants know their phone will be unavailable while it is being encrypted. Do not encourage anyone to encrypt their phone unless it is a new phone or they're 100% confident that everything on the [device is backed up](Chapter02-02-Mobile-Backups.md). If someone loses their authenticator app and doesn't have backup codes, they may have a very (very) difficult time restoring access. So just to reiterate: don't encourage anyone to encrypt their phone unless you're 100% confident that all the data and settings they need to restore their phone are backed up.

-  Make sure your device is fully charged and connected to its charger - encryption can take a while (an hour or more) and can not be interrupted once it starts.
-   Open the Settings app and select `Security > Encrypt phone`.
-   Follow the instructions to complete the encryption process.

## Follow Up
If anyone (or everyone) opted to put off applying system updates or encrypting their phone, make a plan to touch base in a week and remind them to set aside time to actually do it. 

## Recommended Reading

**Other Great Tutorials and Curriculum**

+ [Why You Should Be Encrypting Your Devices and How to Easily Do It](http://fieldguide.gizmodo.com/why-you-should-be-encrypting-your-devices-and-how-to-ea-1798698901)(Gizmodo, Sept 2017)
+ Mobile Phone Settings from [Me and My My Shadow:Tactical Tech' Training Curriculum](https://myshadow.org/train)

**Links in the News**

+ [John Kelly's personal cell phone was compromised, White House believe](http://www.politico.com/story/2017/10/05/john-kelly-cell-phone-compromised-243514), Politico, Oct 4, 2017

*Note: it would be great to include a few links to stories about phone search and seizure here. If you want to help the curriculum grow, we'd love your help adding recommended reading links. [Submit an  issue](https://github.com/OpenNewsLabs/newsroom-security-curricula/issues) or a pull request if you have good links to add.
