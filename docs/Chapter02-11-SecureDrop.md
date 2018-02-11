Planning for Securedrop - how to get it, how to use it
======================================================

## Overview 

SecureDrop is an anonymous whistleblowing tool, built on
well-tested cryptographic technologies, and designed to provide its
users with a high degree of protection from detection through
Internet-based surveillance. This lesson outlines organisational and
technical prerequisites for its installation and use, and helps
participants to complete a top-level roadmap for the deployment of
SecureDrop in their own organization.

**ABOUT THIS LESSON PLAN**

**Review date:** 29 Sep 2017

**Lesson duration:** \[ TBD \]

**What will participants learn?**

At the end of this session, participants will have a general
understanding of how SecureDrop works, what is required to install it,
and its strengths and limitations. They will be able to relate its
requirements to the needs and capabilities of their own organizations,
and will have used the FPF demo SecureDrop site to work through the process of submitting and decrypting a document.

**What materials will participants need?**

A laptop, pen, paper.

**How should participants prepare?**

Participants should visit
[*https://securedrop.org/*](https://securedrop.org/) and review
information about the system available there.

**What materials will the instructor need?**

Laptop, projector, Android or iOS phone


**How should the instructor prepare?**

Review current SecureDrop documentation at
[https://docs.securedrop.org/en/stable/index.html](https://docs.securedrop.org/en/stable/index.html)

Set up journalist access to Securedrop Demo instance at [https://securedrop.org/demo](https://securedrop.org/demo):

- add journalist userame and password to password manager (or write them on a Post-it!)
- scan QR-code with Google Authenticator app to set up 2FA
- save the private key for the demo instance to their GPG keyring

**Level** (advanced)

**Preconditions**

\[GPG lesson plan - TK\]

\[TOR lesson plan - TK\]

**Links in the news**

[*https://securedrop.org/directory*](https://securedrop.org/directory) -
the Freedom Of The Press Foundation’s directory listing media
organizations offering SecureDrop.

[*https://www.wired.com/2015/11/securedrop-leak-tool-produces-a-massive-trove-of-prison-docs/*](https://www.wired.com/2015/11/securedrop-leak-tool-produces-a-massive-trove-of-prison-docs/)
- the Intercept confirms use of SecureDrop in a story for the first
time.

[*https://twitter.com/fahrenthold/status/785195210347163648?lang=en*](https://twitter.com/fahrenthold/status/785195210347163648?lang=en)
- David Fahrenthold of the Washington Post heavily hints at its use
during the 2016 US Presidential election.

**LESSON PLAN**

**Icebreakers/activities - Discussion**

General: how do you communicate with anonymous sources? How many third
parties are involved in those communications?

Journalists - how do you get in touch and maintain contact? Email? Text
messages? Postal service? In-person only?

Editors - what are policies around use and confirmation of anons? Can
you use verified information, information that’s unverified but highly
credible? What about anonymous quotes?

Publishing - what are policies around how stories with anonymous sources
get published?

When leaking goes wrong -
[*https://en.wikipedia.org/wiki/Reality\_Winner*](https://en.wikipedia.org/wiki/Reality_Winner)
\[other examples\]

**Overview**

SecureDrop started off as DeadDrop, a whistleblowing system developed by
Aaron Swartz in collaboration with Kevin Poulsen. The system was later
renamed SecureDrop, and is now maintained as an open-source project by
the Freedom Of The Press Foundation. It's intended to help 
journalists and anonymous sources to communicate
securely over the open Internet, and it does so in three ways:

1.  it reduces the number of 3rd parties involved in communication,

2.  it uses tried-and-true cryptographic technologies,

3.  and it isolates critical components from any networks.

These features make SecureDrop a powerful tool, but they also impose
strict requirements on how the system is implemented and used.

**Prerequisite - a culture of security**

In order to use SecureDrop, and provide a reasonable guarantee of
security for high-risk sources, you should already have some digital
security tools and policies in place.

*\[Instructor could ask why this would be important - a good answer
would be because leaked documents need to be secured and handled safely
within the newsroom, no matter what the source\]*

At a minimum:

-   The system’s users should keep their electronic devices up-to-date
    with any OS updates and security patches.

-   Full Disk Encryption should be turned on for any related computers,
    smartphones, and storage devices.

-   Strong safe password policies should be mandated and enforced.

-   Users should enable 2-factor authentication for any accounts that
    support it.

Your organization should have existing policies for the sharing and
storage of sensitive information (and if it doesn't, you need to create them). These should be reviewed and updated
as necessary to cover digital documents. One important thing to consider in this updated policy is whether or not to reveal the use of SecureDrop in a story. In general, this is not recommended, as it may provide correlating information for someone trying to uncover a leaker, but every story is different.

**Physical Requirements**

A SecureDrop installation has two major components:

-   the public-facing TOR hidden services used by sources and
     journalists, delivered by two servers behind a hardware firewall.

-   the secure viewing station (SVS) - an air-gapped computer used by
     journalists to decrypt messages and files from sources.

During setup, an encryption keypair is generated for use by the
SecureDrop installation - the public key is used by the hidden services
to encrypt messages and files, while the private key is stored on the
SVS and is used by journalists to decrypt the same files. Because the
SVS contains the only copy of the private key, it is critical to keep it
secure and limit access. As such, the two system components have
stringent physical security requirements.

**Public-facing services**

The public-facing services component includes two servers (typically
consumer-grade micro-PCs), a network switch/firewall, and a dedicated Internet connection.
Sources use it to upload documents, journalists use it to download
uploaded files. You should keep these servers somewhere you you can control and monitor, preferably on-site. If they're kept off-site in your datacenter, your hosting company may be forced to give 3rd parties access to them without your knowledge. If a 3rd party has access to these servers, they'll be able to monitor incoming communications, which may compromise your sources. 

**Secure viewing station**

The SVS is an airgapped computer. It's not connected to any network, and ideally has no network or wifi hardware at all. It must be kept in a secure location, and access to it must be strictly limited to the people tasked with downloading and decrypting submissions. When it comes to the SVS, you should be as paranoid as your budget allows. If the SVS is compromised and the private key copied, all your SecureDrop submissions, past and future, can be decrypted.

**Roles and responsibilities**

To maintain and use SecureDrop safely, you'll need to find people in your organization to fulfil the roles below:

- System administrator - they'll need some familiarity with Linux, and will be responsible for updates and backups. They should have access to the public-facing servers, but should not need unsupervised access to the SVS

- User admin - they'll be responsible for managing journalist access to the system. They should not have unsupervised access to the servers or SVS

- Journalist - they'll be responsible for checking for submissions and decrypting them via the SVS. They should have access to the SVS but do not need access to the public-facing servers. 

There is no technical restriction on the number of journalists that can be given access to the system, but you should decide how you want to manage access. The more people that have access, the hard it is to secure the SVS. Typically, most organizations will designate a small team of journalists to check the system periodically, relying on them and their editors to pass along any submissions to the appropriate destination in the newsroom.

**Help your sources use Securedrop safely**

Used properly, SecureDrop makes it difficult to intercept communications between you and your sources, but it doesn't work in a vacuum. If your newsroom network or personal computers are compromised, this puts submitted documents at risk. Similarly, if your sources don't take precautions on their end, they may compromise themselves by contacting you. When you provide a link to your SecureDrop instance, whether publicly or privately, you should also provide instructions for sources on using it safely, covering at these basic points:

- Sources should use a computer they control, that is free of malware or monitoring software. Their employer-issued computer should not be used, as it doesn't meet this requirement. Using a self-contained secure OS like Tails ([https://tails.boum.org/](https://tails.boum.org)) adds an extra level of security here.
- Sources should connect to SecureDrop from a network that isn't associated with them in any way. For example, they should definitely not use their home network, or a coffeeshop network that they use often. Ideally they should find a network connection they've never used before, located somewhere they don't usually go.
- Sources should not contact you via any other method - email, Twitter DMs, or any other social networks. This will reduce the chance of them being exposed by correlating those communications with the content of future stories and the activities of your journalists.

High-risk sources might need to take even more precautions. The SecureDrop Source Guide ([https://docs.securedrop.org/en/stable/source.html](https://docs.securedrop.org/en/stable/source.html)) provides a comprehensive guide for sources looking to protect themselves against surveillance by state-level actors.


Alternatives

> Do you really need it?
>
> Other options - a Signal tipline
