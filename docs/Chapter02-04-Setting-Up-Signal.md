# Setting Up Signal

## Overview
Signal is a secure messaging platform that utilizes end-to-end encryption. Participants should have already been through a [mobile application settings review](/docs/Chapter02-01-Mobile-Security-Settings.md) and added secure lock screens, to ensure that their device is now ready to use with a program like Signal.

Benefits of Signal include the fact that they do not store your messages on their servers, participants can set their conversations to "self-destruct" and users can customize what information (contact name,
message preview) is available on their phones lock screen.

This lesson plan is intended to be taught as the third in a series, following [mobile app security settings](/docs/Chapter02-01-Mobile-Security-Settings/) and [locking down mobile devices](/docs/Chapter02-03-Locking-Down-Mobile.md).

## About This Lesson Plan

**Review date:** June 6, 2017  
**Lesson duration:** 15-30 minutes  
**Level:** Beginner

### Preconditions
This lesson assumes users have already reviewed their [mobile app security settings](/docs/Chapter02-01-Mobile-Security-Settings/), and walked through  [locking down mobile devices](/docs/Chapter02-03-Locking-Down-Mobile.md).

### What will participants learn?

Participants will learn why encrypting messaging is important and easy to set up. They will install Signal, learn how to set and review their privacy settings, verify safety numbers, and explore some of the application's advanced features.

### What materials will participants need?

Smartphone: iPhone or Android

### How can the trainer prepare?

