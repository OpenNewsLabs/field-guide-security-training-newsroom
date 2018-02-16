# Best Practices for a Tips Page

This document was adapted from Martin Shelton's [Opening Secure Channels for Confidential Tips (Source, Feb 2017)](https://source.opennews.org/articles/opening-secure-channels-confidential-tips/). You should read that for a thorough review of best practices.

You should also read Ted Han and Quinn Norton on [Protecting Your Sources When Releasing Sensitive Documents (Source, June 2017)](https://source.opennews.org/articles/how-protect-your-sources-when-releasing-sensitive-/)



This short guide describes some basics around how to think about security on behalf of your sources before thinking about tools and practices. We’ll also describe common communication channels for accepting sensitive tips and tradeoffs when using each channel. When thinking about tradeoffs, consider which channels are right for you.


## Before We Talk About Tools

Before we even talk about tools for taking confidential tips securely, there are some more basic issues to address.

1. Who is going to maintain the page? If you’re reading this, the person maintaining the secure tip page for your newsroom might be you. Make sure you know what that entails, and that there's a plan in place for handing off ownership if you leave the newsroom.

2.  The page should easily accessible, and under the newsroom's control. Don't

3.  Host secure tip pages with HTTPS, not over an unsecured HTTP connection. This prevents unwanted third parties from snooping on would-be sources’ connections to your tip page. If your site doesn't already default to HTTPS, address that first. Two excellent resources to help make the case: [The US CIO's excellent and thorough explanation](https://https.cio.gov/everything/), and [Chrome's Developer Blog](https://developers.google.com/web/fundamentals/security/encrypt-in-transit/why-https).

4. HTTPS prevents an eavesdropper from sniffing out anything beyond the domain name, so your tips page should not be served from a dedicated subdomain (eg. https://tips.example.com), but on a subdirectory of your primary website (eg. https://www.example.com/tips).

5. The newsroom should be prepared to advertise the tips page widely. A good tips page only works if people read it *before* reaching out.

**So what goes on the page?**

* Give sources as many ways to reach out as you have, and be clear about the advantages and drawbacks of each channel.

**Don't stop with a tips page.**

Whether or not a source uses your confidential tips infrastructure to reach you, you have a responsibility to consider their safety before you continue to communicate with a source.

Think about who would care about this information being made public (eg., their employer). What capabilities do they have to investigate the source of the tip? What are the potential consequences for your source if they are discovered? And then guide your source to the communications channels that will best protect them from surveillance.

And when you're ready to publish, make sure you're not inadvertently revealing your source.

[Protecting Your Sources When Releasing Sensitive Documents (Source, June 2017)](https://source.opennews.org/articles/how-protect-your-sources-when-releasing-sensitive-/) is an excellent review.

**Content versus metadata**

Many of the tools we recommend can protect the contents of your communications, but not the fact that you communicated at all. Even if your phone company isn't surveillance the contents of a phone call, their records will show all the numbers you called, whether the other party answered, and how long you stayed on the line. If you make calls over a service like WhatsApp, your phone history will still show that the call was made.

Most secure communications channels do not protect against metadata surveillance, so make note of these constraints in your documentation.

Similarly, any file on your computer has a bunch of metadata attached to it: the date and time it was created, the time it was last modified, size, and filename. And depending on the software that created a the metadata might include the name of the person who created it, or the company the software was licensed to. EXIF data attached to digital images often includes the type of camera the image was captured with.

**First Contact**

If a source reached out over a work phone or email, they have already given their employer a metadata trail. This is sometimes called the "first contact problem," and there is no quick fix. This is why newsrooms have a responsibility to educate sources (and potential sources) before they reach out.

Your tips page is a good place to offer that education.

The best we can do is support the appropriate communication channels, and advertise that we’re available to check out tips. Have a page where these channels are clearly organized, and share it with information about the tradeoffs.

It’s also important to be be clear that if they have reached out over a less-than-ideal channel, such as calling from their work phone or using their work computer, sources may have burned themselves already.

The Intercept has [an excellent guide](https://theintercept.com/leak/) to reaching out anonymously. They are very clear both about how to reach out, and *what not to do*.

![](img/ch3-03.png)  ASK: NEED IMAGE FROM GDRIVEs

**Be clear about risk**

Many existing resources fail to give would-be sources enough information about the risks associated with reaching out with sensitive information. News organizations can, and must, do better.

If someone’s at risk of going to losing their job, going to jail (or worse) for reaching out to you, you owe them a sober explanation. Only promise the protection you know you can actually provide. Don't scare people unnecessarily, but do make sure they understand what they’re getting into.


## Onto The Tools

Many of us already have a professional email address, desk phone, cell phone, or social media accounts (eg. Twitter, Facebook) to gather information for stories. These are all great channels for less sensitive tips, but what do you do if you need to secure your communications?

**Common secure channels**

Some common secure communication channels include [Signal](https://signal.org/), [WhatsApp](https://whatsapp.com/), [Off-the-record messaging](https://wikipedia.org/wiki/Off-the-Record_Messaging), and PGP for email encryption. Each has advantages and tradeoffs:

+ [Signal](https://signal.org/) is a free and open source secure messaging app for [iPhone](https://itunes.apple.com/us/app/signal-private-messenger/id874139669) and [Android](https://play.google.com/store/apps/details?id=org.thoughtcrime.securesms&hl=en), developed by [Open Whisper Systems](https://whispersystems.org/). There is also a [desktop](https://signal.org/download/) application. Signal supports encrypted text messaging and phone calls. Signal’s developers designed the service to retain as little metadata as possible: all they store is a user’s phone number, sign-up time, and the time when the user was last active. Signal also allows messages to "self-destruct" automatically after a preset amount of time, leaving behind as little information as possible. For help getting started, read [Signal for Beginners](https://medium.com/@mshelton/signal-for-beginners-c6b44f76a1f0).

    + Tradeoffs: While Signal’s servers retain [very little metadata](https://whispersystems.org/bigbrother/eastern-virginia-grand-jury/), the app is  not designed to prevent live metadata surveillance. The users in conversation should not be considered anonymous.

+ [WhatsApp](https://whatsapp.com/) has over a billion users on [iPhone](https://itunes.apple.com/us/app/whatsapp-messenger/id310633997) and [Android](https://play.google.com/store/apps/details?id=com.whatsapp) and uses similar encryption to Signal. It’s easy to use, and with the right settings, can be a decent option for routine communications. WhatsApp users can share more types of files than Signal, and it can be
a great way to send documents.

    + Tradeoffs: Importantly, some settings must be tweaked to maximize the security  of the app, and to make it safer for routine use. Under some circumstances, WhatsApp backs up unencrypted messages to iCloud or Google Drive by default: users may need to confirm that backups are be disabled. [Upgrading WhatsApp Security](https://medium.com/@mshelton/upgrading-whatsapp-security-386c8ce496d3) is an excellent guide to ... upgrading WhatsApp securit.

    + Like Signal, WhatsApp stores user phone numbers. They also [store substantially more data](https://www.whatsapp.com/legal/#privacy-policy) -- your address book, who you contact most often, and other information about how you use the service. WhatsApp [shares that data with their parent company, Facebook](https://www.eff.org/deeplinks/2016/08/what-facebook-and-whatsapps-data-sharing-plans-really-mean-user-privacy-0). Facebook,and WhatsApp can be forced to share their user data in response to a court order or subpoena.

+ [Off-the-record](https://en.wikipedia.org/wiki/Off-the-Record_Messaging), or OTR is a messaging encryption standard. OTR can be installed as a plug-in for messaging clients, such as [Pidgin](https://pidgin.im/) or [Adium](https://adium.im/), typically using an open messaging standard called [XMPP](https://en.wikipedia.org/wiki/XMPP). OTR can encrypt communications on a variety of inter-operable messaging clients. The Electronic Frontier Foundation provides a primer on getting started with OTR for [Windows](https://ssd.eff.org/en/module/how-use-otr-windows), [Mac](https://ssd.eff.org/en/module/how-use-otr-mac), and [Linux](https://ssd.eff.org/en/module/how-use-otr-linux). OTR allows users to accept messages from anyone using an OTR client, including some anonymity-protecting clients such as [Tor Messenger](https://blog.torproject.org/blog/tor-messenger-beta-chat-over-tor-easily). If your contacts have the know-how, this can be an asset for protecting their anonymity.

    + Tradeoffs: Not everyone is familiar with OTR -- you’re much more likely to receive an OTR message from a savvy user than anyone else. OTR should not be confused with the "off the record" setting in Google Hangouts.

+ [OpenPGP](https://en.wikipedia.org/wiki/Pretty_Good_Privacy) is an email encryption standard, most commonly used to secure email correspondence. Note that PGP (Pretty Good Privacy) and GPG (GNU Privacy Guard) are two implementations of the same standard, so you may see GPG and PGP used interchangeably. PGP uses public key cryptography: messages scrambled with a "public" key can only be unscrambled by the corresponding "private" key. The public key can be shared widely, so anyone can create a scrambled message that can only be read by the user who holds the corresponding private key. Users typically post their public key in an accessible place, such as a personal website, byline, or a [public keyserver](https://pgp.mit.edu/pks/lookup?search=nytimes&op=index). The Electronic Frontier Foundation has resources for setting up PGP on [Windows](https://ssd.eff.org/en/module/how-use-pgp-windows), [Mac](https://ssd.eff.org/en/module/how-use-pgp-mac-os-x), and [Linux](https://ssd.eff.org/en/module/how-use-pgp-linux).

    + Tradeoffs: PGP is famously tricky to use, even for security geeks. It’s easy to make a mistake that will compromise sensitive communications. And PGP only secures the body of an email: email addresses, timestamps and subject lines are all still sent in plaintext, exposed to eavesdroppers. You are likely to get more "return on investment" with simpler channels, such as Signal.

**Secure Organizational Channels**

When done properly, physical mail and [SecureDrop](https://securedrop.org/) can both be good ways for sources to avoid giving personally identifiable information. The catch is, your sources have to know what to do.

+ Postal mail. Regular old-fashioned postal service physical mail is a solid way to receive sensitive tips because sources don’t need to provide a return address. The U.S. postal service does [collect images of the exterior of paper mail](http://www.nytimes.com/2013/07/04/us/monitoring-of-snail-mail.html), so encourage sources to leave off the return address (or put it inside of the envelope). Physical mail can be a great way to send paper documents as well as electronic media, such as SD cards or small USB devices.

    + Tradeoffs: The main drawback is that mail is one-time communication. If you advertise your office address for accepting tips, encourage sources to give you a way to reach them if you have questions. Also, many workplaces are able to see who accessed a particular document, as well as review individual printer usage: a tipster who prints out a sensitive document at work may be caught by their own infrastructure before the document even reaches a newsroom.

+ [SecureDrop](https://docs.securedrop.org/en/stable/index.html) is an encrypted submission system that can help news organizations receive documents and exchange messages with sources. SecureDrop uses the Tor anonymity network, which encrypts and bounces web traffic around the globe, making it much more difficult for eavesdroppers to determine the original source of a tip. This is one of the best options available for protecting confidentiality.

  + Tradeoffs: Sources using SecureDrop don’t have to provide identifying information unless they choose to do so. This added protection for sources can sometimes present challenges for newsrooms that need to verify the legitimacy of an anonymous leak.

  + SecureDrop requires dedicated equipment and an administrator familiar with the basics of Linux and Bash shell. The SecureDrop docs provide a good overview of the process of [setting up SecureDrop](https://docs.securedrop.org/en/stable/index.html). ASK: LINK TO OUR LESSON. It isn't a trivial undertaking. And while some individual reporters have their own SecureDrop instances -- [Bart Gellman](https://tcfmailvault.info/) and Wired’s [Kevin Poulsen](https://freedom.press/people/kevin-poulsen/) both do, in general SecureDrop should be an institutional tool.



**Pay Attention to File Metadata**

If you’re going to publish files from a source, look out for file metadata. Metadata is information about a file, such as its creator or associated GPS coordinates. You can accidentally burn sources by publishing metadata alone.

This isn’t new. Back in 2012, [Two Vice journalists accidentally outed the location of then-billionaire-in-hiding, John McAfee](https://www.wired.com/2012/12/oops-did-vice-just-give-away-john-mcafees-location-with-this-photo/). How? They shared a picture on their website. It turns out the image was taken an iPhone 4S, and appended GPS metadata. It’s pretty easy to analyze images for appended metadata, and a growing number of web-based tools make this process painless (eg., <http://exifdata.com/>.

Consider whether it’s appropriate to publish original documents with their file metadata intact. You can often remove metadata by converting the file into a new format (eg., by taking a screenshot of a document).

+ It’s fairly easy to scrub unwanted metadata on [Windows](http://www.digitalcitizen.life/what-file-s-metadata-and-how-edit-it).

+ For those who feel comfortable with Bash, consider using the [Metadata Anonymisation Toolkit](https://mat.boum.org/).

To learn more, [please read our section for lessons on scrubbing metadata](https://docs.google.com/document/d/1MS9MoeXmXw_TYOmjXto9mvg-EROL5vds2sl5zytQTZk/edit#).

**Unsafe devices lead to unsafe sources**

Your conversations are only as secure as your devices. Be aware of a few different ways your communications can be compromised.

Perhaps it goes without saying, but encryption doesn’t protect you if someone takes control of your unlocked physical devices. If the device you use to decrypt your messages gets infected with malware, your decrypted files are readily available to the remote attacker. And of course, without strong authentication, there’s not much standing between a hacker and your sensitive communications over your email, Twitter, Facebook, or any online account where you chat with sources.

Defend against common attacks to protect your accounts and conversations with sources. One common way that newsroom accounts and devices are hijacked is through "phishing" emails—emails that link to a fake login page, where you’re encouraged to enter your very real login information.

[Learn more about phishing here](https://freedom.press/training/email-security-tips/).

Another common tactic is to encourage reporters to download and launch malicious file attachments that can give a remote attacker access to your device. Though you will inevitably open email links from strangers (it’s part of the job, after all), use caution and learn to identify suspicious-looking emails. If you’re feeling unsure of a file attachment in an email, consider whether to open PDFs and Microsoft Office documents, which are especially popular for distributing malware. If you’re okay with sharing a document with Google, consider opening it in Google Docs instead of opening it directly on your computer.

To make it harder for remote attackers to log in and see any communications with sources, use hard-to-guess passwords (ideally generated and stored with a [password manager](https://medium.com/@mshelton/password-managers-for-beginners-d1f49866f80f)) and use [two-factor authentication](https://twofactorauth.org/).

Learn more about [how to keep newsroom accounts safe from hijacking](https://source.opennews.org/guides/defending-accounts/).

**Consider What’s Right for Your Sources**

Most newsrooms are overworked, and it’s challenging to find the time to get started with these tools and practices. However, secure tip channels allow sources to come forward with compelling information, especially when they are putting their safety or livelihood at risk for sharing what they know. Secure tip channels also signal to sources that you take their confidentiality seriously. Consider which options are appropriate for your organization and your sources.

Here are some additional examples you can look to for inspiration on your secure tip page:

+ ProPublica: <https://securedrop.propublica.org/> and "[How to Leak to ProPublica](https://www.propublica.org/article/how-to-leak-to-propublica)"

+ The New York Times: <https://www.nytimes.com/tips>

+ The Washington Post: <(https://www.washingtonpost.com/anonymous-news-tips/>

    + See also <https://www.washingtonpost.com/securedrop/> and "[Here’s how to leak government documents to The Post](https://www.washingtonpost.com/news/politics/wp/2017/01/25/heres-how-to-leak-government-documents-to-the-post/)"

+ BuzzFeed: <https://contact.buzzfeed.com/>

+ The Associated Press: <https://www.ap.org/tips/>

+ The Guardian: <https://securedrop.theguardian.com/>

+ The New Yorker: <https://projects.newyorker.com/strongbox/>

+ The Intercept: <https://theintercept.com/leak/>

    + See also <https://theintercept.com/2015/01/28/how-to-leak-to-the-intercept/>  

+ Vice: <https://news.vice.com/securedrop/>

### Recommended Reading

<https://source.opennews.org/articles/how-protect-your-sources-when-releasing-sensitive-/>
