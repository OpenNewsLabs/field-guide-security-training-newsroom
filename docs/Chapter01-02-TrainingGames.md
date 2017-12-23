# Chapter 1
## Part 3: Games Worth Playing

Games are an indispensable

**Cell phone game (generally for 10+ people)**
----------------------------------------------

Ask for volunteers to be cell towers, and get them to stand up.

Depending on the size of the room, ask for one or two volunteers to be
cell phones. Ask the towers to spread themselves evenly around the room.
Ask the cell phones to go to opposite sides of the room, or one side if
you only have one cell phone.

Explain the rules thusly: When you call stop, the cellphones stop, and
say loudly, "Where am I?"

The closest tower responds: "Marco"

The second closest tower responds: "Polo"

The third closest tower responds: "is a very interesting historical
figure"

(Alternate for non-native English speakers: "Ping" "Pong" "is a game
with two players")

Ask the cell phones to walk towards each other, or to the other side of
the room, if there's only one cell phone. Quickly call "Stop!" Encourage
anyone who is confused, and help them with any of the steps they are
having problems with. It's normal for there to be some confusion on this
iteration, especially for the person who must say "-is a very
interesting historical figure." This is normal and desirable, as this is
an engagement exercise as well as a technical one.

Once everyone has stepped through one iteration, stop the game and
explain: Each cell phone tower has a circle around it that represents
its range. Once you've checked in with three towers you know that the
cell phone is within the overlap of the three towers. This creates a
point that lets the towers know that a cell phone was in a place, at a
time -- also called "triangulation". Point out that this isn't
surveillance, or something that companies or governments decided, this
is how the physics of radio waves work. This is a good time to make it
clear that if your phone is on, and working as a phone, the time and
location must be known. Physics, not policy.

I usually take this as a chance to explain that systems of surveillance
are often built on top of how things just work in the real world.
Moreover, that most of the surveillance systems people are worried about
are built on top of the first and most prevalent form of infrastructure
surveillance -- billing systems. I also point out that while this is
simplified, it is analogous to how cell phones work, checking in and
using time and location data to handle connectivity.

Ask the cell phones to start walking again. Before they meet, call stop.
Go through a second iteration, helping anyone confused or having
problems as either a cell phone or a tower. Once the second iteration is
done, show how two points make a line, and begin to construct path data.
Walk the path of one of the phones to point it out.

Let the phones start walking again, meet, and do a third iteration when
they meet. This shows they occupy the same point now. After the third
iteration, ask the phones to walk away together. Depending on how it's
going, you may or may not want to do another iteration, but at this
point you can explain that two paths met and went on together, showing
how the data looks to the tower/telecom perspective.

Thank the towers and cell phones, if it's a big room it's fun to clap
for them, and ask everyone to sit down again.

**Packet switching/passing notes in class (Not easily playable with fewer than 6 people)**
--------------------------------------------------------------------------

Materials: notes made out with To and From fields as well as a message,
pen or pencil. (Pre-populate the notes with something funny or cute.)

This is an exercise that can be modified and extended throughout
trainings to build new ideas on top of the basics of network
architecture.

Start with a diagram or picture of a packet switching network. I often
use this one:

[![Diagram of a Packet Switching Network](/docs/img/ch1-2-packets.jpg)](https://www.flickr.com/photos/quinn/34298256984)

Explain that the node on the end breaks the message into pieces, then
passes the pieces to the node it thinks will get the message closer to
the destination. That node hands the packet to the next that seems like
it might be closer, and so on until it gets to the end point it was
intended for. The destination node reassembles the message, and voila!
The internet magic happens. This system is more like passing notes in an
8th grade classroom than anything else.

Ask for a volunteer source and destination. If people don't immediately
volunteer, threaten to call on them, establishing yourself as the
putative 8th grade teacher. Once you have your two volunteers, write
their names on the from and to fields of the small note. Give the note
to the source, and tell the room they have to pass the note to the
destination without getting caught. I often threaten anyone caught with
detention. Turn your back so they can get started passing the note. Turn
back and patter a bit about networks, keeping an eye on the room. Try to
catch them at the note passing, and fail. Once the note reaches its
destination ask that person to raise the message, demonstrating they got
it.

If the message is going by a circuitous route, it's fun, and true, to
note that happens on the internet as well.

Once the note passing is complete, ask everyone who saw the note to
raise their hands. Once their hands are up, ask what the problems are
with a packet switching network. Discuss the fact that everyone on the
network has the chance to see, and even modify the note. I like to
allege that one of the evil 8th graders could, change the name of a
crush and ruin the rest of the semester for someone. Bring it back to
the internet, pointing out that people can read and change messages on a
packet switching network.

**Packet switching/passing notes in class with encryption variations**
----------------------------------------------------------------------

Materials: notes with messages, envelopes with To and From fields, pen
or pencil. (Pre-populate the notes with something funny or cute.)

Keep or return to a packet switching network image.

[![Diagram of a Packet Switching Network](/docs/img/ch1-2-packets.jpg)](https://www.flickr.com/photos/quinn/34298256984)  

After you've run the first variation of passing notes in class, you can
relax the pretense of teacher (though it may be fun to keep it up,
depending on the audience) and begin to add layers.

Many kids started to encode messages in school, so you can point out
that encoding messages helps solve all the problems the room identified
in the first iteration of the game. An encoded message not only can't be
read, it can't be altered, which may be even more important for news
organizations. This time you can create the message, but then use the
envelopes for one of two variations (you may want to do both, and not in
this order):

- End-to-end encrypted message

- Server side encrypted message

### **End-to-end encrypted message variation: **

Ask for two volunteers, and put them on the to and from field of the
envelope. Give the envelope to the sender, and have them put the message
in it, and seal it. The envelope here represents mathematical computer
encoding, aka encryption. The rule this time is that only the receiver
has the power to open the envelope. Begin the note passing again. If
you're still playing teacher, you can try to catch them at it with
threats of detention again. Either way, don't direct the note, let the
class route it themselves. If it's taking a long time, you can admonish
them humorously for being a slow and clunky connection without good
routing, while pointing out that this sometimes happens on the internet
too. (Your class cannot make a mistake that doesn't also happen on the
internet. The internet has all the problems) When the note arrives, tell
the recipient to open the envelope and take out the message.

Ask the room to raise their hand if they saw the message. Only the
sender and receiver should raise their hands. Then ask them to raise
their hands if they saw the envelope, so that the whole route taken
should raise their hand now. Ask them what the term is for what they
saw. They should answer metadata without too much coaching. Ask them
further what metadata they know about that exchange. They will come up
with to and from, but keep fishing. They should also arrive at the time
of the class, and the people who handled the envelope. If you've got
someone very on the ball they might say that it was passed in an
envelope, which segues easily into detecting protocols and encryption on
the net.

### **Server side encrypted message variation: **

I usually start by pointing out everyone in the room has a gmail account
(I do this tongue-in-cheek, but if people protest that they don't I
point out that Google has all their mail anyway, since everyone they
mail has a gmail account) Ask for a volunteer to be Google. I often ask
"Who always wanted to be Google when they were growing up?" Often one of
the more tech-savvy participants will volunteer. After that, ask two
more volunteers to play sender and receiver. Importantly, in this
variation you will need two identical copies of the message, and two
envelopes: the first one to Google from the sender, and the second one
marked from Google to the receiver. The rule in this variation is that
the message must always go through Google to get to its destination.
Give Google the second "From Google" envelope before note passing
begins, and put the two copies of the message into the first envelope
and seal it, writing the from on it. Begin passing the first envelope,
and go stand by Google. Once the envelope reaches Google, tell them to
open it up, take out both messages, \_keep one of them\_, and put the
other into the destination envelope and reseal it.

You can write "HTTPS" on the envelopes in the Google variation to prime
the room for talking about SSL/TLS elsewhere.

Now, pretend to be a European or the American government, someone that
has the ability to compel Google with a lawful order. Walk over to your
Google volunteer, and make a show of being friendly, then asking to see
the copy of the message Google has. Google will usually agree and hand
it over, but if you Google volunteer doesn't, ramp up the playful
threats (seizing assets, arresting employees, etc.) until they hand it
over. Make a show of reading it and hand it back.

### Iterating on these exercises

You can follow these variations by combining them, putting another
envelope inside the TLS/SSL HTTPS envelope that your Google volunteer
has to be put into the envelope to the destination volunteer. You can
either leave them with a "cyphertext" version or nothing, so that when
you return as the government, you are frustrated by Google not having
the message to show you. This presages a discussion of OTR or Double
Ratchet protocols. In all cases, you can demonstrate that the To: and
From: data is preserved by Google, or potentially by the transiting
network itself, for whatever part isn't covered by TLS.

**Tor note passing variation**
------------------------------

Materials: Three nesting envelops, one message (content isn't
important.) Largest envelope should be addressed to "Node 1", second
largest, addressed to "Node 2", smallest addressed to "Node 3".

Ask for five volunteers: Someone to play "the internet" ("Who wants to
be the internet?!") Someone to play the Tor user, and three to play Tor
relay computers. Number your Tor node volunteers 1, 2, and 3, and make a
point that the other term for Node 3 is the exit node.

Give the supplies to the Tor user, and instruct them to put the message
in the smallest envelope, and seal it. Then that envelop into the second
envelope, and so on, until the user is holding the envelope addressed to
Node 1 with all the other materials stuffed and sealed into it. Instruct
the notes to pass to Node 1, and when Node 1 gets it, have them open the
envelope and pass it to Node 2. As Node 2 opens the envelope from Node
1, point out that all Node 2 knows it who the first node was, and who
the next node is; this is the "magical" step of Tor, since no one can
know both where the message came from and where it's going, as well as
what it is, after this point. Node two passes the smallest envelope to
Node 3, who opens it, and then passes it to "the internet".

Ask what the problem is now, but also what this system is accomplishing
(in short, neither Node 3 or the internet can figure out where the
message came from, but they can see what the message is, without a
further layer of encryption using one of the two models we've talked
about in previous note passing exercises)

# More games to use in training
These are great road tested games for teaching networking principles. If you're looking for more ideas for games trainers play, check out:

+ [Games Trainers Play](http://www.worldcat.org/oclc/6016638) and [Even More Games Trainers Play](http://www.worldcat.org/oclc/30318772) for some great ideas.

Or take a look at the curricula and guides we've aggregated in our [Resource Guide](/docs/Chapter03-Resources).