Two excellent resources on how and why journalists are moving to Signal:
+ [Martin Shelton on Signal for Beginners](https://medium.com/@mshelton/signal-for-beginners-c6b44f76a1f0) 
+ [Security Tips Every Signal User Should Know (The Intercept)](https://theintercept.com/2016/07/02/security-tips-every-signal-user-should-know/).
This lesson draws from both.

Review the Verification process for [Android](https://ssd.eff.org/en/module/how-use-signal-android)  and [iOS](https://ssd.eff.org/en/module/how-use-signal-iOS).

Review the [Introduction to Digital Literacy](LINK TK) to think about how you want to explain encryption to the group.

Read [Signals, Intelligence](https://medium.com/@thegrugq/signal-intelligence-free-for-all-5993c2f72f90) for a good critique of some of the things Signal doesn't protect users against.

Additional readings that will help prepare the trainer for questions that come up: [Martin Shelton](https://medium.com/@mshelton/using-signal-without-giving-your-phone-number-3a575580f652), [Jillian York](https://motherboard.vice.com/en_us/article/9kaxge/how-to-use-signal-without-giving-out-your-phone-number-a-gendered-security-issue), and [Micah Lee](https://theintercept.com/2017/09/28/signal-tutorial-second-phone-number/) all have great walk-throughs on using Signal without giving out your phone number.

## Lesson Plan

Discussion: Why would you want to encrypt calls and text messages? What does it mean to send them in cleartext?

Remind folks that, in addition to keeping their own conversations private, by using encrypted messaging, they can normalize the use of encrypted messaging, which makes it safer for vulnerable people to use encryption without standing out.

*Note: this lesson would be much stronger with a better explanation of who does have access to cleartext SMS, and under what circumstances. We'd love it if you wanted to  [submit an issue](https://github.com/OpenNewsLabs/newsroom-security-curricula/issues) with some resources or readings that do a good job of articulating this.*

The conversation should include some review of what Signal can protect (messages traveling over the network) and what it can't protect (messages are still stored on your phone, so anyone who is able to unlock your phone has access to them.)

Real questions that users might have: who actually has access to your text messages? The answer is a bit complex. While it is relatively trivial for someone else to read messages sent in cleartext over a public wifi network, messages sent from your phone over the cell network are not as easily intercepted. However, your phone company does have access to the contents of all of your cleartext SMS messages, which means they can be subpoenaed or otherwise acquired by local police, the FBI, or the NSA. It is relatively well documented that the NSA has, historically, [swept up phone records in bulk](https://theintercept.com/2015/07/09/spying-internet-orders-magnitude-invasive-phone-metadata/). And that's just inside the US. Around the world, privacy protections can vary widely. And as long as privacy protection is legal, and not technical, individuals are vulnerable to changes in the law or to government overreach.

If you're sure you don't mind the FBI reading all of your text messages there are still good reasons to encrypt them:
+ You might change your mind. And by using Signal now, you can ensure that it is there, and working, when you decide you need it.
+ Other people need it. The more people there are who use software, the easier it is to use. That's because the simple act of using a tool like Signal effectively creates community around that tool.
+ Privacy should be normal. If democracy activists and vulnerable journalists are the only ones encrypting their text messages, their communications stand out. But if everyone encrypts the boring stuff -- the 25 message exchange about who is bringing what to a holiday meal, the back and forth about what time to meet or the dressing room photo of a questionable coat -- then we all clear the way for vulnerable users to use encryption without standing out.
+ You never know when you might find yourself working on a story where the risk of a subpoena is higher than usual. By making some small shifts now, you can ensure that the next time you find yourself thinking "I should probably not be sending this in cleartext" your next thought is "oh, right, I'm not. :)" instead of "Ack, what was that app?"

### Installing Signal

These screenshots reflect the iOS install process.

1. Start by downloading and installing Signal. Visit <https://signal.org> for quick access to the most current download links.

1. You will be prompted to confirm your device and phone number. ![Phone confirmation screen](img/ch2-4/image6.png)

1. Next, Signal/Open Whisper Systems will send you a six-digit verification code. Add it. ![Verification Code Example](img/ch2-4/image4.png) ![Submit the verification code.](img/ch2-4/image7.png)

1. Android users: Signal will offer to become your default messaging app. Say yes! You can still use Signal to send cleartext messages to contacts who don't use the app, and you won't miss messages.

1. You'll know that you've set Signal up correctly when you see the Welcome! popup. You can allow the system to access your contacts and send you notifications. *(NOTE: in the newest version of iOS, it is possible to continue without giving access to your contacts)* ![Welcome!](img/ch2-4/image5.png)![Notifications](img/ch2-4/image3.png)

### For Android:

The steps are very much the same.  Signal will offer to become your default messaging app. Say yes! You can still use Signal to send cleartext messages to contacts who don't use the app, and you won't miss messages.

If you do integrate your SMS with Signal messages, you can always long press on the send icon to send cleartext messages to other Signal users (useful when you don't have data but do need to communicate by text.)

### Additional privacy and security settings

iPhone users: click the white settings gear in the upper left corner to access privacy settings for Signal

In the Privacy tab, you can see and change:

- Numbers you've blocked
- Whether or not to show message previews when you switch apps.
- whether or not you want Signal calls to be integrated with iOS calls (shown on lock screen, show caller's name and number, show in the phone's call history)
- whether or not to relay calls through Signal's server to avoid revealing your IP address to the person on the other end (which can reveal your location).
- You can also clear all history logs in Signal (all messages, attachments, call history)

In the Notifications tab, you can select whether or not to show the sender's name and message, just the sender's name, or no name or message in your push notifications.

You can also decide **how long to keep messages** after you've read them.
- Select a name in a conversation, which will bring you to the contact information and conversation settings.
- There you can enable a setting called "Disappearing Messages," which allows messages to disappear after they have been read. You can set the timer to any length from 5 seconds to 1 week.

### Activity: 10-15 minutes

#### Verifying contacts and sending messages

- Ask participants to pair up with a neighbor and exchange phone numbers.
- They can practice finding a contact on Signal, sending a message, setting it to disappear, and verifying that it was sent securely. (On Android devices, they will see a lock icon and a pair of checkmarks. On iPhones, messages will simply display the word "sent" and "delivered")
- Each participant should practice Veryifying one another's Safety Numbers. The EFF has a nice walk-through of that process for [Android](https://ssd.eff.org/en/module/how-use-signal-android)  and [iOS](https://ssd.eff.org/en/module/how-use-signal-iOS).
- If users are not in the same space, they can check verification numbers using a separate channel, such as a phone call, iMessage, Facebook message, Twitter DMs, etc.

#### Sending documents
- When composing a message, users can click the paperclip icon to attach photos, videos, gifs, and documents to a message. Sending attachments through Signal is secure and encrypted, and does not automatically save a copy to the mobile device.

#### Creating group chats

- Pairs should pair up in groups of four to set up group chat. A mix of OSs helps here but isn't necessary.
- To create a group chat, select the Compose icon, then select the Group icon.
- Name the group chat, then add multiple contacts who are also Signal users.
- Android users will immediately see who else is in the group and what the group is named, even before you send the first message. iPhone users may not.
- You cannot delete a group once you have created it, but any member can leave the group at any point.

*Note: we'd love to know what kinds of questions come up for participants when you lead this session. Feel free to [submit an issue](https://github.com/OpenNewsLabs/newsroom-security-curricula/issues) and share your experience.*

### Wrap up

Remind participants that each conversation is only secure as the most insecure member of the conversation. Signal is a tool that has good options to protect both sides, but if a journalist is using Signal with a source who doesn't have a secure passcode or has left message previews exposed on their lock screen, the conversation may still be exposed.

Similarly, the journalist should take as many steps and precautions a possible to protect their sources by encouraging their sources to read guides on using Signal (such as this one, or the ones linked for trainers above).

## Recommended Reading

+ [How To Keep Your Chats Truly Private With Signal](https://theintercept.com/2017/05/01/cybersecurity-for-the-people-how-to-keep-your-chats-truly-private-with-signal/)
+ [Martin Shelton on Signal for Beginners](https://medium.com/@mshelton/signal-for-beginners-c6b44f76a1f0) 
+ [Security Tips Every Signal User Should Know (The Intercept)](https://theintercept.com/2016/07/02/security-tips-every-signal-user-should-know/)

### More Great Lesson Plans

+ [EFF's Security Education Companion, on How to Install Signal](https://sec.eff.org/topics/how-to-install-signal)
