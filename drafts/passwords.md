NOTE: when this is migrated, it will need a link to the two factor authentication lesson and the phishing lession. 
===================================================================================================================

Password Management
===================

**Overview:** Passwords are the bedrock of account security, but hard to
get right. This lesson provides a methodology for understanding how to
take a harm reduction approach to password management. Participants
should have a clear understanding of phishing (LESSON LINK TK) and two
factor authentication (LESSON LINK TK), or you should cover those topics
with Password Management.

**ABOUT THIS LESSON PLAN**

**Review date:** Oct 5, 2017

**Lesson duration:**

Variable, depending on objectives and time available:

1.  Overview, basic introduction, and securing primary email: **30
    > minutes**.

2.  Strategies for protecting secondary accounts: **30 minutes**.

3.  Setup and use of password managers: **30 minutes**.

**What will participants learn?**

Participants will learn how to protect their online accounts, and how to
understand the risk associated with compromises of those accounts. At a
minimum, participants will learn how to choose a secure password, and
use that skill, alongside two-factor authentication, to secure their
primary email account.

They will also learn strategies to minimize possible exploits associated
with reuse of passwords, including the use of delegated authentication
and password managers.

**What materials will participants need?**

Their own laptop and (optionally) their phone.

**How should participants prepare?**

Read Martin Shelton’s Medium piece, \[Journalists, You Are Worthy of a
Data
Breach\]([*https://medium.com/@mshelton/journalists-you-are-worthy-of-a-data-breach-55f8e53fd3fe*](https://medium.com/@mshelton/journalists-you-are-worthy-of-a-data-breach-55f8e53fd3fe))

**What materials will the instructor need?**

A projector would help, but isn’t essential.

**How should the instructor prepare?**

1.  Get participants to tell you how they currently manage low-stakes
    > passwords (eg. your Wordpress login, or your Walgreens
    > Photo login). Most have a lot of logins saved in their browser --
    > find out which browser.

2.  Talk to IT! Does your IT department have a preference? Anything they
    > explicitly ban? Some organizations want staff to use a preferred
    > solution for work passwords.

3.  Take your own medicine: configure a strong password and two-factor
    > authentication for your primary email account.

4.  If you’re going to recommend a password manager make sure you try
    > installing it across the platforms in use in your office, which
    > might include MacOS X, Windows, Ubuntu, Android, and iOS. Even if
    > you’ve been running the tool for a while, walking through a fresh
    > install will help avoid surprises in the training.

5.  Read the following and think about how you want to structure sharing
    > these core concepts with participants.

A deeper understanding of threat modelling, the high-level mechanics of
delegated authentication, password hashing, and encryption would also be
helpful, though is by no means essential.

This is a lesson where it is very important to make sure that you, as
the instructor, aren’t making things up or sharing bad information with
participants. If you find yourself saying “I don’t really know how that
works but the way I’ve always thought about is that it is a little like
bears and ice chests” keep in mind that 50% of the people in the room
will hear “the expert thinks this is just like bears and ice chests.” So
be very clear and honest about what you don’t really know.

**Harm Reduction** - a guiding principle of this lesson is that people
will *not* use passwords properly, they will not store passwords
securely, they will forget passwords, they will lose passwords, they
will sign up for services that do not store passwords securely and those
services will be hacked. The goal of this exercise is to *reduce the
harm* that individuals (and the teams they work with) experience *when,*
(not if) things go wrong.

This is not a workshop that can guarantee that strong, unique passwords
and strong two factor authentication will be used in all situations. Not
only is that goal unrealistic (impossible!), it’s counter-productive
because it’s an overwhelming goal for most people, and more likely to
lead to people giving up and adopting unsafe practices everywhere. The
reality is that if a good approach to passwords is used in just a few
key places, a majority of the benefit and protection can be gained.

### Basic Digital Literacy (Accounts and Encryption)

There’s a lot of history and context to understanding *why* we have
passwords in the first place, and too often this bit of digital literacy
is missing.

What it comes down to are two models of use for passwords:

1.  Service authentication - so a service can confirm that you are who
    > you say you are

2.  Encryption - a key to unlock a secret lock

![](media/image2.png){width="3.125in" height="3.4895833333333335in"}

In the first case, a service has some data that’s associated with you.
Because there’s no way to identify “you” on the internet, that data is
normally tied to your email address. To gain access, the most common
approach is to prove that you (1) know the password associated with your
email address on that service or (2) have access to your email (and can
then reset the password).

In the second case, the password is a mathematical key – there’s only
one key to unlock the data, and using the key doesn’t prove anything
about the identity of the person using the key, only that they have the
key.

### Password Security (A Harm-Reduction Approach)

No one cares about passwords. No one should need to care about
passwords. Passwords are never a means to an end, they’re a hurdle
between us and the thing we want to do.

There are a few strategies that can be applied incrementally to increase
personal security and simultaneously reduce friction to “doing the right
thing.”

There are two hard and fast rules:

1.  Password security does not need to be uniform. For most people,
    > strongly securing your primary email address(es) will provide the
    > biggest benefit for the least amount of effort.

2.  Passwords should never be reused.

And even rule \#2 is not really that hard and fast: every security
expert has a go-to password for those IDGAF moments -- hobbyist forums
or your login to the local parents group -- forums where the worst case
scenario is that someone uses your login to post spam or malicious
content in your name.

**LESSON PLAN**

### Introduction

Start with a discussion of why we should care about passwords, and some
of the consequences of getting them wrong. Martin Shelton has a [*great
writeup*](https://medium.com/@mshelton/journalists-you-are-worthy-of-a-data-breach-55f8e53fd3fe)
as a starting point.

#### You want to cover: 

1)  What passwords are for.

2)  This system isn’t perfect.

3)  Establishing a heirarchy.

