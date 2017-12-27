**Best Practices for a Tips Page**
----------------------------------

(Loosely adapted from [*Opening Secure Channels for Confidential
Tips*](https://source.opennews.org/articles/opening-secure-channels-confidential-tips/))

To make it easier for tipsters to share sensitive information, news
organizations are launching resources for confidential tips. The [*New
York Times*](https://nytimes.com/tips), the [*Washington
Post*](https://www.washingtonpost.com/anonymous-news-tips/), the
[*Intercept*](https://theintercept.com/2015/01/28/how-to-leak-to-the-intercept/),
[*Propublica*](https://www.propublica.org/article/how-to-leak-to-propublica),
and [*Buzzfeed*](https://contact.buzzfeed.com/) all have one. Maybe you
want to set one up?

This short guide will describe some basics around how to think about
security on behalf of your sources before thinking about tools and
practices. We’ll also describe common communication channels for
accepting sensitive tips and tradeoffs when using each channel. When
thinking about tradeoffs, consider which channels are right for you.

Let’s talk about how to do it right.

**Someone needs to maintain the page -- is it you?**

If you’re reading this, the person maintaining the secure tip web page
is \*probably\* you.

Before we dive into security concerns, there are a few practical
considerations to think about when building a secure tip page.

1.  We need someone to maintain the page. Again, that’s you.

2.  The page should be somewhere easily accessible, and under your
    > control (no one else’s). This gives would-be sources a reliable
    > place to reach out.

3.  Host secure tip pages with HTTPS, instead of an unsecured
    > HTTP connection. This prevents unwanted third parties from
    > snooping on would-be sources’ connections to your tip page. If
    > possible, your tips page should not be served from a dedicated
    > site (https://tips.example.com), but on the HTTPS version of your
    > public website (https://www.example.com/tips).

4.  Your institution should be prepared to advertise the page widely. A
    > secure tip page only works if people read it *before*
    > reaching out.

Let’s talk about the security concerns to consider for your tip page.

**Who is likely to look into your source, and how?**

The truth is, most tips and sources are not terribly sensitive. But when
there’s a reasonable hint that source confidentiality should be upheld,
pause and think carefully about what information you’re publishing so
they don’t run into trouble.

Think about who would care about this tip being shared with a news
organization and the public (e.g., their employer). What capabilities do
they have (e.g., legal, financial) to investigate the source of the tip?
How likely do you think that it is that anyone will look into it? (Very
likely? Not at all?) What are the potential consequences for your source
if they are discovered?

Based on the capabilities of the source’s potential investigators and
the likely consequences, consider which channels are appropriate for
your communications. For example, if you are concerned about an
organization with few resources to investigate, your sources have a lot
of options for communicating with you—anywhere outside of work. If their
potential investigator is a large government agency, however, chances
are that the agency has resources for investigating the tip, and so the
source needs to be cautious. Encourage them to use the right channels.

When the time comes to publish, if you’re in a position to speak with
your sources, give them a realistic idea about the risks and tradeoffs
of publishing before moving ahead.

**Content versus metadata**

Much like our messages sent through a postcard, routine communications
through email or phone calls are often legible to anyone who gets ahold
of them. That may include your internet service provider,
telecommunications company, or any government that makes a legal request
of those companies. Just as we must write an address on our postcards so
the post office will deliver it correctly, our electronic communications
inevitably require us to share information about where to deliver a
message. This is called metadata — data about who spoke to whom, when,
and for how long.

Even if you secure your conversations, remember that both parties are
still identifiable through metadata. A network eavesdropper may not be
able to read your messages, but they can still see the parties in
conversation. We can’t prevent metadata from being produced, but we can
try to minimize it or make it less useful. For example, you can
encourage sources to call from a phone that is not clearly linked to
them (e.g., at a nearby business). The point isn’t to have no metadata;
it’s to have metadata that is less revealing when analyzed later.

**The first contact problem**

It’s easy for sources to "out" themselves with their metadata trail. If
a source reached out over a work phone or email, they have already left
a juicy metadata trail for their employer. This is sometimes called the
"first contact problem," and there is no quick fix. We need sources to
know the appropriate channels before reaching out.

The best we can do is support the appropriate communication channels,
and advertise that we’re available to check out tips. Have a page where
these channels are clearly organized, and share it with information
about the tradeoffs (e.g., see the [*confidential tips page from the New
York Times*](https://nytimes.com/tips)).

Most secure communications channels do not protect against metadata
surveillance, so make note of these constraints in your documentation.

It’s also important to be be clear that if they have reached out over a
less-than-ideal channel, such as calling from their work phone or using
their work computer, sources may have burned themselves already.

The Intercept has [*an excellent guide*](https://theintercept.com/leak/)
walking through the basics of reaching out anonymously. They are very
clear both about how to reach out, and *what not to do*.

![](media/image2.png)

**Be clear about risk**

Many existing resources also fail to give would-be sources enough
information about the risks associated with reaching out with sensitive
information. News organizations can, and must, do better.

If someone’s at risk of going to losing their job, going to jail (or
worse) for reaching out to you, you owe them a sober explanation. Only
promise the protection you know you can actually provide. They should
know what they’re getting into.

Writing a good tip page needs a delicate touch. You want sources to be
informed, but you also don’t want to scare them away. Write a secure
communications page that helps people understand the risks well enough
to make good decisions, but also does not inspire fear without reason.

**Open secure communication channels and describe the tradeoffs**

Give sources as many ways to reach out as appropriate for your
situation, and describe the advantages and constraints of each channel.

Many of us already have a professional email address, desk phone, cell
phone, or social media accounts (e.g., Twitter, Facebook) to gather
information for stories. These are all great channels for less sensitive
tips, but what do you do if you need to secure your communications?

**Common secure channels**

Some common secure communication channels include
[*Signal*](https://signal.org/), [*WhatsApp*](https://whatsapp.com/),
[*Off-the-record
messaging*](https://wikipedia.org/wiki/Off-the-Record_Messaging), and
PGP for email encryption. Let’s briefly walk through some of the
advantages and tradeoffs for each.

-   [*Signal*](https://signal.org/). Signal is a free and open source
    > secure messaging app for
    > [*iPhone*](https://itunes.apple.com/us/app/signal-private-messenger/id874139669)
    > and
    > [*Android*](https://play.google.com/store/apps/details?id=org.thoughtcrime.securesms&hl=en),
    > developed by [*Open Whisper
    > Systems*](https://whispersystems.org/).

    -   Signal supports encrypted messaging and phone calls. Signal’s
        > developers designed the service to retain as little metadata
        > as possible—only the user’s phone number, sign-up time, and
        > the time when the user was last active. It also allows
        > messages to "self-destruct" automatically after a preset
        > amount of time, leaving behind as little information
        > as possible. For help getting started, read [*Signal for
        > Beginners*](https://medium.com/@mshelton/signal-for-beginners-c6b44f76a1f0).

    -   Tradeoffs: While Signal’s servers retain [*nearly no
        > metadata*](https://whispersystems.org/bigbrother/eastern-virginia-grand-jury/)
        > (only the phone number, sign-up date, and the user’s last
        > sign-in date), the app is also not designed to prevent live
        > metadata surveillance. The users in conversation should not be
        > considered anonymous.

-   [*WhatsApp*](https://whatsapp.com/). With over a billion users on
    > [*iPhone*](https://itunes.apple.com/us/app/whatsapp-messenger/id310633997)
    > and
    > [*Android*](https://play.google.com/store/apps/details?id=com.whatsapp),
    > WhatsApp is a popular messaging application that uses similar
    > encryption to Signal. It’s easy to use, and with the right
    > settings, can be a decent option for routine communications.
    > WhatsApp can share more types of files than Signal, and it can be
    > a great way to send documents.

    -   Tradeoffs: Importantly, some settings must be tweaked in order
        > to maximize the security benefits of the app, and to make it
        > safer for routine use. For example, WhatsApp may be backing up
        > your unencrypted messages to iCloud or Google Drive, and you
        > need to turn backups off. To learn more about how to improve
        > the app’s security, read [*Upgrading WhatsApp
        > Security*](https://medium.com/@mshelton/upgrading-whatsapp-security-386c8ce496d3).

    -   Like Signal, WhatsApp stores user phone numbers. Note that
        > WhatsApp is owned by Facebook and shares the user’s phone
        > number (which can help Facebook map connections) and user
        > analytics with the social media company. Facebook can also be
        > forced to share its troves of user data in response to a court
        > order or subpoena.

-   [*Off-the-record*](https://en.wikipedia.org/wiki/Off-the-Record_Messaging) (OTR)
    > messaging. OTR is a messaging encryption standard. OTR can be
    > installed as a plug-in for messaging clients, such as
    > [*Pidgin*](https://pidgin.im/) or [*Adium*](https://adium.im/),
    > typically using an open messaging standard called
    > [*XMPP*](https://en.wikipedia.org/wiki/XMPP).

    -   It can help you encrypt communications with sources on a variety
        > of inter-operable messaging clients. Read the Electronic
        > Frontier Foundation’s primer on getting started with OTR for
        > [*Windows*](https://ssd.eff.org/en/module/how-use-otr-windows),
        > [*Mac*](https://ssd.eff.org/en/module/how-use-otr-mac), and
        > [*Linux*](https://ssd.eff.org/en/module/how-use-otr-linux).

    -   Note that OTR allows you to accept messages from anyone using an
        > OTR client, including some anonymity-protecting clients such
        > as [*Tor
        > Messenger*](https://blog.torproject.org/blog/tor-messenger-beta-chat-over-tor-easily).
        > If your contacts have the know-how, this can be an asset for
        > protecting anonymity.

    -   Tradeoffs: Not everyone is familiar with OTR, and you’re much
        > more likely to receive an OTR message from a savvy user than
        > anyone else. Note that OTR should not be confused with the
        > "off the record" setting in Google Hangouts.

-   [*Pretty Good
    > Privacy*](https://en.wikipedia.org/wiki/Pretty_Good_Privacy) (PGP)
    > email encryption. PGP is an encryption standard that is becoming
    > increasingly popular among journalists for securing email. PGP
    > uses public key cryptography, meaning that each user has a "public
    > key" used to scramble messages to other users. The public key can
    > be shared with anyone. Each user also has a corresponding "private
    > key" that is used to unscramble messages, and should never
    > be shared. Users typically post their public key in an accessible
    > place, such as a personal website, byline, or a [*PGP public
    > keyserver*](https://pgp.mit.edu/pks/lookup?search=nytimes&op=index).

    -   The Electronic Frontier Foundation has resources for setting up
        > PGP on
        > [*Windows*](https://ssd.eff.org/en/module/how-use-pgp-windows),
        > [*Mac*](https://ssd.eff.org/en/module/how-use-pgp-mac-os-x),
        > and
        > [*Linux*](https://ssd.eff.org/en/module/how-use-pgp-linux).

    -   Tradeoffs: PGP is not the best choice for secure communications
        > for a few different reasons. It’s infamously tricky to use,
        > even for security geeks. It’s easy to make a mistake that will
        > compromise your sensitive communications. Most importantly for
        > news organizations, PGP only secures the body of an email,
        > leaving email addresses and the subject line exposed
        > to eavesdroppers. You are likely to get more "return on
        > investment" with simpler channels, such as Signal.

**Secure Organizational Channels**

When done properly, physical mail and
[*SecureDrop*](https://securedrop.org/) can both be good ways for
sources to avoid giving personally identifiable information. The catch
is, your sources have to know what to do.

-   Physical mail. Regular old-fashioned mail is a solid way to receive
    > sensitive tips because sources don’t need to give their
    > return address. [*The U.S. postal service takes images of the
    > exterior of paper
    > mail*](http://www.nytimes.com/2013/07/04/us/monitoring-of-snail-mail.html),
    > so if you want, you can encourage sources to put a return address
    > inside the envelope instead. Physical mail can be a great way to
    > send physical documents as well as electronic media, such as SD
    > cards or small USB devices.

-   Tradeoffs: The main drawback is that physical mail represents a
    > one-off communication. If you advertise your office address for
    > accepting tips, encourage sources to give you a way to reach them
    > so that you can ask them about any materials they share.

-   [*SecureDrop*](https://docs.securedrop.org/en/stable/index.html).
    > SecureDrop is an encrypted submission system that can help news
    > organizations receive documents and exchange messages
    > with sources. SecureDrop uses the Tor anonymity network, which
    > encrypts and bounces web traffic around the globe, making it much
    > more difficult for eavesdroppers to determine the original source
    > of a tip. This is one of the best options available for
    > protecting confidentiality.

-   SecureDrop requires dedicated equipment and an administrator
    > familiar with the basics of Linux and Bash shell. [*Learn more
    > about setting up SecureDrop
    > here*](https://docs.securedrop.org/en/stable/index.html).

-   Tradeoffs: With SecureDrop, sources don’t need to provide
    > identifying information unless they choose to do so. The added
    > protection for sources can sometimes present challenges for
    > newsrooms that need to verify the legitimacy of an anonymous leak.

**Verification**

Consider (1) verifying their information independently by asking
experts, (2) other previous "insiders" (perhaps not present insiders)
who might understand the leak, or (3) consider having a conversation
with your source about information they can give that would verify their
identity without giving information that would be meaningful to their
organization. For example, you can ask them to post a nondescript phrase
in a tweet — visible to anyone, but only meaningful to you.

While it is possible for individual reporters to have individual
SecureDrop pages (e.g., [*Bart Gellman*](https://tcfmailvault.info/);
Wired.com’s [*Kevin
Poulsen*](https://freedom.press/people/kevin-poulsen/)), it takes a fair
bit of know-how. For most, having institutional support is ideal.

**Pay Attention to File Metadata**

If you’re going to publish files from a source, look out for file
metadata. Metadata is information about a file, such as its creator or
associated GPS coordinates. You can accidentally burn sources by
publishing metadata alone.

This isn’t new. Back in 2012, [*Two Vice journalists accidentally outed
the location of then-billionaire-in-hiding, John
McAfee*](https://www.wired.com/2012/12/oops-did-vice-just-give-away-john-mcafees-location-with-this-photo/).
How? They shared a picture on their website. It turns out the image was
taken an iPhone 4S, and appended GPS metadata. It’s pretty easy to
analyze images for appended metadata, and a growing number of web-based
tools make this process painless (e.g.,
[*http://exifdata.com/*](http://exifdata.com/)).

Consider whether it’s appropriate to publish original documents with
their file metadata intact. You can often remove metadata by converting
the file into a new format (e.g., by taking a screenshot of a document).

-   It’s fairly easy to scrub unwanted metadata on
    > [*Windows*](http://www.digitalcitizen.life/what-file-s-metadata-and-how-edit-it).

-   For those who feel comfortable with Bash, consider using the
    > [*Metadata Anonymisation Toolkit*](https://mat.boum.org/).

To learn more, [*please read our section for lessons on scrubbing
metadata*](https://docs.google.com/document/d/1MS9MoeXmXw_TYOmjXto9mvg-EROL5vds2sl5zytQTZk/edit#).

**Unsafe devices lead to unsafe sources**

Your conversations are only as secure as your devices. Be aware of a few
different ways your communications can be compromised.

Perhaps it goes without saying, but encryption doesn’t protect you if
someone takes control of your unlocked physical devices. If the device
you use to decrypt your messages gets infected with malware, your
decrypted files are readily available to the remote attacker. And of
course, without strong authentication, there’s not much standing between
a hacker and your sensitive communications over your email, Twitter,
Facebook, or any online account where you chat with sources.

Defend against common attacks to protect your accounts and conversations
with sources. One common way that newsroom accounts and devices are
hijacked is through "phishing" emails—emails that link to a fake login
page, where you’re encouraged to enter your very real login information.

[*Learn more about phishing
here*](https://freedom.press/training/email-security-tips/).

Another common tactic is to encourage reporters to download and launch
malicious file attachments that can give a remote attacker access to
your device. Though you will inevitably open email links from strangers
(it’s part of the job, after all), use caution and learn to identify
suspicious-looking emails. If you’re feeling unsure of a file attachment
in an email, consider whether to open PDFs and Microsoft Office
documents, which are especially popular for distributing malware. If
you’re okay with sharing a document with Google, consider opening it in
Google Docs instead of opening it directly on your computer.

To make it harder for remote attackers to log in and see any
communications with sources, use hard-to-guess passwords (ideally
generated and stored with a [*password
manager*](https://medium.com/@mshelton/password-managers-for-beginners-d1f49866f80f))
and use [*two-factor authentication*](https://twofactorauth.org/).

Learn more about [*how to keep newsroom accounts safe from
hijacking*](https://source.opennews.org/guides/defending-accounts/).

**Consider What’s Right for Your Sources**

Most newsrooms are overworked, and it’s challenging to find the time to
get started with these tools and practices. However, secure tip channels
allow sources to come forward with compelling information, especially
when they are putting their safety or livelihood at risk for sharing
what they know. Secure tip channels also signal to sources that you take
their confidentiality seriously. Consider which options are appropriate
for your organization and your sources.

Here are some additional examples you can look to for inspiration on
your secure tip page:

-   ProPublica:
    > [*https://securedrop.propublica.org/*](https://securedrop.propublica.org/)
    > and "[*How to Leak to
    > ProPublica*](https://www.propublica.org/article/how-to-leak-to-propublica)"

-   The New York Times:
    > [*https://www.nytimes.com/tips*](https://www.nytimes.com/tips)

-   The Washington Post:
    > [*https://www.washingtonpost.com/anonymous-news-tips/*](https://www.washingtonpost.com/anonymous-news-tips/)

    -   See also
        > [*https://www.washingtonpost.com/securedrop/*](https://www.washingtonpost.com/securedrop/)
        > and "[*Here’s how to leak government documents to The
        > Post*](https://www.washingtonpost.com/news/politics/wp/2017/01/25/heres-how-to-leak-government-documents-to-the-post/)"

-   BuzzFeed:
    > [*https://contact.buzzfeed.com/ *](https://contact.buzzfeed.com/)

-   The Associated Press: *https://www.ap.org/tips/*

-   The Guardian:
    > [*https://securedrop.theguardian.com/*](https://securedrop.theguardian.com/)

-   The New Yorker:
    > [*http://projects.newyorker.com/strongbox/*](https://securedrop.theguardian.com/)

-   The Intercept:
    > [*https://theintercept.com/leak/*](https://securedrop.theguardian.com/)

    -   See also
        > [*https://theintercept.com/2015/01/28/how-to-leak-to-the-intercept/*](https://securedrop.theguardian.com/)

-   Vice: *https://news.vice.com/securedrop/*

### Recommended Reading

[*https://source.opennews.org/articles/how-protect-your-sources-when-releasing-sensitive-/*](https://source.opennews.org/articles/how-protect-your-sources-when-releasing-sensitive-/)
