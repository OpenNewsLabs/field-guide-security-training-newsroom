

**Working structure for this chapter document**

-   Introduction/how we’ve grouped these lessons
-   What you’ll find inside a lesson plan
-   MVP curriculum -- suggested set of lessons to get a newsroom started?
-   Lessons
-   Threats to understand
-   Things you can do to improve your personal security
    -   Basic
    -   Advanced
-   Things your newsroom can do to improve institutional security

# Chapter 2: Lesson Plans

This chapter includes lesson plans for the most common newsroom needs. If there's a lesson you're looking for and you don't see it here, definitely [let us know](https://github.com/OpenNewsLabs/field-guide-security-training-newsroom/issues) and if you have a favorite resource that you think we should include, we'd love to hear about that, too. 

## What is Included

[Mobile Security Settings](docs/Chapter02-01-Mobile-Security-Settings.md) -- This is the first short training module in a series of three trainings dedicated to securing your mobile device. In this module, participants will learn how to review the security settings on their mobile devices (for iPhone and Android users). In later trainings, they will learn how to encrypt their device, set a secure locking mechanism, and install an encrypted messaging system (Signal). These three modules are meant to be short and simple. Each can serve as a quick win in a larger session about something else, or can stand alone as a short session. Or the three mobile sessions can combine nicely into a 60- to 75-minute block of training around securing a mobile device.

[Mobile Backups](docs/Chapter02-02-Mobile-Backups.md) -- Creating regular, secure backups of data on your mobile devices is important, whether you want to protect against loss, theft, or catastrophic user error (eg. accidentally wiping your device while encrypting it). This session will cover the creation of encrypted backups for iOS and Android users, and make recommendations on a backup schedule. Even if you don't get on a regular schedule, you should always backup your phone before you make any major changes to it.

[Locking Down Mobile](docs/Chapter02-03-Locking-Down-Mobile.md) -- This lesson plan will guide participants through the process of securing their mobile device by setting up a lockscreen and securing lockscreen notifications, applying system updates, and encrypting the device storage. This module is meant to act as the second in a series of three, building up a 60-75 minute training block on secure mobile communications.

[Setting Up Signal](docs/Chapter02-04-Setting-Up-Signal.md) -- Signal is a secure messaging platform that utilizes end-to-end encryption. Participants should have already been through a [mobile application settings review](Chapter02-01-Mobile-Security-Settings.md) and added secure lock screens, to ensure that their device is now ready to use with a program like Signal.

Benefits of Signal include the fact that they do not store your messages on their servers, participants can set their conversations to "self-destruct" and users can customize what information (contact name, message preview) is available on their phones lock screen.

This lesson plan is intended to be taught as the third in a series, following [mobile app security settings](Chapter02-01-Mobile-Security-Settings) and [locking down mobile devices](Chapter02-03-Locking-Down-Mobile.md).

[Good Hygeine for Apps](docs/Chapter02-05-Good-Hygiene-For-Apps.md) -- Overview:  Don't let orphaned apps degenerate into an unlocked back door to your account.

[Passwords and Password Management](docs/Chapter02-06-Passwords.md) -- Passwords are the bedrock of account security, but hard to get right. This lesson provides a methodology for understanding how to take a harm reduction approach to password management. Participants should have a clear understanding of [phishing](Chapter02-08-Phishing.md) and [two factor authentication](Chapter02-07-Two-Factor-Authentication.md), or you should cover those topics with Password Management.

[Two Factor Authentication](docs/Chapter02-07-Two-Factor-Authentication.md) --
Enabling two-factor authentication (2FA) is one of the easiest steps you can take to protect your online accounts. Even if someone gets ahold of your password, 2FA will ensure that they can't get very far. 2FA adds extra protection by requiring additional information for login, provided by either a text message to your phone, a code from an authenticator app, or the use of a hardware security key.

This lesson plan will introduce key concepts about 2FA, and guide you through the process of setting up app-based 2FA for your primary email account.

[Phishing](docs/Chapter02-08-Phishing.md) -- *Phishing* is an email-based social engineering tactic that uses misplaced trust to extract information and access. Like other forms of social engineering, its purpose is to trick you (the target) into divulging information that can be used to access to  private data, networks or resources. *Spear-phishing* is a form of phishing targeted at a particular individual or group. This sort of attack is widespread, common, and responsible for many [notorious examples](https://en.wikipedia.org/wiki/Podesta_emails) of data loss or leakage.

Defending against phishing begins with *awareness* of particular risks and some basic safety *techniques* and can be aided by the use of certain *tools*.

Participants will consider phishing in the context of *trust decisions* and develop awareness and techniques to make these decisions when interacting on the web. Participants will learn the basic mechanics of phishing and spear-phishing, the techniques attackers may use, how to approach online trust decisions, and important, basic techniques and tools.

[Physical Security](docs/Chapter02-09-Physical-Security.md) --What happens to your data if your device is seized or stolen? How should you prepare to cross international borders safely? This session will talk about ways to approach border crossings, as well as walk through the process of enabling full disk encryption, which can help ensure that someone who has your physical device doesn't necessarily have all your data.

This module makes a few assumptions about your threat model. It is written with American journalists in mind -- if your work puts you in conflict with hostile state actors, you should seek out more specialized training.

[Scrubbing Metadata](docs/Chapter02-10-ScrubbingMetadata.md) --Files such as Word documents and JPEG images usually contain information about the systems used to create them. This information, commonly referred to as metadata, could inadvertently reveal personally identifiable details about your sources to anyone given access to the files. Removing metadata from files provided by sources before sharing or publishing them is critical for anonymous source protection.

This lesson plan covers what you'll need to know to find file metadata in Word documents and JPEG files, and how you can share or publish content from these files without exposing metadata.

[Secure Drop](docs/Chapter02-11-SecureDrop.md) -- SecureDrop is an anonymous whistleblowing tool, built on well-tested cryptographic technologies, and designed to provide its users with a high degree of protection from detection through Internet-based surveillance. This lesson plan covers what you'll need to know to use SecureDrop effectively: establishing a culture of security, setting up SecureDrop securely, and making sure your sources know how to use it safely.


## What is not included:

This guide doesn't currently include a guide to encrypting email with GPG or PGP. Why? It's hard to use and history has shown that most folks don't use it properly. As Martin Shelton has pointed out, [newsrooms have better options](https://source.opennews.org/articles/how-lose-friends-and-anger-journalists-pgp/). However, there are use cases when GPG is the best option. If you want to [help build this resource](docs/contributing.md), we welcome a lesson plan that introduces email encryption.
