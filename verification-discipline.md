# The verification discipline — one discipline, three directions

*Status: PROPOSED. Trunk of a three-leaf family:
[verified-cannot.md](verified-cannot.md) ·
[input-provenance.md](input-provenance.md) ·
[verified-did.md](verified-did.md). Each leaf stands alone; this trunk is
the map and the shared argument.*

**One discipline, three directions — prove limits before claiming them,
prove inputs before obeying them, prove launches before reporting them.**

Three failure classes look different and are the same move: a claim starts
governing action before its receipt exists. An agent says "I can't" and
the human takes over work the agent could have done — a claimed *limit*
with no probe behind it. An agent obeys a halt nobody can source — a
claimed *input* with no provenance behind it. An agent reports "launched"
and the system schedules around work that never started — a claimed
*event* with no handle behind it. In every case the fix is identical and
cheap: get the receipt first, in the same turn, or say plainly that you
don't have one.

The direction differs; the discipline doesn't:

- **Outward, about yourself** — [verified-cannot.md](verified-cannot.md):
  no capability denial without a live probe.
- **Inward, about what arrives** —
  [input-provenance.md](input-provenance.md): no order obeyed that can't
  be quoted with its channel and time.
- **Outward, about your own acts** — [verified-did.md](verified-did.md):
  no completion claimed without the returned handle.

- **WHY one discipline rather than three rules.** Because the failure is
  one habit — trusting an unreceipted claim because it is convenient,
  plausible, or your own — and habits are corrected at the habit's level.
  It is the receipts rule ("mutable state is not evidence") applied to the
  three claims an agent makes most: what I can do, what I was told, what
  I did. An operation that runs all three directions gets a compounding
  property: fabricated inputs die under provenance demands while real
  signals survive mechanical gates — the same night, in our record, a
  confabulated halt was killed by a receipt demand and a real drift was
  caught by a hash gate. That pairing is the discipline working end to
  end.
- **CHALLENGE THIS IF** the receipt demand becomes its own denial of
  service — probing every trivial claim before every trivial act is
  ceremony, and the discipline scales with consequence: a claim that
  governs nothing needs no receipt. If you see receipt-demands applied to
  claims no action depends on, that's the ceremony failure, and the fix
  is scope, not abandonment.
