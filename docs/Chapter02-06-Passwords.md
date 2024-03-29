# Passwords and Password Management

## Overview
Passwords are the bedrock of account security, but hard to get right. This lesson provides a methodology for understanding how to take a harm reduction approach to password management. Participants should have a clear understanding of [phishing](Chapter02-08-Phishing.html) and [two-factor authentication](Chapter02-07-Two-Factor-Authentication.html), or you should cover those topics with Password Management.

## About This Lesson Plan

**Review date:** August 19, 2021<br />
**Lesson duration:**  Variable, depending on objectives and time available:
  1.  Overview, basic introduction, and securing primary email: **30 minutes**.
  2.  Strategies for protecting secondary accounts: **30 minutes**.
  3.  Setup and use of password managers: **30 minutes**<br />

**Level** Introductory  <br />
**Preconditions**

**What will participants learn?**

Participants will learn how to protect their online accounts, and how to understand the risk associated with compromises of those accounts. At a minimum, participants will learn how to choose a secure password, and use that skill, alongside two-factor authentication, to secure their primary email account.

They will also learn strategies to minimize possible exploits associated with reuse of passwords, including the use of delegated authentication and password managers.

**What materials will participants need?**

Their own laptop and (optionally) their phone.

**How should participants prepare?**

Read Martin Shelton’s Medium piece, [Journalists, You Are Worthy of a Data Breach](https://medium.com/@mshelton/journalists-you-are-worthy-of-a-data-breach-55f8e53fd3fe).

**What materials will the instructor need?**

A projector would help, but isn't essential.

**How should the instructor prepare?**

Read EFF's essays on [Harm Reduction](https://sec.eff.org/articles/harm-reduction) and [Knowing When You Are Out Of Scope](https://sec.eff.org/articles/out-of-scope) -- both are particularly relevant to this session.

1.  Get participants to tell you how they currently manage low-stakes passwords (eg. your Wordpress login, or your Walgreens Photo login). Most have a lot of logins saved in their browser -- find out which browser.

2.  Talk to IT: If you're working with a group in a single office, does their IT department have a preference? Anything they explicitly ban? Some organizations want staff to use a preferred solution for work passwords.

3.  Take your own medicine: configure a strong password and two-factor authentication for your primary email account.

4.  If you’re going to recommend a password manager make sure you try installing it across the platforms in use in your office, which might include MacOS X, Windows, Ubuntu, Android, and iOS. Even if you've been running the tool for a while, walking through a fresh install will help avoid surprises in the training.

5.  Read the lesson plan and think about how you want to structure sharing these core concepts with participants.

A deeper understanding of threat modeling, the high-level mechanics of delegated authentication, [password hashing](https://en.wikipedia.org/wiki/Cryptographic_hash_function#Password_verification), and encryption would also be helpful, though is by no means essential.

This is a lesson where it is very important to make sure that you, as the instructor, aren’t making things up or sharing bad information with participants. So be very clear and honest about what you don’t really know.<br />

**Harm Reduction** - a guiding principle of this lesson is that people will *not* use passwords properly, they will not store passwords securely, they will forget passwords, they will lose passwords, they will sign up for services that do not store passwords securely and those services will be hacked. The goal of this exercise is to *reduce the harm* that individuals (and the teams they work with) experience *when* (not if) things go wrong.

This is not a workshop that can guarantee that users will adopt strong, unique passwords
and strong two factor authentication in all situations. Not only is that goal unrealistic, it’s counter-productive because it’s an overwhelming goal for most people, and when people are overwhelmed they're more likely to give up. The reality is that if a good approach to passwords is used in just a few key places, a majority of the benefit and protection can be gained.

### Basic Digital Literacy (Accounts and Encryption)

There’s a lot of history and context to understanding *why* we have passwords in the first place, and too often this bit of digital literacy is missing. What it comes down to are two models of use for passwords:

1.  Service authentication - so a service can confirm that you are who you say you are
2.  Encryption - a key to unlock a secret lock

![Who are you, really?](img/ch2-6-1.png)

In the first case, a service has some data that’s associated with you. Because there’s no way to identify "you" on the internet, that data is normally tied to your email address. To gain access, the most common approach is to prove that you (1) know the password associated with your email address on that service or (2) have access to your email (and can then reset the password).

In the second case, the password is a mathematical key – there’s only one key to unlock the data, and using the key doesn’t prove anything about the identity of the person using the key, only that they have the key.

### Password Security (A Harm-Reduction Approach)

No one cares about passwords. No one should need to care about passwords. Passwords are never a means to an end, they’re a hurdle between us and the thing we want to do.

There are a few strategies that can be applied incrementally to increase personal security and simultaneously reduce friction to "doing the right thing."

There are two hard and fast rules:

1.  Password security does not need to be uniform. For most people, strongly securing your primary email address(es) will provide the biggest benefit for the least amount of effort.

2.  Passwords should not be reused.

And even rule #2 is not really that hard and fast: every security expert has a go-to password for those IDGAF moments -- hobbyist forums or your login to the local parents group -- forums where the worst case scenario is that someone uses your login to post spam or malicious content in your name.

You’re always better off if you don’t re-use passwords, but if you’re going to re-use passwords, you can probably safely use the same password for your neighborhood parents newsletter that you use on a game forum.

Lead a brief brainstorming exercise with participants to come up with different "classes" of accounts where reusing a password might be ok, so that they can think about the different security properties of those accounts in a concrete way. Some categories that they might come up with are: online shopping, games, discussion forums, commenting accounts on blogs, and so on).

## Lesson Plan

### Introduction

Start with a discussion of why we should care about passwords, and some of the consequences of getting them wrong. Martin Shelton has a [great writeup](https://medium.com/@mshelton/journalists-you-are-worthy-of-a-data-breach-55f8e53fd3fe) as a starting point -- we recommend asking folks to read it in advance.

Your discussion should cover these bases:
1. What passwords are for.
2. This system isn’t perfect.
3. Establishing a hierarchy.
4. Choosing and using a strong password.

### Secure Your Primary Email Account

Email is used by 99.9% of services as a password-reset mechanism, which means that if someone can gain access to your email, they can gain access to just about every other account you have. Because email is almost always the weakest link, securing email accounts is the absolute #1 priority for everyone. Thankfully, it’s easy!

#### Choosing a Strong Password

We’ll get to password managers later, but an email account is the main thing that someone will always need access to. For that reason, everyone should have a password that they remember *without writing it down* for their primary email.

[Security in a Box](https://securityinabox.org/en/) includes a great segment on [secure, unique, and memorable passwords](https://securityinabox.org/en/guide/passwords/) – this section is really an exercise in how to choose a password, and some of the reasons *why* it’s important to choose a strong password.

1.  Computers are really good at quickly guessing passwords (think millions of attempts per second).
2.  Modern storage means that lists of most passwords ever used, plus likely combinations are stored and available for download online.
3.  If someone can guess your password, it’s the easiest way to access your accounts, and the hardest to detect.

There are a few useful rules-of-thumb for choosing a password:

1.  Make it long – the longer the password, the harder it is to crack.
2.  Make it complex – the more variation of characters you use, the harder it is to crack. Use punctuation, non-latin characters, and numbers in addition to upper- and lower-case latin characters.
3.  Make it practical – a password isn’t helpful if you can't remember it.
1.  Don't make it personal – don’t use personally identifiable information (eg. family names, birthdates) in your password.
2.  Keep it secret – never share your password. A password must be a secret between you and the service you use it on. This is especially true for your email password. Never, ever share your email password with anyone, and never use it on any other sites or services.

The strategy we'd recommend is to come up with a short password based on a memorable phrase. To quote Tactical Tech:

> Passwords can also take advantage of more traditional mnemonic devices, such as the use of acronyms. This allows long phrases to be turned into complex, seemingly-random words:
>
> 'To be or not to be? That is the question' becomes '2Bon2B?TitQ'
>
> 'We hold these truths to be self-evident: that all men are created equal' becomes 'WhtT2bs-e:taMac='
>
> 'Are you happy today?' becomes 'rU:-)2d@y?'
>
> These are just a few examples to help you come up with your own method of encoding words and phrases to make them simultaneously complex and memorable.

🐇 DISTRACTION ALERT: Many participants will have heard of some other strategy for developing a strong memorable password. As long as your password is long, practical, and complex, you’re good. Don’t get lost comparing password strategies or sharing stories.

**Activity:** Everyone should come up with a secure password and change their email password so that it is strong and secure.

> Links to change passwords for common email providers:
>
> Google: <https://www.google.com/settings/passwordchange>
>
> Microsoft / Outlook: <https://account.live.com/password/reset>
>
> Apple iCloud: <https://support.apple.com/en-us/HT201355>

#### Keeping that Password Secure

If you force yourself to type your email password every time you check your email, you’ll do a much better job of remembering your password. But a strong password isn’t enough to keep your email safe. You also need to enable [two-factor authentication](Chapter02-07-Two-Factor-Authentication.html). If you haven't already covered 2FA, do it now.

Slightly trickier is securing other central services. The same basic rules apply: secure, unique password plus 2FA. Examples of these services include: Apple ID (for participants with iPhones, iPads, or Macs), Google Account (especially for Android, even if not using GMail), Facebook, Twitter, WhatsApp, Signal.

**Activity:** Have participants brainstorm a list of these "primary accounts" that offer special access to their phones, messaging, etc.

Either have everyone set a secure password and enable 2FA or have everyone make that list and assign password resetting as homework.

#### Never, Ever Reuse Passwords

If you reuse the same password all over the place, you run the risk that one service’s poor password management will compromise all of your accounts. Troy Hunt's [Have I Been Pwned?](https://haveibeenpwned.com/) is a great resource for tracking database breaches to see if your username or email address is included in the latest batch of pwned accounts. It's also a great teaching tool for your participants - chances are, at least one of their email addresses is listed for at least one service. If they are, and they reused a password for that service, their other logins are also at risk.

The challenge is that **not** reusing passwords is really inconvenient. So there are a few strategies you can use to avoid worrying about it:

#### Option 1: Password Manager
Using a password manager is the most secure approach. It is also the most unwieldy, and it isn't without tradeoffs. Martin Shelton has a [great roundup of password managers](https://medium.com/@mshelton/password-managers-for-beginners-d1f49866f80f). You want a password manager that will keep your passwords accessible if you lose access to your primary computer, but won’t store them in plain text or make them available to anyone who shouldn’t have them.

Martin’s review covers [Bitwarden](https://bitwarden.com), [1Password](https://1password.com/), and [KeePassXC](http://keepassxc.org), all of which are excellent solutions. Note that if you go with KeePassXC, [Martin Shelton’s installation guide](https://medium.com/@mshelton/keypass-for-beginners-dc8adfcdad54) is the best way to get it running on OSX.

Some people think password managers are annoying and terrible. Some people genuinely love them. They are not a silver bullet. As a trainer you should share what works for you, but make sure participants understand that your preferred solution isn't their only option.

**Activity:** Installing a password manager together. As the trainer, you should pick one and have everyone install the same one. Have everyone ...

1. Export their saved browser passwords. In Firefox, users can export passwords saved in the browser by typing "about:logins" into their search bar (or navigate to `Settings` > `Privacy & Security` > `Saved Logins` > `...` (three-dot menu). In Chrome users should be able to go to "chrome://settings/passwords" (or navigate to `Settings` > `Autofill` > `Passwords` > `...` (three-dot menu, under `Saved Passwords`).
2. Install the password manager that you’ve decided to focus on.
3. Set a strong password for the password manager vault.
4. Decide where to store the vault.
4. Import their stored browser passwords and...
  * delete them from the browser
  * disable password storage
5. Add a browser plugin to integrate the password manager with their primary web browser.

Now everyone is in a good position to use the password manager as their primary password repository for a while and decide whether or not it is a fit.

*Note:*  The password manager exercise might seem like a good opportunity to change *all* their passwords to secure unique passwords, but this isn't typically practical in the time available. We recommend starting by just moving from your current system (which is probably a combination of sticky notes and passwords saved in the browser) to a password manager, and focusing on changing key passwords. Once they have a password manager set up, people can replace old passwords with more secure versions as they use them.

### Option 2: Use Your Inbox

Remember that we're taking a harm reduction approach here. Some people just won’t use a password manager. If you already know your team isn’t on board, or if folks try a password manager and confess that it didn’t stick, this is a slate of "good enough" strategies:

1.  Have everyone strongly secure their primary email account. If you only do one thing, do this.

2.  Encourage everyone to use single sign on wherever it is available (This is "Sign In With Google" or "Sign in With Facebook"). If you have secured your single sign on account, this is a good option. Click approve the first time, any subsequent login is automatic but **still secure**. Note: make sure every one knows how to watch for the difference between using Facebook or Google to sign  in and giving an app or service permission to access your Facebook or Google data. Sign-in With Google is totally secure and fine, but be very careful about what other access you grant apps that are using Google Sign-In. Don’t just "click okay" and accept whatever access they are asking for. (Note to trainers: consider covering [Mobile Security Settings](Chapter02-01-Mobile-Security-Settings.html) to ensure that participants understand this.)

3.  Use the "reset my password by email" link. It’s very secure (almost as secure as single sign-on) and as long as you don’t use a weak or reused password to start, it guarantees that no-one will be able to sign in as you later without access to your account.
    *  Use a random password and don’t save it! Especially for sites you don’t visit often, just using a throw-away password can be the most secure thing.
    * Use a password manager to generate a password; if you can reset the password later with an email link, then you don’t need to worry about the password manager backups, etc.

More notes about harm reduction: Many security experts will recoil at this strategy. They're right: password managers are far more secure, but this is a viable backup option for those who can’t or won’t use a purpose-built password manager.

Participants should take stock of all the points of entry to their email inboxes: are messages stored locally on their phone or laptop? Will someone who accesses their laptop or phone have access to all of their account information? Remind participants that this strategy is good enough for most threat models but won't protect them from police search, for instance.


### Follow Up
-   Homework: if you assigned 2FA or password resets as homework, be sure to send everyone a follow up note reminding them to DO IT.

-   Remind everyone to disable stored passwords and set up the password manager on their secondary computer and on their phone.

-   Remind everyone to take stock of whether they’re still using their password manager. If they are, a week out is a good moment to look at all the other places

## Recommended Reading

**Password Dumps in the news**
-   <https://www.wired.com/2012/08/apple-amazon-mat-honan-hacking/>
-   <https://www.buzzfeednews.com/article/blakemontgomery/one-billion-more-yahoo-accounts-have-been-hacked>
-   <https://www.wired.com/story/yahoo-breach-three-billion-accounts/>
-   <https://krebsonsecurity.com/2013/10/adobe-breach-impacted-at-least-38-million-users/>
-   <https://haveibeenpwned.com/>
-   <https://www.espn.com/mlb/story/_/id/13089501/report-fbi-investigating-st-louis-cardinals-hacking-houston-astros-database>
-   <https://www.accessnow.org/doubleswitch-attack/>
-   <https://www.wsj.com/articles/the-man-who-wrote-those-password-rules-has-a-new-tip-n3v-r-m1-d-1502124118>
-   <https://www.csoonline.com/article/3266607/1-4b-stolen-passwords-are-free-for-the-taking-what-we-know-now.html>
+  [Twitter discovered 336 million passwords stored in plaintext](https://www.wired.com/story/change-your-twitter-password-right-now/) (that is, not encrypted) on an internal server. They [don't think](https://blog.twitter.com/official/en_us/topics/company/2018/keeping-your-account-secure.html) that anyone actually accessed the password list, but the announcement is a good reminder that re-using passwords is a bad practice, precisely because you can't assume that services outside your control are storing your password responsibly. (Wired, May 2018)
+  [Collection #1](https://www.troyhunt.com/the-773-million-record-collection-1-data-reach/) is a massive, multi-site breach that includes 773M email address with a combined total of 1.16B username/passwords combinations. (January 2019)
