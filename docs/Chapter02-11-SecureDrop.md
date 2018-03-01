# Using SecureDrop Securely

## Overview 

SecureDrop is an anonymous whistleblowing tool, built on well-tested cryptographic technologies, and designed to provide its users with a high degree of protection from detection through Internet-based surveillance. This lesson plan covers what you'll need to know to use SecureDrop effectively: establishing a culture of security, setting up SecureDrop securely, and making sure your sources know how to use it safely.

## About This Lesson Plan

**Review date:** 29 Sep 2017<br />
**Lesson duration:** 1 hour (or 90 minutes with the optional demo section)<br />
**Level** (advanced)<br />

**What will participants learn?**<br />
At the end of this session, participants will have a general understanding of how SecureDrop works, what is required to install it, and its strengths and limitations. 

**What materials will participants need?**<br />
A laptop, pen, paper.

**How should participants prepare?**<br />
Participants should visit [*https://securedrop.org/*](https://securedrop.org/) and review information about the system available there.

**What materials will the instructor need?**<br />
Laptop, projector, Android or iOS phone

**How should the instructor prepare?**<br />
Review current SecureDrop documentation at [https://docs.securedrop.org/en/stable/index.html](https://docs.securedrop.org/en/stable/index.html)

Optional: Set up journalist access to Securedrop Demo instance at [https://securedrop.org/demo](https://securedrop.org/demo):

- add journalist userame and password to password manager (or write them on a Post-it!)
- scan QR-code with Google Authenticator app to set up 2FA
- save the private key for the demo instance to their GPG keyring

**Preconditions**<br />
Lesson plans covering basic digital security topics: disk encryption, password management, 2-factor authentication.

## Lesson Plan

**Icebreakers/activities - Discussion**<br />
General: how do you communicate with anonymous sources? How many third parties are involved in those communications?

Journalists - how do you get in touch and maintain contact? Email? Text messages? Postal service? In-person only?

Editors - what are policies around use and confirmation of anons? Can you use verified information, information that’s unverified but highly credible? What about anonymous quotes?

Publishing - what are policies around how stories with anonymous sources get published?

When leaking goes wrong - [*https://en.wikipedia.org/wiki/Reality\_Winner*](https://en.wikipedia.org/wiki/Reality_Winner) \[other examples\]

**Overview**<br />
SecureDrop started off as DeadDrop, a whistleblowing system developed by Aaron Swartz in collaboration with Kevin Poulsen. The system was later renamed SecureDrop, and is now maintained as an open-source project by the Freedom Of The Press Foundation. It's intended to help journalists and anonymous sources communicate securely over the open Internet, and it does so in three ways:

1.  it reduces the number of 3rd parties involved in communication,

2.  it uses tried-and-true cryptographic technologies,

3.  and it isolates critical components from any networks.

These features make SecureDrop a powerful tool, but they also impose strict requirements on how the system is implemented and used. Specifically, you'll need to establish a culture of security, set SecureDrop up securely, and ensure your sources know how to use it safely.

### A culture of security

In order to use SecureDrop, and provide a reasonable guarantee of security for high-risk sources, you should already have some digital-security tools and policies in place.

*\[Discussion: Instructor could ask why this would be important - a good answer would be because leaked documents need to be secured and handled safely within the newsroom, no matter what the source.\]*

At a minimum:

-   The system’s users should keep their electronic devices up-to-date
    with any OS updates and security patches.

-   Full Disk Encryption should be turned on for any related computers,
    smartphones, and storage devices.

-   Strong safe password policies should be mandated and enforced.

-   Users should enable 2-factor authentication for any accounts that
    support it.

Your organization should have existing policies for the sharing and storage of sensitive information (and if it doesn't, you need to create them). These should be reviewed and updated as necessary to cover digital documents. One important thing to consider in this updated policy is whether to reveal the use of SecureDrop in a story. In general, this is not recommended, as it may provide correlating information for someone trying to uncover an anonymous source, but every story is different.

### Setting up SecureDrop

The FPF provides full instructions and hardware requirements for setting up SecureDrop at [https://securedrop.org](https://securedrop.org), and it is possible for a competent Linux adminstrator to set it up themselves. However, given the many ways in which even simple setup mistakes could cripple its security, it's highly recommended that you reach out to the FPF for support and assistance with the initial setup.

A SecureDrop installation has two major components:

-   the public-facing TOR hidden services (the TOR network's equivalent of websites) used by sources and journalists, delivered by two servers behind a hardware firewall.

-   the secure viewing station (SVS) - an air-gapped computer used by journalists to decrypt messages and files from sources.

*\[Discussion: Instructor could ask what kind of challenges participants might face setting up and protecting these servers, both from physical access and from attacks over the Internet, and compare with existing server infrastructure, if they know how and where it's currently hosted.\]*

During setup, an encryption keypair is generated for use by the SecureDrop installation - the public key is used by the hidden services to encrypt submissions, while the private key is stored on the SVS and is used by journalists to decrypt the same files. Because the SVS contains the only copy of the private key, it is critical to keep it secure and limit access. As such, the two system components have stringent physical security requirements.

**Public-facing services**<br />
The public-facing services component includes two servers (typically consumer-grade micro-PCs), a network switch/firewall, and a dedicated Internet connection. Sources use it to upload documents, journalists use it to download uploaded files. You should keep these servers somewhere you can control and monitor, preferably on-site. If they're kept off-site, for example in your datacenter, your hosting company may be legally compelled to give 3rd parties access to them without your knowledge. If a 3rd party has access to these servers, they'll be able to monitor incoming communications, which may compromise your sources. 

**Secure viewing station**<br />
The SVS is an airgapped computer. It's not connected to any network, and ideally has no network or wifi hardware at all. It must be kept in a secure location, and access to it must be strictly limited to the people tasked with downloading and decrypting submissions. When it comes to the SVS, you should be as paranoid as your budget allows. If the SVS is compromised and the private key copied, all your SecureDrop submissions, past and future, can be decrypted.

**Roles and responsibilities**<br />
To maintain and use SecureDrop safely, you'll need to find people in your organization to fulfil the roles below:

- System administrator - they'll need some familiarity with Linux, and will be responsible for updates and backups. They should have access to the public-facing servers, but should not need unsupervised access to the SVS.

- User admin - they'll be responsible for managing journalist access to the system. They should not have unsupervised access to the servers or SVS.

- Journalist - they'll be responsible for checking for submissions and decrypting them via the SVS. They should have access to the SVS but do not need access to the public-facing servers. 

There is no technical restriction on the number of journalists that can be given access to the system, but you should decide how you want to manage access. The more people who have access, the harder it is to secure the SVS. Typically, most organizations will designate a small team of journalists to check the system periodically, relying on them and their editors to pass along any submissions to the appropriate destination in the newsroom.

### Help your sources use SecureDrop safely

Used properly, SecureDrop makes it difficult to intercept communications between you and your sources, but it doesn't work in a vacuum. If your newsroom network or personal computers are compromised, this puts submitted documents at risk. Similarly, if your sources don't take precautions on their end, they may compromise themselves by contacting you. When you provide a link to your SecureDrop instance, whether publicly or privately, you should also provide instructions for sources on using it safely.

*\[Discussion: Instructor should ask participants, given what they know already, what kind of risks a source might face while submitting documents to SecureDrop.\]*

At a minimum, sources need to be aware of these basic points:

- Sources should use a computer they control, that is free of malware and monitoring software. Their employer-issued computer should not be used, as it doesn't meet this requirement. Using a self-contained secure OS like Tails ([https://tails.boum.org/](https://tails.boum.org)) adds an extra level of security here.
- Sources should connect to SecureDrop from a network that isn't associated with them in any way. For example, they should definitely not use their home network, or a coffeeshop network that they use often. Ideally they should find a network connection they've never used before, located somewhere they don't usually go.
- Sources should not contact you via any other method - email, Twitter DMs, or any other social networks. This will reduce the chance of them being exposed by correlating those communications with the content of future stories and the activities of your journalists.

High-risk sources need to take more precautions. The SecureDrop Source Guide ([https://docs.securedrop.org/en/stable/source.html](https://docs.securedrop.org/en/stable/source.html)) provides a comprehensive guide for sources looking to protect themselves against surveillance by state-level actors.


### Alternatives
SecureDrop's requirements might make it not the best fit for your newsroom. In particular, if you can't guarantee the physical security of the public-facing servers or the air-gapped SVS, you should consider other options to support anonymous sources. Traditional methods such as postal mail still work, if sources take the appropriate precautions. GPG-encrypted email is another option, although it can be difficult to use correctly and may leak information about source identities via email metadata. One option worth considering is a newsroom dropbox using Signal, the encrypted messaging platform written and maintained by Open Whisper Systems. Barton Gellmann has written a guide on using Signal as a newsroom dropbox, which you can find here: [https://github.com/b4rton/signal-newsroom/blob/master/README.md](https://github.com/b4rton/signal-newsroom/blob/master/README.md). 


### (Optional) SecureDrop Demo

*\[Practical: Instructor should guide participants through the process of submitting to SecureDrop, using the FPF demo instance at [https://securedrop.org/demo](https://securedrop.org/demo). Participants should play the role of sources, using the source interface to send one or more messages. The instructor should have already configured their access to the demo instance's Journalist interface and be able to decrypt submissions.\]*
 
## Recommended Reading

**Links in the news**<br />
[*https://securedrop.org/directory*](https://securedrop.org/directory) - the Freedom Of The Press Foundation’s directory listing media organizations offering SecureDrop.

[*https://www.wired.com/2015/11/securedrop-leak-tool-produces-a-massive-trove-of-prison-docs/*](https://www.wired.com/2015/11/securedrop-leak-tool-produces-a-massive-trove-of-prison-docs/) - the Intercept confirms use of SecureDrop in a story for the first time.

[*https://twitter.com/fahrenthold/status/785195210347163648?lang=en*](https://twitter.com/fahrenthold/status/785195210347163648?lang=en) - David Fahrenthold of the Washington Post heavily hints at its use during the 2016 US Presidential election.

**More Training Resources**<br />
[*https://docs.securedrop.org/*](https://docs.securedrop.org/) - The official documentation site for SecureDrop, maintained by the Freedom Of The Press Foundation.

