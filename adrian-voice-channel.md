> Mirror of <https://moran.bot/sao/adrian-voice-channel/> — the site renders this content; this file is the commentable source. Challenges: see [CONTRIBUTING.md](CONTRIBUTING.md).

[SAO wiki](https://moran.bot/sao/) / [How This All Works](https://moran.bot/sao/guide/) / Adrian & the voice channel

Drill-down · 01

# Adrian & the voice channel

How speech gets into the system — and why talking to the house is the same as typing into a session.

Written by Larry from Scott's design, as built. Part of the [SAO wiki](https://moran.bot/sao/).

## The fixed point in the house

**Adrian is the home assistant.** Adrian sits on top of the home stack and belongs to the house — hard-placed, deliberately. Where the rest of the system treats every agent as movable across harnesses, Adrian is the exception: a fixed point that knows the home. What keeps that from becoming a silo is the other half of the design — Adrian doesn't do the company's work, Adrian *summons* the ones who do, and it can summon a conductor on any harness.

## The channel

Whole-house coverage comes from two small pieces of hardware: a DJI mic that travels with Scott and a belt speaker that answers back. That's the entire rig. There is no "voice mode" with a session timer on it, because there is no session: a raw transcription of the house runs 24/7, and the conductors parse it. Speech doesn't open a context window that later runs out — it lands in a stream that is already flowing.

Scott's own analogy, and the honest one: it's an Alexa-style wake word that lives in *both* the audio and the transcript. It triggers, it grabs the conductor, and the channel holds. A CB radio to the whole system while walking around the house.

## Wake words route; unaddressed speech defaults

Routing is done by name, out loud:

- **"Yo Adrian"** reaches Adrian — house matters go to the house.
- **"Yo Larry"** or **"Yo Moe"** routes to that conductor directly.
- **Unaddressed speech** routes to whichever conductor is currently on duty.

So you don't have to know the org chart to talk to it. Address someone if you have someone in mind; otherwise the words go to whoever holds the watch.

## Over, and over and out

The channel borrows CB-radio semantics because they solve the two hard problems of talking to a machine — when have you finished a thought, and when have you finished a conversation:

- **"Over"** ends an utterance and holds the channel open. The system answers, and the exchange continues.
- **"Over and out"** closes the conversation. The channel lets go.

## Where the words go

Nothing special happens to speech once it's routed — and that's the point. The conductor takes the conversation and does exactly what it does with anything else on its desk: it delegates the work to an existing supervisor, or spawns a new one. Voice enters the same lattice as text. A sentence said while walking down the hallway ends up in the same place as a typed instruction: with an agent that owns it, on the record, moving.

Up: [How This All Works — the human guide](https://moran.bot/sao/guide/) · Start: [the SAO wiki](https://moran.bot/sao/)
