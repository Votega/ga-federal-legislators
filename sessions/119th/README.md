# 119th Congress: Georgia delegation (frozen record)

The Georgia federal delegation's record for the 119th Congress (January 3, 2025 to January 3, 2027), kept as history. Freeze kind: **provisional**, taken 2026-10-30T02:31:01.887493+00:00.

> **Provisional.** The Congress was still sitting when this was taken, so later votes, sponsorships and roster changes are missing. A final freeze replaces it once the Congress has adjourned.

The live files in [`data/`](../../data) describe the current Congress and are replaced at each new Congress. Nothing in this directory is touched by the daily publish.

## Files

- `members.json`, `members.csv`: the 16 delegation members (`members.schema.json`).
- `votes.json`: every recorded roll call (1591) joined to the delegation, in the same shape as the live file (`votes.schema.json`). `votes.csv` and `member-votes.csv` are flat versions.
- `scorecard.json`, `scorecard.csv`: party-unity and participation per member.
- `sponsorship/`: each member's complete sponsored and cosponsored record (392 sponsored, 4601 cosponsored) in the compact form the site uses: `index.json` plus one `<bioguideId>.json` per member, where each row is `[type, number, title, introducedDate, actionDate, actionIdx, policyIdx]` and the last two index that file's own `actions` and `policyAreas` lists. `sponsorship.csv` is the same data, one flat row per bill.
- `freeze.json`: what was frozen, when, from which sources, and with what counts.

## Notes

- Members are keyed by `bioguideId`, Congress.gov's stable id.
- Where a Senate roll call is marked in `votes.json` `metadata.senateRollsFromVoteview`, it was taken from Voteview because senate.gov was unreachable; those records may differ slightly from the official one.
- Reuse is governed by the repository's `LICENSE` and `NOTICE.md`.

