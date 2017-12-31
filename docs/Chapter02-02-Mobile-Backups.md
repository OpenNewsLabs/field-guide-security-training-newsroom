# Backing up your mobile device

## Overview
Creating regular, secure backups of data on your mobile devices is important, whether you want to protect against loss, theft, or catastrophic user error (eg. accidentally wiping your device while encrypting it). This session will cover the creation of encrypted backups for iOS and Android users, and make recommendations on a backup schedule. Even if you don't get on a regular schedule, you should always backup your phone before you make any major changes to it.

Getting everyone started backing up their phones is a great way to make sure everyone leaves a workshop with something solidly accomplished.

## About This Lesson Plan

**Review date:** Dec 5, 2017  
**Lesson duration:** This should take under an hour.
**Level:** Introductory

**What materials will participants need?**

Any phones or tablets they want to back up.

**What materials will the instructor need?**


**Links in the news**

+ BuzzFeed's Nicole Nguyen has a nice [round up of backup apps](https://www.buzzfeed.com/nicolenguyen/what-to-do-if-your-phones-storage-is-full)

+ Hackers Stole My Life by [Mat Honan on Wired](https://www.wired.com/2012/08/apple-amazon-mat-honan-hacking/) is a great lesson in the perils of cloud backups.

## Lesson Plan

Read [EFF on Harm Reduction](https://sec.eff.org/articles/harm-reduction) -- it's an important perspective to keep in mind here. And remember that it is better to acknowledge it when you're [out of scope](https://sec.eff.org/articles/out-of-scope), than to bluff or share bad information.

Everyone should take stock of what is actually on their phone that isn't already backed up. Most folks are syncing calendars and contacts with [Nextcloud](https://nextcloud.com/) or Google or iCloud or iTunes already, but if anyone isn't, start there.

Have everyone go through the apps installed on their phones (this is also a fine time to think about deleting apps you don't use). Some things, like email, are easily restored from settings, but if you know you're going to do a hard reset on your phone, take a moment to make sure you have a record of those settings.
+ Social Media (eg. Tumblr, Twitter, What's App) is easy to restore if you know your login information.
+ Email often requires you to know a few settings.
+ Two Factor Authentication can really throw you -- if you're using 2FA open your authenticator app and make sure that you have backup codes for every service listed. If you aren't, make that sure that's one of your next sessions. :)
+ Photos might be backed up automatically but if you'll be devastated to lose them, consider copying them to a hard drive somewhere.
+ Podcast subscriptions probably aren't dire, but you can usually export an OPML that will make it easy to restore your subscriptions after a reset.

As other things come up, add to this list. Does the app contain data or settings that need backing up? What's a good strategy for making that backup happen?

Note: we'd love your help expanding this lesson. Consider filing an [issue](https://github.com/OpenNewsLabs/newsroom-security-curricula/issues) or pull request if there are valuable backup points that you think belong here.

### Automated Backups
By default, Android phones back up quite a bit of data to Google, iOS phones to iCloud. These baked in cloud backup services are far and away the easiest way to make sure that your contacts, photos and calendar are backed up someplace off of your phone. However, commercial cloud backup services are not a good fit for everyone. Commercial cloud providers may not be willing or able to fight a subpoena for contacts you've backed up to their server.

Where you back your work up depends a lot on your values and threat model. For some folks, the risk of losing all their data outweighs their discomfort with or handing over evermore personal data to Google or Apple.

Setting up and hosting your own service ([Nextcloud](https://nextcloud.com/) or [ownCloud](https://owncloud.com/) are good options if you want to go that route) is not a trivial undertaking. Keeping up with updates and ensuring that your server is configured securely are all you as the host. You can also [pay someone to maintain Nextcloud for you](https://nextcloud.com/providers/).

Users should make a conscious decision about their own needs and values: if you're fine backing up to Google or iCloud, then go for it. If you'd rather backup to them than lose all your data, then go ahead and make sure things are getting backed up while you work on setting up a more perfect solution. And if you'd rather risk losing your contacts than backing up to a Google or iCloud, at least take a moment to export your data and back it up manually from time to time.

Some folks like to start over with a clean slate from time to time -- they're fine not backing up at all.

Everyone's backup strategy is going to be different. Your goal is to find a strategy that you'll actually stick with, and that suits your values.

### Android Users
In addition to backing up to a cloud or web-based service, Android users can back up directly to a laptop or desktop via USB.  Just watch out for power-only USB cables that don't support data transfer. You should see a prompt inviting you to allow file transfer when you connect your phone to your laptop via USB -- it might be labeled "MTP" or "FTP". Once you accept that, your phone should mount as a drive on your laptop. If you're going to make a one-off backup like this, especially if you're going to be resetting your phone consider also ...
+ Export your contacts to a `.vcf` file (`Import/Export` is one of just four menu options) and back that up.
+ Most podcast apps will let you export an OPML file so you can restore your subscriptions.

### iOS Users

*You can help us make this lesson stronger by [contributing](contributing.md) insights on backup strategies for iOS users.*
