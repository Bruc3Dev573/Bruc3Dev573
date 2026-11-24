# Bruc3Dev573

ROM hacking and MiSTer FPGA core work: translations, patches, and savestate ports.

![Game Boy Advance](https://img.shields.io/badge/Game%20Boy%20Advance-8B0000?style=flat-square)
![SNES](https://img.shields.io/badge/SNES-5A5A99?style=flat-square)
![PC Engine](https://img.shields.io/badge/PC%20Engine-1E5AA8?style=flat-square)
![Mega CD](https://img.shields.io/badge/Mega%20CD-37474F?style=flat-square)
![32X](https://img.shields.io/badge/32X-B71C1C?style=flat-square)
![Commodore 64](https://img.shields.io/badge/Commodore%2064-6C5EB5?style=flat-square)
![MiSTer FPGA](https://img.shields.io/badge/MiSTer%20FPGA-2E7D32?style=flat-square)

## How I work

I use AI tools throughout my work: RTL, tools, debugging and my English.
Changes go through several rounds of review and testing in private repos before they're published,
and each release says what was tested and on what hardware.
I'm responsible for what I publish: report problems in my repos, not to the original core authors.
Feedback on the code is welcome, and I'll rework it if needed to go upstream. If a question goes
beyond what I know, I'll say so and look into it.

## MiSTer FPGA

### Savestate cores

| Core | What it adds | Release notes | Download | Main download | Status |
|---|---|---|---|---|---|
| [TurboGrafx16 / PC Engine](https://github.com/Bruc3Dev573/TurboGrafx16_MiSTer) | Savestates for HuCard, SuperGrafx and CD games | [v1.0.2](https://github.com/Bruc3Dev573/TurboGrafx16_MiSTer/releases/tag/v1.0.2) | [RBF](https://github.com/Bruc3Dev573/TurboGrafx16_MiSTer/releases/download/v1.0.2/TurboGrafx16_SS_20261124.rbf) | [Disc images](https://github.com/Bruc3Dev573/Main_MiSTer/releases/download/20261010-pcecd-savestates/MiSTer) · [Physical drive](https://github.com/Bruc3Dev573/Main_MiSTer_Physical_Disc/releases/download/v2.10.0-pcecd-savestates/MiSTer_Physical-CD) | Stable. Main needed only for CD games |
| [MegaCD / Sega CD](https://github.com/Bruc3Dev573/MegaCD_MiSTer) | Savestates | [v0.1.1](https://github.com/Bruc3Dev573/MegaCD_MiSTer/releases/tag/v0.1.1) | [RBF](https://github.com/Bruc3Dev573/MegaCD_MiSTer/releases/download/v0.1.1/MegaCD_SS_20261105.rbf) | [Disc images](https://github.com/Bruc3Dev573/Main_MiSTer/releases/download/20261010-megacd-savestates-r9/MiSTer) · [Physical drive](https://github.com/Bruc3Dev573/Main_MiSTer_Physical_Disc/releases/download/v2.10.0-megacd-savestates-r10/MiSTer_Physical-CD) | Stable |
| [Sega 32X](https://github.com/Bruc3Dev573/S32X_MiSTer) | Savestates for 32X and Mega Drive games, Virtua Racing with its SVP chip, Pier Solar | [v0.1.0-pre4](https://github.com/Bruc3Dev573/S32X_MiSTer/releases/tag/v0.1.0-pre4) | [RBF](https://github.com/Bruc3Dev573/S32X_MiSTer/releases/download/v0.1.0-pre4/S32X_SS_20261120.rbf) | Official | Test build. Works with the official Main |
| [Commodore 64](https://github.com/Bruc3Dev573/C64_MiSTer) | Savestates of the whole machine, also during disk and tape loads: 1541 and 1581 drives, datassette, cartridges with EasyFlash, REU up to 16 MB, GeoRAM, Sound Expander | [v0.1.0-pre2](https://github.com/Bruc3Dev573/C64_MiSTer/releases/tag/v0.1.0-pre2) | [RBF](https://github.com/Bruc3Dev573/C64_MiSTer/releases/download/v0.1.0-pre2/C64_SS_20261119.rbf) | [SD slots](https://github.com/Bruc3Dev573/Main_MiSTer/releases/download/20261010-c64-savestates-r2/MiSTer) | Test build. Official Main supports in-memory slots |

Install steps for these cores, and the modified Main that TurboGrafx16, MegaCD and C64 need, are on [MiSTer-savestates](https://github.com/Bruc3Dev573/MiSTer-savestates). Reports are welcome in the issues of each core's repository.

### Other builds

| Core | What it adds | Release notes | Download | Main download | Status |
|---|---|---|---|---|---|
| [SNES for SuperStation One](https://github.com/Bruc3Dev573/SNES_MiSTer) | Fix for savestates that get corrupted on some SuperStation One boards ([#505](https://github.com/MiSTer-devel/SNES_MiSTer/issues/505)) | [snes_ss_fwdual_15082026](https://github.com/Bruc3Dev573/SNES_MiSTer/releases/tag/snes_ss_fwdual_15082026) | [RBF](https://github.com/Bruc3Dev573/SNES_MiSTer/releases/download/snes_ss_fwdual_15082026/SNES_ss_fwdual_20260815.rbf) | — | Fixed upstream in [PR #525](https://github.com/MiSTer-devel/SNES_MiSTer/pull/525), merged on 5 November 2026, coming in the next official release. Until then this workaround still works |
| [GBA with Pause](https://github.com/Bruc3Dev573/GBA_MiSTer/tree/pause) | Mappable Pause button that stops picture and sound; fast forward stays off while paused | [pause-20261120](https://github.com/Bruc3Dev573/GBA_MiSTer/releases/tag/pause-20261120) | [RBF](https://github.com/Bruc3Dev573/GBA_MiSTer/releases/download/pause-20261120/GBA_pause_20261120.rbf) | — | One-off build on the official core of 22 July 2026, not kept up to date |
| [SNES with Pause](https://github.com/Bruc3Dev573/SNES_MiSTer/tree/pause) | Mappable Pause button; HDMI keeps the last frame while paused | [pause-20261115](https://github.com/Bruc3Dev573/SNES_MiSTer/releases/tag/pause-20261115) | [RBF](https://github.com/Bruc3Dev573/SNES_MiSTer/releases/download/pause-20261115/SNES_pause_20261115.rbf) | — | One-off build on the official core of 5 November 2026, not kept up to date |
| [MegaCD with Pause](https://github.com/Bruc3Dev573/MegaCD_MiSTer/tree/pause) | Savestates v0.1.1 plus a mappable Pause button that stops picture, sound and CD drive | [v0.1.1-pause](https://github.com/Bruc3Dev573/MegaCD_MiSTer/releases/tag/v0.1.1-pause) | [RBF](https://github.com/Bruc3Dev573/MegaCD_MiSTer/releases/download/v0.1.1-pause/MegaCD_SS_pause_20261116.rbf) | [Disc images](https://github.com/Bruc3Dev573/Main_MiSTer/releases/download/20261010-megacd-savestates-r9/MiSTer) · [Physical drive](https://github.com/Bruc3Dev573/Main_MiSTer_Physical_Disc/releases/download/v2.10.0-megacd-savestates-r10/MiSTer_Physical-CD) | One-off build based on v0.1.1 |
| [32X with Pause](https://github.com/Bruc3Dev573/S32X_MiSTer/tree/pause) | Savestates v0.1.0-pre4 plus a mappable Pause button (also the keyboard Pause key) that stops everything, Virtua Racing included | [v0.1.0-pre4-pause](https://github.com/Bruc3Dev573/S32X_MiSTer/releases/tag/v0.1.0-pre4-pause) | [RBF](https://github.com/Bruc3Dev573/S32X_MiSTer/releases/download/v0.1.0-pre4-pause/S32X_SS_pause_20261120.rbf) | Official | One-off build; the regular one is v0.1.0-pre4 |
| [TurboGrafx16 with Pause](https://github.com/Bruc3Dev573/TurboGrafx16_MiSTer/tree/pause) | Savestates v0.2.0-pre2 plus a mappable Pause button that also stops CD music | [v0.2.0-pre2-pause](https://github.com/Bruc3Dev573/TurboGrafx16_MiSTer/releases/tag/v0.2.0-pre2-pause) | [RBF](https://github.com/Bruc3Dev573/TurboGrafx16_MiSTer/releases/download/v0.2.0-pre2-pause/TurboGrafx16_SS_pause_20261116.rbf) | [Disc images](https://github.com/Bruc3Dev573/Main_MiSTer/releases/download/20261010-pcecd-savestates/MiSTer) · [Physical drive](https://github.com/Bruc3Dev573/Main_MiSTer_Physical_Disc/releases/download/v2.10.0-pcecd-savestates/MiSTer_Physical-CD) | Older test build. Main needed only for CD games. [Current core without Pause](#savestate-cores) |
| [C64 with Pause](https://github.com/Bruc3Dev573/C64_MiSTer/tree/pause) | Savestates v0.1.0-pre2 plus a mappable Pause button (also the keyboard Pause/Break key) that stops the machine, drives and tape included | [v0.1.0-pre2-pause](https://github.com/Bruc3Dev573/C64_MiSTer/releases/tag/v0.1.0-pre2-pause) | [RBF](https://github.com/Bruc3Dev573/C64_MiSTer/releases/download/v0.1.0-pre2-pause/C64_SS_pause_20261119.rbf) | [SD slots](https://github.com/Bruc3Dev573/Main_MiSTer/releases/download/20261010-c64-savestates-r2/MiSTer) | One-off build based on v0.1.0-pre2 |

### Merged upstream

- [SNES](https://github.com/MiSTer-devel/SNES_MiSTer): savestates for CX4 games (Mega Man X2 and X3), merged in [PR #487](https://github.com/MiSTer-devel/SNES_MiSTer/pull/487), part of the official core since release 20260823.

## Translations and ROM patches

| Project | Description |
|---|---|
| [Castlevania: Aria of Sorrow, Italian Enhanced Edition](https://github.com/Bruc3Dev573/castlevania-aos-ita) | Italian translation with visual improvements and optional gameplay variants |
| [Castlevania: Harmony of Dissonance, Italian translation](https://github.com/Bruc3Dev573/castlevania-hod-ita) | Unofficial Italian translation, compatible with Visual Improvement V1.2.7 |
| [Castlevania: Symphony of the Night, JP-ITA QHack](https://github.com/Bruc3Dev573/sotn-jp-ita-qhack) | QHack v1.3 ported onto the Italian-translated Japanese Rev 2 release |
| [Final Match Tennis 2026](https://github.com/Bruc3Dev573/final-match-tennis-2026) | ATP and WTA 2026 roster patches for PC Engine |
| [Metroid Fusion, European Vanilla+](https://github.com/Bruc3Dev573/metroid-fusion-vanilla-plus) | Revised palettes, faster text, doors and elevators, and Start-to-skip introduction for the European release |
