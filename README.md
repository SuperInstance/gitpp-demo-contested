# gitpp-demo-contested

A live demonstration of git.pp's **retraction law** (dispute + settlement,
git.pp-ng v0.2.0) — including the part the law exists to make visible: a
retraction its target's author still stands behind is marked
**contested**, never silently voided.

## The story in six records (`.gitpp/records/`)

1. `genesis` (task, harbor-master) — the harbor is open.
2. `freeze-1` (override, harbor-master) — a storm front freezes the
   harbor to all berth claims. Authoring a landed override makes
   harbor-master captain-class.
3. `claim-berth-7` (task, agent-north) — written off a stale view that
   descends only from genesis: agent-north claims berth 7 anyway.
4. `dispute-claim` (dispute, agent-south) — disputes the claim: the
   freeze already stood, so berth 7 was never agent-north's to take.
5. `settle-dispute` (settlement, harbor-master) — the captain upholds
   the dispute. The claim's effects are voided (`berth.7` derives to
   nothing), but because agent-north **neither filed the dispute nor
   authored the settlement**, the retraction is marked **contested**
   in the Check, with the dispute and settlement named.
6. `witness-tide` (witness, agent-south) — an ordinary record that
   survives untouched: the tide gauge reads rising.

## What to look at

The `git.pp state - contested-demo` Check on the latest commit: the
derived state (harbor frozen, no berth 7) and the **Retractions**
section naming `claim-berth-7` as retracted and **contested**.

Re-derive it yourself with the fold in
[patchwork-quilt/gitpp-action](https://github.com/patchwork-quilt/gitpp-action)
or the spec and conformance corpus in
[patchwork-quilt/git.pp-ng](https://github.com/patchwork-quilt/git.pp-ng).
