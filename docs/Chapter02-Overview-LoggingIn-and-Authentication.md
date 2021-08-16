# Security in the Newsroom: Who are you?

This lesson plan, which covers Passwords and Two Factor Authentication is a great hour long brown-bag session that was shared with us by Alan Palazzolo at the Minneapolis Star Tribune. For other great overview lesson plans, take a look at:

Or, there are more great resources in [the resource roundup](https://securitytraining.opennews.org/en/latest/Chapter03-01-Resources.html).

## Logging in and authentication

There’s a login for everything these days. The default way to prove to computers that you are you is with a username and password. We all have hundreds of different websites, computers, and other digital things that require passwords. That’s a lot of opportunity for attackers to try to steal your identity or your personal information. So, how can we make sure we are being safe when we log into things? Let’s talk about strong passwords, password managers, two-factor authentication, digital keys, HTTPS and more.


## Security

A quick step back. Security comes in many forms, not just digital. There are lots of aspects to consider when it comes to your personal security, and many things to focus in on when talking about security in the newsroom. A few things to keep in mind about security in general:

-   Good security takes a little bit of effort. There is sometimes a trade-off of what is easy and what is most secure.
-   Though there are good general security practices, thinking about your security in terms of threat modeling (who will reasonably attack me, and what specifically do you need to defend against) will help focus your efforts.
-   Attacks are always changing, it’s good to stay up to date, even if just on a high level.
-   Talk to experts. Unless you are totally confident of what you are doing, take a moment to double check with someone how to practice good security.
-   Nothing can be 100% secure, but we can be significantly more secure with minimal cost.
-   Even if you don’t think you are at risk, we are all avenues to other people who may be targets. [*You are worthy of a data breach*](https://medium.com/@mshelton/journalists-you-are-worthy-of-a-data-breach-55f8e53fd3fe).

## Some terminology

Just to make sure we are all on the same page, here are some top-level words and concepts:

-   **Authentication**: A mechanism used to identify someone. The most common mechanism is a username and password, but there are others, such as PIN codes, fingerprints, and more.
-   **Password**: Usually a single word or short random set of characters used for authentication.
-   **Passphrase**: A phrase used for authentication, usually at least a few words or a whole sentence. Note, that when we refer to good, secure “passwords”, we usually mean a passphrase.

![customize](img/ch2_o01_02.png) -- this icon indicates that you should customize the section to your newsroom.


![important](img/ch2_o01_01.png) -- If you see this icon, this is important.

## What’s at stake?

Though fairly simple, authentication, i.e. logging in, is a huge, far-reaching topic. Almost anything important these days has some sort of authentication. Your email, you bank account, your bills, your medical history, and so much more all are just a username and password away from being accessed.

**One compromise can lead to many**. Huge companies such as Target, Equifax, Yahoo, and [*many others*](https://haveibeenpwned.com/PwnedWebsites) have had huge amounts of their user’s data compromised. If you have use the same password or a pattern of passwords, once one site if compromised, your other accounts are much more likely to get compromised.

It is very possible that you have had an account compromised. The site “[*Have I Been Pwned*](https://haveibeenpwned.com/)” will give you some insight into that possibility. Note that “pwned” is a term used to describe getting “owned” by someone.

[*Mat Honan had his digital life erased*](https://www.wired.com/2012/08/apple-amazon-mat-honan-hacking/) and hijacked because of a series breaches chained together.

**Your identity**. If someone has access to your account, they can do things as you, such as post things to Twitter, reset accounts, or access sensitive information.

In 2017, the Twitter account of CNN’s host, Anderson Cooper claimed his account was was [*compromised*](http://thehill.com/homenews/media/364646-anderson-cooper-says-twitter-account-hacked-after-tweet-calling-trump-a). And even with two-factor authentication enabled, Deray McKesson ([*@deray*](https://www.wired.com/2016/06/deray-twitter-hack-2-factor-isnt-enough/)), a prominent figure in the Black Lives Matter movement, had his account breached. The lesson: High-profile individuals are disproportionately targeted, and must take extra steps to lock down their account tightly.

**Specifically your email**. Your email is very strongly tied to your identity. In fact, most online accounts allow you to reset authentication with email, so, if your email gets compromised, many other accounts can be compromised. Your email is also often a trusted contact for the inbox of the people you know, so an attacker can more easily become a trusted contact if your email is compromised. Generally, when it comes to securing your online accounts, securing your primary email should be your first priority.

### Passwords

Passwords (and usernames) are probably the most common way to authenticate someone to access a service and one of the most important security concerns.

### Password managers

Most of us have hundreds of services that require a username and password. Most of us can’t remember hundreds of passwords. This is where a password manager comes in; they create a secure way to store all the username and passwords you need. And most have the ability to integrate with your web browser so it makes it easy to login to a service.


![important](img/ch2_o01_01.png) **Installing and using a password manager is possibly the biggest step you can take in making your life more secure, and it’s one of the easiest.**

There are two popular password manager products that you should consider using: LastPass and 1Password. Both have similar features, but **LastPass** has a free tier with all the main features, and it can be used/installed without installing an application on your computer, so it is suggested for most users.

To see other options and features, see this [*Wirecutter review*](https://thewirecutter.com/reviews/best-password-managers/) or [suggestions from Freedom of the Press Foundation](https://freedom.press/training/blog/choosing-password-manager/).

It’s important to note that you are putting a lot of trust into your password manager and the company that makes it and stores your data. Though it is not in their interest to compromise anyone’s security, you cannot be 100% sure that it won’t happen, and access to all your passwords is a lot of important information. But, it is still better than most alternatives.

### Example: 1Password

There are many types of password managers, but one of the best and easiest to use is 1Password. There are many ways to use 1Passwords.

One of the main ways is to use their [*browser extensions*](https://support.1password.com/getting-started-browser/). These are particularly great because they make it very easy to log into websites.

![1Password in the browser](https://user-images.githubusercontent.com/4054013/129640160-480ba891-6ff2-47f5-a27e-c88c7fb68e61.gif)

Another useful way to get access to your 1Password account is with their mobile applications, both for [*Android*](https://1password.com/downloads/android/) and [*iOS*](https://1password.com/downloads/ios/).

![1Password mobile](https://user-images.githubusercontent.com/4054013/129640681-508c5634-3791-4e3d-8433-ff3d24f27a0f.png)

You can also install [*stand-alone desktop applications*](https://1password.com/downloads) for 1Password.

Note that normally many password managers are paid services, but [journalists may request a free 1Password account](https://1password.com/for-journalism/)! 

![important](img/ch2_o01_02.png)
**Does your newsroom have a policy that prevents users from installing software or plugins? How should users in your newsroom install?**


### Unique passwords

So, now that you have a password manager, you can practice some other good security more easily.


![important](img/ch2_o01_01.png) **Use unique passwords for everything.**

Unique passwords are important because you never know what site or service may be compromised. If you share passwords among services, the password is only as strong as the weakest security of all the services.

Unique passwords are hard to do without a password manager. Some people use a specific pattern that makes a unique password for each service, but more than likely, this pattern is easily discerned by an attacker.

Since Strib account passwords must be changed regularly, it’s tempting to have your password include a number that you just increment at each change, e.g. “fiddler111” followed by “fiddler112”. This is easy to remember but leaves a trail of breadcrumbs for any adversary who discovers an old password.

With a password manager, it is trivial to use a unique, unrelated password for every service.

### Strong passwords

The strength of a password refers to the ability for it to be determined or guessed by trying many combinations of words, letters, numbers, and symbols. The password “password” is both very short and extremely common and might be the first attempt someone uses when guessing your password; therefore it is very weak.


![important](img/ch2_o01_01.png) **Use strong passwords.**

In fact, just use long, random passwords. Most password managers will provide a way to generate passwords.

In some cases, you have accounts that you log into often where you need a password that you can remember. Overall, length is more secure than the variation (i.e. using symbols or uppercase letters). So, create a phrase that is memorable, but not easily guessable, and maybe add some easily rememberable variation. Some examples:

    security-sure-is-gr8-for-us-all!

    is it snowing outside today in minneSNOWta?

Note, that once you start using really long passwords, you may notice that some services limit the length of your password. This is bad security on their part but not something that you will be able to change. This can be particularly annoying if you paste in passwords where the input has a maximum length.

### While we’re at it...

Use unique, random usernames too. Many times your username is an email, but when its not, why not use a unique username. This adds more security as it is less guessable, and if compromised less likely to be associated with another account.

###  Shared passwords

It’s a sad fact, but we often use shared passwords in the office; sometimes this is out of necessity and sometimes it’s just a lack of effort.

Until our organization has a common, shared password solution that makes shared passwords easy and secure, here are a few tips for handling shared passwords. Basically, follow the same advice for non-shared passwords.

-   Don’t use easily guessable passwords like `startribune`. Use strong passwords.
-   Don’t use the same password over and over again. Use unique passwords.
-   Don’t write them down, or if you must, dispose of them in a shredder or other secure way.
-   Put your shared passwords in your password manager.

*To explore*: It has been suggested that some services will allow multiple authenticator applications to be tied to one account, thus allowing 2FA for a shared account.

###  More about passwords

There is plenty written about passwords; here are some good resources if you want to dive deeper.

-   [*Wirecutter’s review of password managers*](https://thewirecutter.com/reviews/best-password-managers/)
-   [*OpenNews security training on passwords*](https://securitytraining.opennews.org/en/latest/Chapter02-06-Passwords.html) 
-   [*Freedom of the Press Foundation's work on choosing a password manager*](https://freedom.press/training/blog/choosing-password-manager/)

## Two-factor authentication

A password is often referred to as a knowledge factor when authenticating. To make accounts more secure, more factors can be introduced if the service allows it. Common examples are possession factors (keys, phones, etc) and inherence factors (fingerprints, iris, etc).

Many services these days offer 2FA (two-factor authentication), allowing you to add a factor on top of the main mechanism which is most often a username and password. Some of the common ones are:

-   A text or call sent to your phone with a specific code.
-   A custom or 3rd-party application that provides a code (usually installed on your phone).
-   A USB key.
-   A physical device that generates a code.
-   Fingerprint.

Note that two-factor authentication may be referred to in other ways such as “two step verification” or “multi-factor authentication”.

![important](img/ch2_o01_01.png) **Enable two-factor authentication wherever you can.**

2FA makes your accounts much more secure (note nothing is 100% secure). If for some reason an attacker gets your password, or finds some way to reset your account, they still need some access to your second factor which makes it much harder to compromise your account.

Common services that have the ability to turn on 2FA:

-   Google (GMail)
-   Dropbox
-   Twitter
-   Facebook
-   and [*more*](https://2fa.directory/)

![Customize This](img/ch2_o01_02.png) **If your newsroom has a two factor policy, include it here.**

###  Choosing your second factor

Some services allow you to choose different methods for your second factor. We’ll go over a couple different ones. Though some are better than others, they are all better than nothing. If a choice is available, the preferred factor for most people is the **authenticator application**.

####  Texting (SMS) or phone call

This is where the service will send you a code via SMS and then you enter that code into the service.

![2FA via SMS](https://user-images.githubusercontent.com/4054013/129642015-8018b913-2dd4-4ef1-821a-1d1f58a4c508.png)

The main downsides of this is that you need to have phone reception, and your text and phone access is actually tied to your SIM card and not the actual phone; and there has been cases where a SIM has been transferred and an [*account compromised*](https://www.wired.com/2016/06/deray-twitter-hack-2-factor-isnt-enough/).

####  Authenticator application

Another popular option is to use an authenticator application, often on your phone. This works similarly to SMS by generating a code that is tied to your account.

![2FA via Authenticator app](https://user-images.githubusercontent.com/4054013/129642416-e53ad050-f38a-4726-8acc-8e04b6752eed.png)

This is beneficial over the SMS approach, since it does not require network access, and does not lend itself to the SIM attacks described above.

There are a number of authenticator applications. Most services will let you use the one you want, but some are more forceful in their requirements. Some popular authenticator applications are [*Google’s Authenticator for Android*](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2&hl=en) and [*iOS*](https://itunes.apple.com/us/app/google-authenticator/id388497605?mt=8) and [*Authy*](https://authy.com/).


####  Security keys

While not offered on all services, many major services support the use of physical security keys — usually small USB devices that help you authenticate into a website. These are much harder to compromise, but they are not free. A very popular option is [*YubiKey*](https://www.yubico.com/), and they offer a basic key for as little as [*\$25*](https://www.yubico.com/store/).

![2FA via security key](https://user-images.githubusercontent.com/4054013/129642480-245780eb-5793-48ba-b1ee-3d9c05e581bb.gif)


###  You have a password manager now...

When setting up a 2FA, you will usually get some set of recovery codes that can be used if you lose your phone or authentication method. Put these in your password manager.

###  More about 2FA

Enabling two-factor authentication is one of the best security practices that you can do and there’s lots more to read up about it if you want.

-   [*Freedom of the Press Foundation: "Two-factor authentication for beginners*](https://freedom.press/training/2fa-beginners/)
-   [*2fa.directory*](https://2fa.directory/), a place to see what services offer two-factor authentication, and what kind they offer
-   [*OpenNews security training chapter on 2FA*](https://securitytraining.opennews.org/en/latest/Chapter02-07-Two-Factor-Authentication.html)

##  Biometric authentication

Often used in place of a password, biometric authentication is using something that is unique to your physical body to prove that you are you. The most common is fingerprint scanning on our phones, as well as the face recognition that Apple has recently introduced.

Biometric authentication has its pros and cons (need reference). If you want to use biometric authentication, it is suggested to enhance it with a password or PIN; for instance, on Android, you can require the password every few days. If you are at a higher risk than most, such as working on very sensitive materials, use both a password and biometrics every time.

The use of biometric authentication is not new, but its consumer use is relatively new, we are still learning about the [*practical*](https://techcrunch.com/2021/07/26/court-orders-us-capitol-rioter-to-unlock-his-laptop-with-his-face/) and [*legal*](http://www.pennstatelawreview.org/print-issues/face-it-the-convenience-of-a-biometric-password-may-mean-forfeiting-your-fifth-amendment-rights/) implications of biometric device unlock software. In general, in risky situations where there is a reasonable chance your device might be seized (e.g., when visiting a border or protest) it may be best to disable biometrics.

##  Enhancements when authenticating

Some services will use different techniques or data points to “enhance” the authentication process. It can be argued whether these actually produce better security, but either way, these things should not be taken lightly, as they could be ways for attackers to access your account.

###  Security questions

“Security questions” are often used to enhance authentication. The idea is that by using some simple, easy-to-remember questions and answers, the service can be more certain you are who you are.

In practice, these should just be viewed as another password. So, treat it like one. Use unique answers, and write them down in your password manager. You should use human-readable answers for these, as they may be used to confirm your account verbally over the phone with customer service representatives (though hopefully not).

###  PIN

A PIN (personal identification number) is sometimes used to enhance a username and login, and sometimes it is the main method of authentication.

Again, these should be considered the same as passwords. Make them as long as possible, don’t use the same one twice, and store them in your password manager.

For things like a debit card, you’re authenticating with the card itself and the PIN. In practice, you will probably want to use a number that you can remember. Make sure not to use a number that is easily associated with you, such as your house number.

###  Login images

These are not technically about authenticating who you are, but in actuality an anti-phishing technique; it is a mechanism for you to be (more) sure that the service is the correct service and not an attacker faking the service. It is suggested to make note of the image you set when creating an account in your password manager.

Note that we will talk about phishing in another session.

## Email address

Your email address is very often your username for a service. Often, a service will have you “verify” your email address by sending you an email with some sort of verification link or something similar.

This is a sort of second form of authentication, as your email is assumed to be associated with you personally.

Your email becomes a gateway to many other accounts, as it is the username, and it is the main mechanism for services to reset your account. Make sure you use a very strong, unique password for you email and turn on two-factor authentication.

**At the very least, make sure you use strong passwords and 2FA for your email addresses.**

###  Temporary emails

For serious, though a bit risky, security, you can use temporary or throw-away email services to verify accounts. While researching online, and obviously depending on the nature of the research, it may be beneficial to use a temporary email to sign up for websites so that your real email is not tied to any work you may be doing. Note that these email providers may decrypt your emails, so any email you receive through these services should not be considered private. This is a good idea to ensure that your own email is not compromised, but it means that you won’t be able to recover access if needed. 

This list has not been reviewed, but here is a list of [*disposable email services*](https://www.digitaltrends.com/computing/best-sites-for-creating-a-disposable-email-address/).

## Make sure the site is secure

When actually logging into a site, you should consider a couple things. First, particularly if someone has sent you the link, you should make sure it’s the correct site and you are not being phished. This is covered in-depth [in the phishing section](https://securitytraining.opennews.org/en/latest/Chapter02-08-Phishing.html).

###  HTTPS

You should make sure the browser is communicating securely with the server via HTTPS. When you connect to a website, some may use unsecured HTTP connections. You can see this by looking at corner of your browser's address bar for "http://" (as in (http://example.com) or in many browsers, an unlocked padlock icon. On an HTTP website, intermediaries (e.g., your Internet Service Provider; other people on an unsecured Wi-Fi connection) can see that password. That’s where HTTPS comes in (the “s” in HTTPS is for secure)! HTTPS creates an encrypted channel between your computer and the website. Fortunately, most common websites now use HTTPS. Your browser should make it fairly easy to know if the site is secure.

On most browsers HTTPS websites have a padlock in the address bar, similar to the following:

![Lock icon](https://user-images.githubusercontent.com/4054013/129637935-e06f875d-8545-4282-8304-fa437ef6ee3e.png)

Note that in recent years, even phishing websites may use HTTPS. When you receive an email or communication over email or anywhere else, the safest thing to do is navigate directly to the website you want to visit by searching for it or entering its URL yourself, if you know the URL.

## In the newsroom

What are specific considerations in the newsroom. Indirectly, any information or communications that can be accessed by a login is at stake; this may include a source’s identity, communication to colleagues, sensitive documents, etc.
