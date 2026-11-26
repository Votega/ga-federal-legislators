# Changes

Changes to this repo's files that a consumer may need to act on. Routine data refreshes are not listed.

## Coming: 3 January 2027, 120th Congress

- `data/` and `ROSTER.md` become the **120th Congress**: its delegation, and from then on its roll calls only. `votes.json` starts nearly empty and fills as the new Congress votes.
- The 119th Congress's final record stays at `sessions/119th/`, frozen before the switch (`freeze.json` will say `"kind": "final"`).

## November 2026

- `data/members.json`: Senators now carry `"district": null`, as the schema and README say. The key used to be missing from their records.
- `sessions/119th/` holds a provisional freeze of the 119th Congress, replaced by the final one before the switch.
- `data/en-bloc-nominees.json` and `.csv` list every nomination behind each Senate en bloc vote.
