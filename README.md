# AtlasForge Releases

This repository hosts public release ZIPs for **AtlasForge**, a Windows desktop tool for **World of Warcraft 1.12.1 ADT/WMO editing and patch building**.

AtlasForge can browse game assets, preview WMO/M2 models, edit ADT tile placements, work with custom WMO doodads, and build changes into a client patch using **Ladik's MPQEditor**.

## Latest Release

**AtlasForge `0.1.0-beta`**

This is the first public/community beta release. It is beta software, so please back up your client patch files and test small edits first.

## Download

Download the latest ZIP from this repository:

```text
AtlasForge-0.1.0-beta.zip
```

Extract the ZIP before running the app.

## Install

1. Extract the full `AtlasForge` folder from the ZIP.
2. Keep `AtlasForge.exe` beside the `_internal` folder.
3. Run `AtlasForge.exe`.
4. Complete the Setup Wizard.
5. Let AtlasForge Doctor run after setup.

Do **not** move `AtlasForge.exe` out of the extracted folder. It needs `_internal` beside it.

## Requirements

You need:

- Windows.
- A local World of Warcraft `1.12.1` client `Data` folder.
- **Ladik's MPQEditor.exe**.
- Optional: your WoW `Logs\WoWChatLog.txt` path for `.gps` loading.

AtlasForge has been tested with **Ladik's MPQEditor**. Other MPQ tools are not currently supported or recommended.

## User Data Location

AtlasForge stores settings, imported ADTs, asset caches, staged patch files, logs, backups, and generated support files under:

```text
%USERPROFILE%\Documents\AtlasForge
```

You do not need to create these folders manually. AtlasForge creates them during setup and normal use.

## Basic Workflow

1. Run `AtlasForge.exe`.
2. Complete the Setup Wizard.
3. Import ADTs and populate the asset cache.
4. Open a tile for editing:
   - Use the **ADT Map** tab to select an imported map tile directly, or
   - In WoW, go to the area you want to edit, use `/chatlog` and `.gps`, then load the latest GPS tile in AtlasForge.
5. Choose an asset from the Catalog.
6. Use the Tile Editor or WMO Editor to place, edit, copy, move, or remove objects.
7. Build the session or WMO.
8. Test the generated `patch-Z.MPQ` in-game.

## Troubleshooting

Use these built-in tools:

```text
Tools > Health & Support > Run AtlasForge Doctor
Tools > Health & Support > Create Debug Bundle
Tools > Recovery
```

If previews do not load, run Doctor and confirm the asset cache has been populated.

If packing fails:

- Close WoW.
- Close any open MPQ tools.
- Confirm **Ladik's MPQEditor.exe** is configured.
- Confirm your WoW `Data` folder is writable.
- Run Doctor again.

## Reporting Issues

When reporting a beta issue, include:

- The AtlasForge version.
- What you were trying to do.
- Whether it happened in Tile Editor, WMO Editor, setup, or packaging.
- The Doctor report.
- A Debug Bundle if possible.

Reports and debug bundles are stored under:

```text
Documents\AtlasForge\LOGS
```

## Notes

AtlasForge is an independent fan-made tool. It is not affiliated with, endorsed by, or sponsored by Blizzard Entertainment.

World of Warcraft and all related game assets, names, and trademarks are property of Blizzard Entertainment.

Users are responsible for using their own local WoW `1.12.1` game data and complying with any applicable rules, licenses, or community guidelines.
