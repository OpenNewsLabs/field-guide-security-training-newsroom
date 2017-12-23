Locking down your mobile devices
================================

## Overview FIX This lesson plan will guide participants through the
process of securing their mobile device by setting up a lockscreen and
securing lockscreen notifications, applying system updates, and
encrypting the device storage. This module is meant to act as the second
in a series of three, building up a 60-75 minute training block on
secure mobile communications.

**ABOUT THIS LESSON PLAN**

**Review date:** June 6 2017 (reviewed by CW)

**Lesson duration:** 30 mins (estimated) \[could be longer if some
Android phones need to be encrypted\]

**Gotcha:** Consider how much time you have available before choosing to
do this session. Are all your participants’ devices either brand new or
recently backed up? Do you have 30+ minutes \*and\* a low participant to
trainer ratio? If not, you may want to either do this session in two
parts on subsequent days (cover mobile device backups where you cover
encrypted backups on one day, then actual encryption on the second day),
*or* you share a link on backups and require participants to complete
(or verify cloud backups) *before* this session.

**What will participants learn?**

Participants will learn how to set up a secure lockscreen and encrypt
their mobile device storage. In conjunction with the previous lesson on
mobile application permissions hygiene, this prepares the device for the
installation and use of a secure messaging system (which participants
will set up in the next lesson).

**What materials will participants need?**

They’ll need their mobile devices (iPhone or Android) and device
chargers.

**How should participants prepare?**

They should backup their mobile devices, if possible, before the
training begins.

**What materials will the instructor need?**

If you don’t already know the group well, make sure you’ve checked in
about their technical capacity and check out Chapter 1 to make sure
you’re planning ahead.

**How should the instructor prepare?**

Read through:

