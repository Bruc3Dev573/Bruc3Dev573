# Bruc3Dev573

ROM hacking and MiSTer FPGA core work: translations, patches, and savestate ports.

![Game Boy Advance](https://img.shields.io/badge/Game%20Boy%20Advance-8B0000?style=flat-square)
![SNES](https://img.shields.io/badge/SNES-5A5A99?style=flat-square)
![PC Engine](https://img.shields.io/badge/PC%20Engine-1E5AA8?style=flat-square)
![MiSTer FPGA](https://img.shields.io/badge/MiSTer%20FPGA-2E7D32?style=flat-square)

## What I'm working on

Updated September 24, 2026.

1. **TurboGrafx-16 / PC Engine CD savestates**  
   [v0.2.0-pre1](https://github.com/Bruc3Dev573/TurboGrafx16_MiSTer/releases/tag/v0.2.0-pre1) is out: HuCard and CD, with SD persistence for CD slots.  
   CD needs the [companion Main](https://github.com/Bruc3Dev573/Main_MiSTer/releases/tag/tg16-savestates-v0.2.0-pre1). Reports welcome in the issues.

2. **MegaCD / Sega CD savestates**  
   Hardware testing continues in parallel.  
   **90 of 201 discs confirmed working, about 45%.**

## Translations and ROM patches

| Project | Description |
|---|---|
| [Castlevania: Aria of Sorrow, Italian Enhanced Edition](https://github.com/Bruc3Dev573/castlevania-aos-ita) | Italian translation with visual improvements and optional gameplay variants |
| [Castlevania: Harmony of Dissonance, Italian translation](https://github.com/Bruc3Dev573/castlevania-hod-ita) | Unofficial Italian translation, compatible with Visual Improvement V1.2.7 |
| [Castlevania: Symphony of the Night, JP-ITA QHack](https://github.com/Bruc3Dev573/sotn-jp-ita-qhack) | QHack v1.3 ported onto the Italian-translated Japanese Rev 2 release |
| [Final Match Tennis 2026](https://github.com/Bruc3Dev573/final-match-tennis-2026) | ATP and WTA 2026 roster patches for PC Engine |
| [Metroid Fusion, European Vanilla+](https://github.com/Bruc3Dev573/metroid-fusion-vanilla-plus) | Revised palettes, faster text, doors and elevators, and Start-to-skip introduction for the European release |

## MiSTer FPGA

| Project | Description |
|---|---|
| [GBA core](https://github.com/Bruc3Dev573/GBA_MiSTer) | Unofficial build adding an OSD freeze button |
| [SNES core, CX4 savestates](https://github.com/Bruc3Dev573/SNES_MiSTer_cx4) | CX4 coprocessor savestate support (Mega Man X2/X3) |
| [SNES core](https://github.com/Bruc3Dev573/SNES_MiSTer) | Fork of the upstream core, not actively maintained, with one build fixing an SDRAM timing issue on SuperStation One hardware |
| [TurboGrafx-16 / PC Engine CD core](https://github.com/Bruc3Dev573/TurboGrafx16_MiSTer) | Upstream fork with savestate support for HuCard, CD-ROM² and Super CD-ROM² titles. Latest: v0.2.0-pre1 |
