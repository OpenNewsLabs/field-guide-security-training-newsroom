# Concept Glossary

There are many ways to talk about digital-security concepts, and the example that really clicks can be different for every person. This resource is less a glossary than a roundup of great analogies and explanations, offering easier ways to explain technical concepts for non-technical users.

**Adding your ideas:** We know this list is incomplete, and it probably always will be! It's a great place for contributions from the journalism-security community, so if you have a favorite concept or helpful analogy to share, we'd love to [hear from you](mailto:fieldguide@opennews.org). Let's make this list a lot longer:

* [Networks](#networks)
* [HTTPS](#https)
* [Certificate Authority](#certificate-authority)
* [Encryption](#encryption)
* [Authentication](#authentication)
* [What is a Computer](#what-is-a-computer)

And if you're looking to build your own expertise as a security trainer, you'll find a community-driven list of resources to help you in [Chapter 3: Resources](Chapter03-01-Resources.md).

## Networks

A network is two or more nodes connected physically and informationally over time. For example:

* Electrical grids
* Social graphs
* Road systems
* [John Snow's cholera map](https://www.theguardian.com/news/datablog/2013/mar/15/john-snow-cholera-map)
* [Packet-switching diagram](https://en.wikipedia.org/wiki/Packet_switching#/media/File:Packet_Switching.gif)

Think about what a network sees when it sees you. On some you look like a billing point, little more than an amount of money owed, with a individual ID number. On some you look like a series of paths: Think about cell phone towers and ATM withdrawals. In a medical network, you look like a series of diagnoses, vital statistics, and a place where medical professional time and drugs vanish. That's what the you-shaped hole in that network looks like. To the electrical grid, your house looks like a point where power vanishes and money comes out. On a smart grid, that portrait is a little more complex. What do you look like on a phone network? You look like data, metadata, and paths from tower to tower. Time stamps, locations, and connections out to nodes on the internet tell the story of your day, and much of your life.

Most surveillance, good or bad, is built on how networks operate on the physical level. They're not nefarious, they're physics.

We live with and in networks every minute of every day. These networks lay over each other and touch all over the place. Once we start thinking about them, what they're shaped like, where we are in them, our contemporary world starts to make more sense.

The net is a packet-switching network. Packet switching is rather like passing notes in class: You hand the note to someone near you, who tries to hand it to someone closer to the person it's intended for. To know where to pass the note, a person has to know who it's going to, and they know who gave it to them. This knowledge is called metadata: the data a network needs to function.

## HTTPS

* [The US CIO's excellent and thorough explanation](https://https.cio.gov/everything/), and [Chrome's Developer Blog](https://developers.google.com/web/fundamentals/security/encrypt-in-transit/why-https) are both excellent explanations of why HTTPS is important.
* [HTTPS as Pigeons](https://medium.freecodecamp.org/https-explained-with-carrier-pigeons-7029d2193351) via Andrea Zanin on freeCodeCamp walks through the core principles of HTTP and HTTPS with some nice pigeon analogies. (Not helpful, but clever, is the [IP Over Avian Carriers](https://en.wikipedia.org/wiki/IP_over_Avian_Carriers) protocol.)
* Wikipedia's [HTTPS entry](https://en.wikipedia.org/wiki/HTTPS)

### What is a Certificate Authority

* [HTTPS as Pigeons](https://medium.freecodecamp.org/https-explained-with-carrier-pigeons-7029d2193351) covers CAs as trusted signatories (but doesn't address Let's Encrypt).

## Encryption

* [Wikipedia's entry on Encryption](https://en.wikipedia.org/wiki/Encryption) is a solid overview.

## Authentication

The [passwords lesson](Chapter02-06-Passwords.md) is a great resource for explaining the process of authentication. But at its core, "authentication" is just the process that a system uses to determine that you are who you say you are.

### Key-Based Authentication

Seth Schoen leads a great workshop on key-based authentication, and the analogy he uses is this: If you remember anything about mathematics, you might remember that it's not that hard to multiply two big numbers together. It takes time if you're only using a pencil, but you can do it. Factoring the product of two primes, however, is a lot harder. You can think of key-based encryption as taking advantage of this disparity.

## What is a Computer (& What is Software)

* As ever, [Wikipedia's entry on Computers](https://en.wikipedia.org/wiki/Computer) is an excellent resource for thinking about definitions.
