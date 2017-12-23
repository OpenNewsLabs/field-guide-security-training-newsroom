Physical Custody of Electronics &\
Full Disk Encryption
==================================

**Overview:** Digital security isn't just about encryption and data and
metadata. The physical security of data and devices is also paramount:
What happens to your data if your device is stolen? What's at risk if a
border agent or other adversary takes your laptop for 30 minutes? We'll
discuss these security aspects and ways to protect yourself from the
associated risks.

**ABOUT THIS LESSON PLAN**

**Review date:** June 5, 2017

**Lesson duration:** 30 minutes

**What will participants learn?**

What's at risk when you lose custody of your devices, say at an
international border. How to protect your data from device theft with
full disk encryption.

**What materials will participants need?** smartphone, laptop

**How should participants prepare?**

For laptops, a participant needs to have administrator access to their
machine so that they can change system settings to enable disk
encryption.

**What materials will the instructor need?**

**EXAMPLE MESSAGING FOR PARTICIPANTS**

**Links in the news**

-   [*https://www.washingtonpost.com/news/the-switch/wp/2016/11/30/u-s-border-agents-stopped-journalist-from-entry-and-took-his-phones/*](https://www.washingtonpost.com/news/the-switch/wp/2016/11/30/u-s-border-agents-stopped-journalist-from-entry-and-took-his-phones/)

-   [*https://www.theguardian.com/media/2016/jul/21/homeland-security-journalist-maria-abi-habib-detained*](https://www.theguardian.com/media/2016/jul/21/homeland-security-journalist-maria-abi-habib-detained)

-   [*https://www.theverge.com/2017/2/12/14583124/nasa-sidd-bikkannavar-detained-cbp-phone-search-trump-travel-ban*](https://www.theverge.com/2017/2/12/14583124/nasa-sidd-bikkannavar-detained-cbp-phone-search-trump-travel-ban)

-   [*http://www.cnn.com/2017/03/17/politics/missing-secret-service-laptop/index.html*](http://www.cnn.com/2017/03/17/politics/missing-secret-service-laptop/index.html)

**Advance email**

**Followup email**

**LESSON PLAN**

**Icebreakers/activities**

**Walkthrough or Active Lesson**

(This is more of a guide of the subject matter and things to touch on or
relay in your own teaching; probably not a literal lesson plan.)

Digital security isn't just about encryption and data and metadata. The
physical security of data and devices is also paramount: What happens to
your data if your device is stolen? What's at risk if a border agent or
other adversary takes your laptop for 30 minutes?

The physical custody issues generally boil down to two categories: theft
/ permanent loss of your device, and temporary custody.

**Theft / Permanent Loss**

Examples: You left your backpack in a taxi. Your laptop disappears from
your hotel room. A thief swipes your phone when you're standing on the
sidewalk.

Risks:

-   Your data (documents, passwords, address book, calendar, etc.)
    > are stolen.

    -   Is it a work device? Do you have sensitive work information
        > (documents, e-mails or other communication about your
        > reporting, communications from anonymous sources)?

Mitigations:

-   Full disk encryption (we'll get to this below)

-   Backups of your data

**Temporary Custody**

Examples: Border agents seizing your device and then returning it to
you. "Evil maid" attack: you leave your laptop in a hotel room or
sitting around in your office or some other place temporarily
unattended. (The border crossing case has unique legal and operational
risks that go well beyond this summary guide; for more information,
[*the EFF has a
report*](https://www.eff.org/wp/digital-privacy-us-border-2017)
focussing on these issues at the U.S. border.)

Risks:

-   Your data (documents, passwords, address book, calendar, etc.)
    > are stolen.

    -   (As above: is this a work device? If so, what types of
        > work-sensitive information is at risk?)

    -   Border or police agent (Department of Homeland Security /
        > Homeland Security Investigations / ICE / La Migra) takes a
        > copy of the full disk of your device.

-   Your device has been tampered with and contains malware.

Mitigation:

-   Mitigate what data is available without your permission:

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