[*https://theintercept.com/2017/05/01/cybersecurity-for-the-people-how-to-keep-your-chats-truly-private-with-signal/\#lockdown*](https://theintercept.com/2017/05/01/cybersecurity-for-the-people-how-to-keep-your-chats-truly-private-with-signal/#lockdown)

**Level**: intro

**Preconditions**: This should happen in conjunction with the app
permissions lesson, as a precursor to setting up Signal.

**Additional Precondition/Gotcha:** Participants should \*not\* actively
encrypt their devices for the first time during this session unless
their devices are either brand new *or* they are certain they have a
recent backup available. This is in case something goes wrong during the
encryption process so they do not use their data.

**LESSON PLAN**

**Introduction**

Survey the room and ask:

-   Who’s lost their phone before? (Bonus points for the best story! If
    > anybody lost theirs and got it back, might be a good time to ask
    > if they were worried about the time it spent out of their control)

-   Which device types people are using (iOS/Android/other? The “others”
    > may need special attention)

-   How many already have a passcode or password lock screen set up?

-   How many have encryption set up?

-   How many apply updates regularly?

Spend some time on what makes a good passcode (length and randomness
good, birthdays and sequential numbers bad).

**Walkthrough or Active Lesson**

Split people into groups by device types - instructions will differ for
iOS vs Android.

For iOS:
--------

Trainer notes: Password is recommended, passcode is acceptable if 6
digits or longer. Biometric locking (fingerprint) is not recommended, as
they’re fakeable and do not have the same degree of legal protection
(i.e. You could be legally compelled to provide your biometrics to
unlock a device by a court).

**Set a passcode:**

-   To set a passcode, open Settings > go to Touch ID & Passcode
    > (it’s a little red icon with a fingerprint on it)

-   If you already have a passcode in place, you will be asked to
    > re-enter your existing passcode.

-   Click “set passcode” to reset your passcode or create a new one. The
    > default is a 6-digit code, but if you click “passcode options” you
    > can also choose Custom Alphanumeric Code, Custom Numeric Code, and
    > 4-Digit Numeric Code.

-   Enter your chosen passcode twice to verify it

-   You will also be asked for your Apple ID password to verify your new
    > passcode

-   The default setting for an iPhone with a passcode is that it is
    > required “immediately” after locking the phone.

-   iPhones also have a setting called “Erase Data,” which allows you to
    > require all data on the phone to be wiped after 10 failed
    > passcode attempts. This is strongly **not recommended** for
    > incredibly clumsy people or people with small children.

**Secure lockscreen notifications:**

-   Open the Signal app and select the gear icon to open its settings

-   Select **Notifications / Background Notifications / Show**.

-   Select **No name or message**. With this option, Signal lockscreen
    > notifications will not contain the sender name or message content.

-   To completely disable Signal notifications, or any other sensitive
    > notifications, open the Settings app, select **Notifications**,
    > and change the notification settings for Signal and other
    > sensitive apps.

**Apply system updates:**

\[Trainer notes: this may take a while. Be sure to let participants know
that it may take upward of 20-30 minutes to download and install the
software update, as they may wish to do this on their own time, after
the training is over.\]

-   Make sure your device is fully charged and connected to its charger.
    > It’s also a good idea to backup your device data before applying
    > system updates.

-   Open the Settings app and go to General. If a software update
    > exists, there should be a small, red circle with a 1 inside of it.

-   When you click through, choose “Software Update,” choose “Install
    > Now,” enter your passcode and let it run.

**Encryption**:

iPhones are already encrypted. Congratulations!

For Android:
------------

\[Trainer notes: Password is recommended, PIN is acceptable if 6 digits
or longer, pattern unlock is problematic. Biometric locking (face,
fingerprint) is not recommended, as they’re fakeable and do not have the
same degree of legal protection. Android OS flavors and device
manufacturer versions may move these settings around, so you may have to
help people look for them \]

**Set a passcode:**

-   Open the Settings app and select **Security / Screen Lock** - (this
    > option may be available in a different section of the Settings app
    > on some versions of Android)

-   Select a lock screen type. Password is potentially the most secure
    > type, PIN is less secure but may be more convenient. Other methods
    > that are pattern-based or rely on biometric data are
    > not recommended.

-   Depending on Android version, you may be prompted to enable “Require
    > password to start device” - this option will lock your device on
    > startup, preventing it from receiving calls or messages until the
    > password is entered. It’s recommended but not required.

-   Memorize and enter your new password or passcode. If you use a
    > password, it should be relatively strong - don’t include
    > dictionary words, don’t reuse passwords. If you use a PIN, random
    > is best, and PINs derived from personal information such as
    > birthdays or significant dates should be avoided. PINs should have
    > at least 6 digits, the more the better.

**Secure lockscreen notifications:**

-   Open the Settings app, and select **Device / Sound & notification /
    > When device is locked**.

-   Select **Hide sensitive information content**. With this option,
    > lockscreen notifications will not contain any
    > sensitive information. (This will apply to all applications, not
    > just Signal.)

**Apply system updates:**

\[Trainer notes: this may take a while. It should be done before
encryption, and if you’re doing multiple lesson plans you should
consider leaving this until you’ve worked through the other plans, or
timing this plan to be followed by a break\]

-   Make sure your device is fully charged and connected to its charger.
    > It’s also a good idea to backup your device data before applying
    > system updates.

-   Open the Settings app and select **About Phone / System Updates**

-   If a system update is available, follow the on-screen instructions
    > to apply it.

**Encrypt your device:**

\[Trainer notes: this may take a while, an hour or more for some
devices. You should make sure that participants know their phone will be
unavailable while it is being encrypted, and if you’re doing multiple
lesson plans you might want to consider leaving encryption until last.\]

I’d recommend NOT doing this unless they have a new phone or they’re
100% sure everything on their device si

-   Make sure your device is fully charged and connected to its
    > charger - encryption can take a while (an hour or more) and should
    > not be interrupted.

-   Open the Settings app and select **Security / Encrypt phone.**

-   Follow the instructions to complete the encryption process.

<!-- -->

-   

**LINKS**

**Other Tutorials and Curriculum**

[*Why You Should Be Encrypting Your Devices and How to Easily Do It
*](http://fieldguide.gizmodo.com/why-you-should-be-encrypting-your-devices-and-how-to-ea-1798698901)(Gizmodo,
Sept 2017)

[*Mobile Phone Settings, Hands-on; My Shadow: (Tactical
Tech*](https://myshadow.org/train)’s Road Tested Curriculum)

**Links in the News**

John Kelly's personal cell phone was compromised, White House believe,
Politico, Oct 4, 2017

http://www.politico.com/story/2017/10/05/john-kelly-cell-phone-compromised-243514
