# Super Mario Maker 2 — public game data

Public data parts for the SMM2 web port on dilldoe-games.pages.dev.

Each large file is split into numbered parts (`name.000`, `name.001`, ...) because the
static host caps files at 25 MiB. `split.json` lists, for each original file, how many
parts there are and its total size; the port streams the parts back to back.

`gamedata/manifest.json` and `gamedata/*.data` are the game's packed romfs; the port
copies them into the browser's private file storage on first start.

Not affiliated with Nintendo.
