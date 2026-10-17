# Bruc3Dev573

ROM hacking and MiSTer FPGA core work: translations, patches, and savestate ports.

![Game Boy Advance](https://img.shields.io/badge/Game%20Boy%20Advance-8B0000?style=flat-square)
![SNES](https://img.shields.io/badge/SNES-5A5A99?style=flat-square)
![PC Engine](https://img.shields.io/badge/PC%20Engine-1E5AA8?style=flat-square)
![Mega CD](https://img.shields.io/badge/Mega%20CD-37474F?style=flat-square)
![MiSTer FPGA](https://img.shields.io/badge/MiSTer%20FPGA-2E7D32?style=flat-square)

## MiSTer FPGA

| Core | What it adds | Download | Status |
|---|---|---|---|
| [TurboGrafx16 / PC Engine](https://github.com/Bruc3Dev573/TurboGrafx16_MiSTer) | Savestates for HuCard, SuperGrafx and CD games | [v0.2.0-pre2](https://github.com/Bruc3Dev573/TurboGrafx16_MiSTer/releases/tag/v0.2.0-pre2) | Test build. CD games also need the modified Main |
| [MegaCD / Sega CD](https://github.com/Bruc3Dev573/MegaCD_MiSTer) | Savestates | [v0.1.0-pre5](https://github.com/Bruc3Dev573/MegaCD_MiSTer/releases/tag/v0.1.0-pre5) | Test build. Needs the modified Main |
| [SNES](https://github.com/MiSTer-devel/SNES_MiSTer) | Savestates for CX4 games, Mega Man X2 and X3 | Official core | Merged in [PR #487](https://github.com/MiSTer-devel/SNES_MiSTer/pull/487), part of the official core since release 20260823 |
| [SNES for SuperStation One](https://github.com/Bruc3Dev573/SNES_MiSTer) | Fix for savestates that get corrupted on some SuperStation One boards ([#505](https://github.com/MiSTer-devel/SNES_MiSTer/issues/505)) | [snes_ss_fwdual_15082026](https://github.com/Bruc3Dev573/SNES_MiSTer/releases/tag/snes_ss_fwdual_15082026) | Only for affected boards. Based on the official core of 4 August 2026 |
| [GBA](https://github.com/Bruc3Dev573/GBA_MiSTer) | OSD freeze button | [pause-hotkey-20260831](https://github.com/Bruc3Dev573/GBA_MiSTer/releases/tag/pause-hotkey-20260831) | Unofficial build. Hardware testing is limited |

Install steps for the TurboGrafx16 and MegaCD cores and the modified Main they need are on [MiSTer-savestates](https://github.com/Bruc3Dev573/MiSTer-savestates). Reports for those two cores are welcome in the issues of their repositories.

## Translations and ROM patches

| Project | Description |
|---|---|
| [Castlevania: Aria of Sorrow, Italian Enhanced Edition](https://github.com/Bruc3Dev573/castlevania-aos-ita) | Italian translation with visual improvements and optional gameplay variants |
| [Castlevania: Harmony of Dissonance, Italian translation](https://github.com/Bruc3Dev573/castlevania-hod-ita) | Unofficial Italian translation, compatible with Visual Improvement V1.2.7 |
| [Castlevania: Symphony of the Night, JP-ITA QHack](https://github.com/Bruc3Dev573/sotn-jp-ita-qhack) | QHack v1.3 ported onto the Italian-translated Japanese Rev 2 release |
| [Final Match Tennis 2026](https://github.com/Bruc3Dev573/final-match-tennis-2026) | ATP and WTA 2026 roster patches for PC Engine |
| [Metroid Fusion, European Vanilla+](https://github.com/Bruc3Dev573/metroid-fusion-vanilla-plus) | Revised palettes, faster text, doors and elevators, and Start-to-skip introduction for the European release |