4)  Choosing and using a strong password.

### Secure Your Primary Email Account

Email is used by 99.9% of services as a password-reset mechanism, which
means that if someone can gain access to your email, they can gain
access to just about every other account you have. Because email is
almost always the weakest link, securing email accounts is the absolute
\#1 priority for everyone. Thankfully, it’s easy!

#### Choosing a Strong Password

We’ll get to password managers later, but an email account is the main
thing that someone will always need access to. For that reason, everyone
should have a password that they remember *without writing it down* for
their primary email.

[*Security in a Box*](https://securityinabox.org/en/) includes a great
segment on [*secure, unique, and memorable
passwords*](https://securityinabox.org/en/guide/passwords/) – this
section is really an exercise in how to choose a password, and some of
the reasons *why* it’s important to choose a strong password.

1.  Computers are really good at quickly guessing passwords (think
    > millions of attempts per second).

2.  Modern storage means that lists of most passwords ever used, plus
    > likely combinations are stored and available for download online.

3.  If someone can guess your password, it’s the easiest and hardest to
    > detect way of gaining access to your accounts.

A good set of rules-of-thumb for choosing a password:

1.  Make it long – the longer the password, the harder it is to crack.

2.  Make it complex – the more variation of characters you use, the
    > harder it is to crack. Use punctuation, non-latin characters, and
    > numbers in addition to upper- and lower-case latin characters.

3.  Make it practical – a password isn’t helpful if you can’t
    > remember it.

<!-- -->

1.  Don't make it personal – don’t use personally identifiable
    > information (e.g., yours or family’s names, birthdates, etc) in
    > your password.

2.  Keep it secret – never share your password with others. A password
    > must be a secret between you and the service you use it on. This
    > is especially true for your email password. Never, ever share your
    > email password with anyone, and never use it on any other sites.

The strategy we’d recommend is to come up with a short password based on
a memorable phrase. To quote Tactical Tech:

> Passwords can also take advantage of more traditional mnemonic
> devices, such as the use of acronyms. This allows long phrases to be
> turned into complex, seemingly-random words:
>
> 'To be or not to be? That is the question' becomes '2Bon2B?TitQ'
>
> 'We hold these truths to be self-evident: that all men are created
> equal' becomes 'WhtT2bs-e:taMac='
>
> 'Are you happy today?' becomes 'rU:-)2d@y?'
>
> These are just a few examples to help you come up with your own method
> of encoding words and phrases to make them simultaneously complex and
> memorable.

🐇 DISTRACTION ALERT: Many participants will have heard of some other
strategy for developing a strong memorable password. As long as your
password is long, practical, and complex, you’re good. Don’t get lost
comparing password strategies or sharing stories.

**Activity:** Everyone should come up with a secure password and change
their email password so that it is strong and secure.

> Links to change passwords for common email providers:
>
> Google:
> [*https://www.google.com/settings/passwordchange*](https://www.google.com/settings/passwordchange)
>
> Hotmail:
> [*https://account.live.com/password/change*](https://account.live.com/password/change)
>
> Apple iCloud:
> [*https://support.apple.com/en-us/HT201355*](https://support.apple.com/en-us/HT201355)

#### Keeping that Password Secure

If you force yourself to type your email password every time you check
your email, you’ll do a much better job of remembering your password.
But a strong password isn’t enough to keep your email safe. You also
need to enable two-factor authentication.

#### Two Factor Authentication

If you haven’t already covered 2FA, do that now.

#### [*Two-factor Authentication*](https://docs.google.com/document/d/198q22aHCYSduD0jBCXFn3qh3i4mULUjZhpbHgxBEBZQ/edit) – LINK TK (post migration)

#### Securing Additional Accounts

Slightly trickier is securing other central services. The same basic
rules apply: secure unique password plus 2FA. Examples of these services
include: Apple ID (for participants with iPhones, iPads, or Macs),
Google Account (especially for Android, even if not using GMail),
Facebook, Twitter, WhatsApp, Signal.

**Activity:** Have participants brainstorm a list of these “primary
accounts” that offer special access to their phones, messaging, etc.

Either have everyone set a secure password and enable 2FA or have
everyone make that list and assign password resetting as homework.

### Never Reuse Passwords

If you reuse the same password all over the place, you run the risk that
one service’s poor password management will compromise all of your
accounts. \[Have I Been
Pwned?\]([*https://en.wikipedia.org/wiki/Have\_I\_Been\_Pwned%3F*](https://en.wikipedia.org/wiki/Have_I_Been_Pwned%3F))
is a great resource but the real takeaway is that everyone, everywhere
has been pwned somewhere along the line. So don’t reuse passwords.

The problem is that **not** reusing passwords is really inconvenient. So
there are a few strategies for **not** worrying about it:

**Option 1:** Use a password manager. This is the most secure approach.
It is also the most unwieldy. Martin Shelton has a [*great roundup of
password
managers*](https://medium.com/@mshelton/password-managers-for-beginners-d1f49866f80f).
You want a password manager that will keep your passwords accessible if
you lose access to your primary computer, but won’t store them in plain
text or make them available to anyone who shouldn’t have them.

Martin’s review covers LastPass, [*1Password*](https://1password.com/)
or [*KeePass*](http://keepass.info/), all of which are excellent
solutions. Note that if you go with KeePass, [*Martin Shelton’s
installation
guide*](https://medium.com/@mshelton/keypass-for-beginners-dc8adfcdad54)
is the best way to get it running on OSX.\
\
Some people think password managers are annoying and terrible. Some
people genuinely love them. They definitely are not a silver bullet. As
a trainer you should share what works for you, but make sure
participants understand that your preferred solution isn’t their only
option.

**Activity: **

Have everyone…

-   Export their saved browser passwords. There’s a [*good Firefox
    > plugin*](https://addons.mozilla.org/en-US/firefox/addon/password-exporter/)
    > for this, in Chrome users should be able to go
    > to &lt;chrome://flags/\#password-import-export&gt;.

-   Install the password manager that you’ve decided to focus on.

-   Set a strong password for the password manager vault.

-   Import their stored browser passwords and (this is key!) delete them
    > from the browser and disable password storage.

Now everyone is in a good position to use the password manager as their
primary password repository for a while and decide whether or not it is
a fit.

*Note:* Some trainers feel strongly that everyone should use the
password manager exercise as an opportunity to change all their
passwords to secure unique passwords, but that adds a layer of work
before you’ve even figured out whether this tool will work. So we
recommend starting by just moving from your current system (which is
probably a combination of sticky notes and passwords saved in the
browser) to a password manager. This

**Option 2:** Some people just won’t use a password manager. If you
already know your team isn’t on board, or if folks try a password
manager and confess that it didn’t stick, this is a slate of strategies
that is good enough in many cases:

1.  Strongly secure your primary email account. If you only do one
    > thing, do this.

2.  Use “Sign In With \[Google/Facebook/etc\]”\
    > \
    > If you have secured your primary email account, this is a good
    > option and is the easiest option. (click approve the first time,
    > any subsequent login is automatic but **still secure**).\
    > \
    > Watch for the difference between using Facebook or Google to sign
    > in and giving the app or service permission to access your
    > Facebook or Google data.\
    > \
    > Sign-in With Google is totally secure and fine, but be very
    > careful about what other access you grant apps that are using
    > Google Sign-In. Don’t just “click okay” and accept whatever access
    > they are asking for. (Note: there’s a whole workshop on working
    > with mobile apps in this curriculum. It’s worth addressing.)

3.  Use the “reset my password by email” link. It’s very secure (almost
    > as secure as “sign in with \[google/etc\]”) and as long as you
    > don’t use a weak or reused password to start, it guarantees that
    > no-one will be able to sign in as you later without access to
    > your account.

    a.  Use a random password and don’t save it! Especially for sites
        > you don’t visit often, just using a throw-away password can be
        > the most secure thing. This has the added benefit in a legal
        > situation that if someone asks you for the password, you
        > *literally don’t know it*.

    b.  Use a password manager to generate a password; if you assume
        > that you can reset the password later with an email link, then
        > you don’t need to worry about the password manager
        > backups, etc.

4.  Email passwords to yourself. As long as you’re confident that your
    > email account is secure and only accessible to you, and the
    > passwords aren’t reused, this is a perfectly good option, because
    > anyone who has access to your email account can almost certainly
    > sign in to any of your accounts already.\
    > \
    > Many security experts will recoil at the thought of this, and
    > participants should be *encouraged* to use password managers, but
    > this is a viable backup option for those who can’t or won’t use a
    > purpose-built password manager.

### Failure Modes

We’re addressing a few different scenarios with good password policies.
These include: non-targeted hacking by spammers and scammers that can
still make your life absolutely miserable by cutting off access to
infrastructure you rely on like credit cards and email; targeted hacking
with a financial goal -- someone wants access to your money and things;
targeted hacking with a personal goal -- someone wants access to you.
They know exactly who you are and want to make your life miserable or
expose you or use you as a stepping stone to reach another target.

There’s a good chance that no-one is going to follow all of the advice
offered as part of this lesson. They’ll make mistakes, and use weak
passwords and reuse passwords. They won’t consistently use a password
manager, and when they do, there’s a chance that they’ll expose
themselves to significant risk by losing control of (or access to) their
password vault. Offering strategies to minimize the effect of that “risk
seeking behaviour” is possibly the most valuable advice that can be
given to participants.

Create a hierarchy accounts. For example, passwords for really core
stuff should be secure, and each should be unique. As above, some of
those include (but aren’t limited to):

-   Primary email account

-   Your laptop’s password

-   Banking passwords

-   Apple or Google ID connected to a phone

Secondary things might include:

-   Services where you’ve stored credit card information (eg. retailers,
    > car services, course registration). Note that one way to move
    > these logins down the hierarchy is to remove your stored
    > credit card.

-   Mileage accounts

Even Less important things:

-   Forums and services that don’t have stored credit card information.

You’re always better off if you don’t re-use passwords, but if you’re
going to re-use passwords, you can probably safely use the same password
for your neighborhood parents newsletter that you use on a sewing forum.

Lead a brief brainstorming exercise with participants to come up with
different “classes” of accounts where reusing a password might be ok, so
that they can think about the different security properties of those
accounts in a concrete way. Some categories that they might come up with
are: online shopping, games, discussion forums, commenting accounts on
blogs, and so on).

**Follow Up**

-   Homework: if you assigned 2FA or password resets as homework, be
    > sure to send everyone a follow up note reminding them to DO IT.

-   Remind everyone to disable stored passwords and set up the password
    > manager on their secondary computer and on their phone.

-   Remind everyone to take stock of whether they’re still using their
    > password manager. If they are, a week out is a good moment to look
    > at all the other places

**Recommended Reading**

**Links in the news**

**Reports on Password Dumps**

-   [*https://www.wired.com/2012/08/apple-amazon-mat-honan-hacking/*](https://www.wired.com/2012/08/apple-amazon-mat-honan-hacking/)

-   [*https://www.buzzfeed.com/blakemontgomery/one-billion-more-yahoo-accounts-have-been-hacked*](https://www.buzzfeed.com/blakemontgomery/one-billion-more-yahoo-accounts-have-been-hacked)

-   [*https://www.wired.com/story/yahoo-breach-three-billion-accounts/*](https://www.wired.com/story/yahoo-breach-three-billion-accounts/)

-   [*http://krebsonsecurity.com/2013/10/adobe-breach-impacted-at-least-38-million-users/*](http://krebsonsecurity.com/2013/10/adobe-breach-impacted-at-least-38-million-users/)

-   [*https://haveibeenpwned.com/*](https://haveibeenpwned.com/)

-   [*http://www.espn.com/mlb/story/\_/id/13089501/report-fbi-investigating-st-louis-cardinals-hacking-houston-astros-database*](http://www.espn.com/mlb/story/_/id/13089501/report-fbi-investigating-st-louis-cardinals-hacking-houston-astros-database)

-   [*https://www.accessnow.org/doubleswitch-attack/*](https://www.accessnow.org/doubleswitch-attack/)

-   [*https://www.wsj.com/articles/the-man-who-wrote-those-password-rules-has-a-new-tip-n3v-r-m1-d-1502124118*](https://www.wsj.com/articles/the-man-who-wrote-those-password-rules-has-a-new-tip-n3v-r-m1-d-1502124118)

Big picture readings
