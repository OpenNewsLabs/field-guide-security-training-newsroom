Planning for Securedrop - how to get it, how to use it
======================================================

**Overview:** SecureDrop is an anonymous whistleblowing tool, built on
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
and will have written a top-level roadmap for their own deployment of
SecureDrop.

**What materials will participants need?**

A laptop, pen, paper.

**How should participants prepare?**

Participants should visit
[*https://securedrop.org/*](https://securedrop.org/) and review
information about the system available there.

**What materials will the instructor need?**

Projector?

**How should the instructor prepare?**

Review current SecureDrop documentation at
[*https://docs.securedrop.org/en/stable/index.html*](https://docs.securedrop.org/en/stable/index.html)

**Level** (advanced)

**Preconditions**

\[GPG module - or public key crypto intro if there is one\]

\[TOR module\]

**EXAMPLE MESSAGING FOR PARTICIPANTS**

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

**Advance email**

\[ TK \]

**Followup email**

\[ TK \]

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

**Walkthrough or Active Lesson**

\[demo upload could go here - is there a publicized demo Securedrop
instance?\]

**\
Overview**

SecureDrop started off as DeadDrop, a whistleblowing system developed by
Aaron Swartz in collaboration with Kevin Poulsen. The system was later
renamed SecureDrop, and is now maintained as an open-source project by
the Freedom Of The Press Foundation. It is an attempt to solve the
problem of how to allow journalists and anonymous sources to communicate
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

At a bare minimum:

-   The system’s users should keep their electronic devices up-to-date
    > with any OS updates and security patches.

-   Full Disk Encryption should be turned on for any related computers,
    > smartphones, and storage devices.

-   Strong safe password policies should be mandated and enforced

-   Users should enable 2-factor authentication for any accounts that
    > support it.

*\[instructor should refer participants to the first section of the
checklist, and ask them to take a few minutes to fill it in.\]*

Your organization should have existing policies for the sharing and
storage of sensitive information. These should be reviewed and updated
as necessary to cover digital documents.

*\[Another discussion point - what would you do right now if I handed
you a USB key containing what I claimed was the next Pentagon Papers?
Instructor should ask participants to fill in relevant checklist
sections\]*

**Physical Requirements**

A SecureDrop installation has two major components:

-   the public-facing TOR hidden services used by sources and
    > journalists, delivered by two servers behind a hardware firewall.

-   the secure viewing station (SVS) - an air-gapped computer used by
    > journalists to decrypt messages and files from sources.

During setup, an encryption keypair is generated for use by the
SecureDrop installation - the public key is used by the hidden services
to encrypt messages and files, while the private key is stored on the
SVS and is used by journalists to decrypt the same files. Because the
SVS contains the only copy of the private key, it is critical to keep it
secure and limit access. As such, the two system components have
stringent physical security requirements.

**Public-facing services**

The public-facing services component includes two servers (typically
consumer-grade micro-PCs), a network switch, and an Internet connection.
Sources use it to upload documents, journalists use it to download
uploaded files

**Secure viewing station**

Physical Requirements

> Servers and network config - security and maintenance
>
> Secure viewing station (SVS) - protecting the key!

**Roles and responsibilities**

> System admin - access to servers
>
> Admin - access to admin interface to manage users
>
> Journalist - access to journalist interface to download, SVS to
> decrypt

Operational Security

> Control and monitor access to critical components
>
> Secure the servers and keep them local
>
> Secure the SVS and restrict access to it
>
> Help sources use the system effectively
>
> Uploading from unmonitored computers and networks
>
> Avoiding correlation by reducing points of contact
>
> Have a policy about whether or not to reveal the use of Securedrop in
> a story.

Alternatives

> Do you really need it?
>
> Other options - a Signal tipline
