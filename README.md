# GTA 6 PC Port Progress: open data

Stage, frame-rate and test-hardware data for the open-source projects that try to run the Xbox Series build of GTA 6 on Windows. This is the dataset behind the live tracker at **[gtapcport.org](https://gtapcport.org/)**.

No game files, code, dumps or download links are included or linked here. Every project needs the user's own copy of the game.

## Files

| File | What it is |
|---|---|
| [`data/projects.json`](data/projects.json) | Snapshot of every tracked project: repository, stage, reported frame rate, test hardware |
| [`SCHEMA.md`](SCHEMA.md) | Field descriptions and the stage scale |

The snapshot here is updated by hand from time to time. The **current** data, re-read from every project README twice a day, is always available as JSON at:

```
https://gtapcport.org/_d/tracker/projects
```

## The six stages

Progress is never expressed as a percentage. Each project sits on one stage, taken only from what its own README reports:

| # | Stage | Meaning |
|---|---|---|
| 1 | Groundwork | The game has not been run yet |
| 2 | Boots | The executable starts and shows first screens |
| 3 | Menus | Start screen, loading or the opening cutscene |
| 4 | World renders | The 3D world is drawn |
| 5 | In control | The player moves the character or plays a mission |
| 6 | Playable | The README says it is playable **and** reports 25+ fps in the world without regular crashes |
| 0 | Removed | The repository is no longer available on GitHub |

As of the snapshot date, no project is at stage 6.

## Using the data

- Frame rates and hardware are quoted as each README states them; they are developer reports, not independent tests.
- Please credit "GTA 6 PC Port Progress (gtapcport.org)" and link to the project's own GitHub page for any claim you repeat.
- Corrections and missing projects: open an issue with a link to the project's README.

## Related pages

- [Live board of every project](https://gtapcport.org/)
- [All projects by stage](https://gtapcport.org/projects)
- [Can I run the GTA 6 PC port? (requirements)](https://gtapcport.org/can-i-run-gta-6-pc-port)
- [GTA 6 PC port trackers compared](https://gtapcport.org/gta-6-pc-port-progress-trackers-compared)

Grand Theft Auto and GTA are trademarks of Take-Two Interactive Software. This dataset is independent and not affiliated with Rockstar Games or Take-Two Interactive.
