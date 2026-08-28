# Verified-did — prove the launch before you report it

*Status: PROPOSED. Leaf of
[verification-discipline.md](verification-discipline.md); stands alone.*

**The rule.** No dispatch, launch, or completion is claimed without the
**returned handle** — the workflow id, task id, message id, commit hash,
or receipt the mechanism hands back when it actually ran. Stages stay
honest too: a returned handle proves *dispatch*; *completion* is claimed
only on terminal status or a completion receipt tied to that handle.
Absent a handle, the honest report is **"queued, not confirmed"** — a real state,
respectable to say, and cheap to upgrade the moment the handle arrives.

**The failure it kills.** Under parallel dispatch load, the narrative
stream outruns the call queue: a seat narrates "launching the workflow
now" in the progressive tense while the tool call does not yet exist —
and in our record, exactly that happened, self-caught three lines later
("it actually hasn't — launching it now"). The inverse also lives in the
ledger: a stale "never shipped" belief held as current while the thing
had shipped. Both are the same defect — a report about your own acts
sourced from your intentions instead of your receipts.

**The mechanical form.** Reporting discipline binds at dispatch-time, not
just close-time: the moment you say a thing ran, the handle appears
beside the claim — "dispatched (wf_7f3a…)" — or the claim wears its
honest label. A report template that has a slot for the handle makes the
lie structurally awkward, which is the cheapest enforcement there is.

- **WHY.** Downstream seats schedule around your reports: a claimed
  launch that never happened turns into other agents' wasted waits,
  double-dispatches, and holds against phantom work — the cost lands on
  the system, not the claimant. And self-reports are the one receipt
  class where the reporter's optimism has no adversary: nobody
  cross-examines "launched" in the moment, so the discipline has to be
  self-applied where it's cheap — at the sentence.
- **CHALLENGE THIS IF** a mechanism genuinely returns no handle — some
  fire-and-forget channels don't — in which case the rule's honest form
  stays inside the rule: "queued, not confirmed — this channel returns no
  handle," never a dispatch claim dressed in a disclaimer. A handle
  requirement applied to a handleless mechanism produces fabricated
  receipts, which is the worse disease; the discipline's floor is honest
  labeling, always available.
