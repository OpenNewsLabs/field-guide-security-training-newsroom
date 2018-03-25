# Chapter 2: Lesson Plans

This chapter includes lesson plans for the most common newsroom needs. If there's a lesson you're looking for and you don't see it here, definitely [let us know](https://github.com/OpenNewsLabs/field-guide-security-training-newsroom/issues). If you have a favorite resource that you think we should include, we'd love to hear about that, too. 

Every lesson plan includes an overview of the lesson, prerequisites and materials that trainers and participants will need, and a good walk through of the tool and concepts. If you run one of these lessons and find that it goes a lot faster (or a lot slower) than our estimate, we want to know. Each lesson concludes with a round up of links in the news that illustrate the importance of the material in the lesson, and a round up of links to other teaching resources that cover the material well. If you have resources that should be included in those link round ups, please do share them with us. 

## What Is Included

**[Mobile Security Settings](Chapter02-01-Mobile-Security-Settings.html)**  <br />
This is the first short module in a series of three trainings dedicated to securing your mobile device. In this module, iPhone and Android users will learn how to review the security settings on their mobile devices. In later trainings, they will learn how to encrypt their device, set a secure locking mechanism, and install an encrypted messaging system (Signal). These three modules are meant to be short and simple. Each can serve as a quick win in a larger session about something else, or can stand alone as a short session. Or the three mobile sessions can combine nicely into a 60- to 75-minute block of training around securing a mobile device.

**[Locking Down Mobile](Chapter02-02-Locking-Down-Mobile.html)**  <br />
This lesson plan helps participants secure their mobile devices by setting up lockscreens and securing lockscreen notifications, applying system updates, and encrypting device storage. This module is meant to act as the second in a series of three, building up a 60-75 minute training block on secure mobile communications.

**[Setting Up Signal](Chapter02-03-Setting-Up-Signal.html)** <br /> 
Signal is a secure messaging platform that utilizes end-to-end encryption. Before starting this lesson, participants should have already been through a [mobile application settings review](Chapter02-01-Mobile-Security-Settings.html) and added secure lockscreens to ensure that their device is ready to use with a program like Signal. Some benefits of Signal: they do not store messages on their servers, participants can set their conversations to "self-destruct," and users can customize what information (contact name, message preview) is available on their phone's lockscreen. This lesson plan is intended to be taught as the third in a series, following [mobile app security settings](Chapter02-01-Mobile-Security-Settings.html) and [locking down mobile devices](Chapter02-02-Locking-Down-Mobile.html).

**[Mobile Backups](Chapter02-04-Mobile-Backups.html)** <br /> 
Creating regular, secure backups of data on mobile devices is important, whether users want to protect against loss, theft, or catastrophic error (e.g. accidentally wiping a device while encrypting it). This session covers the creation of encrypted backups for iOS and Android users, and make recommendations on a backup schedule.

**[Good Hygiene for Apps](Chapter02-05-Good-Hygiene-For-Apps.html)**  <br />
Overview: Don't let orphaned apps degenerate into an unlocked back door to your account.

**[Passwords and Password Management](Chapter02-06-Passwords.html)**  <br />
Passwords are the bedrock of account security, but they're hard to get right. This lesson explains how to take a harm-reduction approach to password management. Participants should have a clear understanding of [phishing](Chapter02-08-Phishing.html) and [two-factor authentication](Chapter02-07-Two-Factor-Authentication.html), or you should cover those topics as part of this lesson.

**[Two-Factor Authentication](Chapter02-07-Two-Factor-Authentication.html)**  <br />
Enabling two-factor authentication (2FA) is one of the easiest steps people can take to protect their online accounts. Even if someone gets ahold of a user's password, 2FA will ensure that they can't get very far. 2FA adds extra protection by requiring additional information for login, which is provided by text message, a code from an authenticator app, or the use of a hardware security key. This lesson plan introduces key concepts about 2FA, and guides participants through the process of setting up app-based 2FA for their primary email accounts.

**[Phishing](Chapter02-08-Phishing.html)** <br /> 
Phishing is an email-based social engineering tactic that uses misplaced trust to extract information and access. Like other forms of social engineering, its purpose is to trick you (the target) into divulging information that can be used to gain access to private data, networks or resources. Participants will learn about phishing in the context of trust decisions, and develop awareness and techniques to make these decisions when interacting on the web.

**[Physical Security](Chapter02-09-Physical-Security.html)**  <br />
What happens to a person's data if their device is seized or stolen? How should people prepare to cross international borders safely? This session discusses ways to approach border crossings, and walks through the process of enabling full-disk encryption, which can help ensure that someone who has a physical device doesn't necessarily have access to all its data. This module makes a few assumptions about participants' threat models, and is written with American journalists in mind. If participants' work puts them in conflict with hostile state actors, they should seek out more specialized training.

**[Scrubbing Metadata](Chapter02-10-ScrubbingMetadata.html)** <br /> 
Files such as Word documents and JPEG images usually contain information about the systems used to create them. This information, commonly referred to as metadata, could inadvertently reveal personally identifiable details about sources to anyone given access to the files. This lesson plan teaches participants how to find metadata in Word documents and JPEG files, and ways to share or publish content from these files without exposing metadata.

**[Secure Drop](Chapter02-11-SecureDrop.html)** <br /> 
SecureDrop is an anonymous whistleblowing tool designed to provide users with a high degree of protection from detection through Internet-based surveillance. This lesson plan covers the keys to using SecureDrop effectively: establishing a culture of security, setting up SecureDrop securely, and making sure sources know how to use it safely.


## What Is Not Included

This guide doesn't currently include a guide to encrypting email with GPG or PGP. Why? It's hard to use, and history has shown that most folks don't use it properly. As Martin Shelton has pointed out, [newsrooms have better options](https://source.opennews.org/articles/how-lose-friends-and-anger-journalists-pgp/). However, there are use cases when GPG is the best option. If you want to [help build this resource](contributing.html), we welcome a lesson plan that introduces email encryption. There are a few good resources out there on the subject: This one, from [Riseup](https://riseup.net/en/security/message-security/openpgp/best-practices), is a good start.
