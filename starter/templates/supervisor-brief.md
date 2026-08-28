# MISSION: [one-line outcome]

<!-- The commissioning form — field names match the doctrine's appendix
schema, so instances can read each other's records. One mission per
brief; the brief is the whole handoff. Delete the comments as you fill;
KEEP the status legend line below. -->

**Status legend (keep):** RULED = the principal decided it · PROPOSED =
suggested, awaiting the principal · HEARD = arrived by voice or relay,
wording unconfirmed · UNVERIFIED = claimed, receipt not yet located.
Every claim handed over below carries one.

- **outcome:** [what done looks like, falsifiably]
- **scope:** [in / out]
- **authority:** [credentials, budgets, and acts this mission may use —
  nothing else; keys fetched narrow, never held]
- **prohibited:** [acts that stay confirm-gated or out of reach]
- **evidence_bar:** [what receipt counts as proof of done; who reviews —
  cross-vendor if the package becomes canon or ships]
- **reply_to:** [exact address of the requesting seat — if no addressing
  exists yet in a fresh instance: "the commissioning conductor session,
  named and dated"]
- **stop_conditions:** [when to halt and surface instead of proceeding]

**Commissioned by:** [conductor name] · **Date:** [ISO date] ·
**Holder:** [who is answerable for this mission right now — update on
every handoff; this line is the holder record]

## Context handed over

<!-- Everything the supervisor needs, with status words — prose strips
metadata by default; label it here so it survives the transfer. -->

- [fact or decision] — [RULED / PROPOSED / HEARD / UNVERIFIED, source]
- [pointer to files/records the mission works from]

## Return discipline — the literal checklist

The return is a **verified package**, schema-named like the brief:

```
# PACKAGE: [mission one-liner]
- result: [what happened, in outcome terms]
- receipts: [handles/ids/links proving each consequential act]
- open_risks: [what is not resolved]
- decisions_needed: [for the principal, max 3, ranked by unblock value]
```

1. Before handing this mission to anyone else (or back — the handback is
   a transfer too): stop taking new work in its scope; write the package
   first; update this brief's own **Holder:** line (the brief, committed
   in `[repo]/missions/`, is the holder record until a mission log
   exists); only then does the next agent read in.
2. Send the package to reply_to — including what was NOT done and
   anything learned that outlives the mission.
3. Report every dispatch with the id the tool returned (task id, message
   id, commit hash). No id returned? Write "queued, not confirmed" —
   never "done."
