# Find (Ashita v4) with /finddump

A modified copy of the **Find** addon for Ashita v4, adding a `/finddump` command that writes your full inventory to a text file.

Original addon by MalRD, zombie343, and sippius (v4). Version 3.1.0. MIT licensed.

## What /finddump does

Writes every item in every bag to a plain text file, grouped by bag, sorted alphabetically, with stack counts. Storage slips are listed with the gear actually stored on them underneath — so you can see what's on your slips without visiting a Porter Moogle.

It is read-only. It reads inventory from memory and writes one text file. No automation, no network activity, no combat advantage.

Built for checking LuAshitacast gear profiles against items you actually own, offline.

## Usage

    /finddump

Writes to `config\addons\find\gear_dump_charactername.txt` inside your Ashita install folder.

**You must create that folder first.** Ashita does not make it for you. Go to your Ashita install folder, open `config`, make a folder called `addons`, and inside that make one called `find`.

Or skip the folder and give it a path directly:

    /finddump C:\path\to\gear_dump.txt

The filename includes your character name, so running it on a second character won't overwrite the first one's dump.

## Other commands (unchanged from the original)

- `/find <item>` — search your bags for an item
- `/findmore <item>` — same, but also searches item descriptions
- `/finddupes` — list items taking up more than one slot
- `/findslips` — list items you own that can be stored on slips
- `/findslips <1-27>` — same, for one specific slip

## Install

Replace `find.lua` in your Ashita `addons\find\` folder with this one. Keep a backup of the original.

## HorizonXI

Approved by HorizonXI staff on August 6, 2026 (ticket #addon-0008).

## License

MIT, as the original. See the header in find.lua.
