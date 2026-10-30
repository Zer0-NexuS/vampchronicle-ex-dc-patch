```text
███████╗██╗      ██████╗
██╔════╝██║     ██╔════╝
███████╗██║     ██║  ███╗
╚════██║██║     ██║   ██║
███████║███████╗╚██████╔╝
╚══════╝╚══════╝ ╚═════╝
```
<img width="1806" height="1347" alt="image" src="https://github.com/user-attachments/assets/00ece1c2-5e2e-4859-8b5a-d9706b81b532" />

**BE ADVISED: THE PATCH TAKES 2-3 MINUTES TO COMPLETE**

HOW TO SELECT
• DEE: Highlight the ? / Random square. Press and release START once,
  then confirm with any punch or kick. Works in Arcade and dedicated Versus.
• DARK GALLON: Highlight Gallon. Press and release START, then confirm
  with any punch or kick. Press START again to return to ordinary Gallon;
  moving to another character resets the choice.

ADDITIONS INCLUDED IN THIS BUILD
1. Playable Dee, with the CPS2 character graphics/data, special/super
   controller, guard animation, teleport and sword/effect corrections.
2. Native Dee voice integration: 24 recordings and 26 command bindings.
   (Two cues remain silent).
3. English native dialogue: 326 translated messages, plus Dee’s three
   existing approved English quotes.
4. Dee’s wordless ending route: native map/VS transition and Adult Anita
   encounter.
5. EX title emblem.
6. Permanent access to EX Options and EX Editions. These expose the
   native option values and edition/stage-color choices. Some EX selections
   reset on a cold boot; the menus remain available.
7. Dark Gallon is selectable from Gallon. RC41 gives him Gallon’s winning
   themes for all character types. Alternate colors keep the approved
   Weak Punch dark fur/skin/red eyes and native alternate accent colors;
   their native pulse animation now follows the selected color.

**REMAINING KNOWN BUGS**

- CDI IS NOT HARDWARE COMPATIBLE. WORKING GDEMU IMAGE IS BEING TESTED.
- DARK GALLON MAY ADD LOAD TIME WHEN USING ALT PALETTE'S.
- DEE's FULL BLOCK ANIMATION.
- DURING DARK FORCE, DEE MAY FREE MID-AIR JUMP (LOCKS GAME).

OTHER NATIVE SHORTCUTS RETAINED
• EX Options: Options + hold L and R + A; also accessible in the expanded menu.
• Oboro Bishamon: Bishamon + hold START + attack.
• Shadow: Random + START five times + attack.
• Marionette: Random + START seven times + attack.
• Alternate stage palette: hold START when confirming the Versus stage.

##This is an unofficial, fan-made patch for Vampire Chronicle for Matching Service. I do not own the original game, its characters, artwork, music, or other original assets. All copyrights and trademarks belong to Capcom, SEGA, and their respective owners##

##This project is not affiliated with, endorsed by, or sponsored by Capcom or SEGA. The patch is provided “as is,” without warranty. Please use it with a legally obtained copy of the original game.##

**DEVELOPMENT & TOOL CREDITS**

Development tools and code used for this project:

KallistiOS (KOS) Dreamcast SDK, hardware interfaces, graphics, audio, controllers, and VMU support. GNU GCC and GNU Binutils — SH-4 toolchain Compiling, assembling, linking, and inspecting Dreamcast executables. Flycast Runtime testing, debugging, screenshots, and performance checks. NJEMU / inherited CPS2 emulator source Emulator foundation used in the experimental CPS2-to-Dreamcast work. Python Build automation, ROM preparation, graphics conversion, profiling, and packaging. FFmpeg Audio conversion and ADX decoding/preparation.

Flycast supports Dreamcast and NAOMI; chdman provides the CHD-management tools used for disc extraction. GitHub

Shared build and asset utilities

These can go in a general “Development tools” credit rather than being repeated under every system:
- Python / Python Software Foundation
- GNU Compiler Collection — GCC / G++
- GNU Binutils
- GNU Make
- CMake
- Git / MinGit
- MinGW-w64
- LLVM / lld
- Capstone
- FFmpeg
- NumPy
- SciPy
- Pillow
- Lua
- libretro
- zlib — used in documented reconstruction/delta workflows
- Our custom extraction, conversion, relocation, patching, profiling, and verification tools
Additional credits for the older Jaguar Neo Geo compatibility experiment

These belong specifically to that earlier prototype, rather than automatically to the later native rewrite:
Dependency	Contribution
Geolith	Neo Geo cartridge hardware/core implementation.
Musashi — Karl Stenerud	Motorola 68000 CPU emulation.
superzazu/z80	Z80 CPU emulation.
YMFM — Aaron Giles / YMFM-C adaptation	Yamaha sound-chip emulation.
OpenBIOS — the version retained in that project	Replacement Neo Geo BIOS source.
FinalBurn Neo	Instrumented reference traces.
Virtual Jaguar	Historical SD-test adapter work, before the later BigPEmu-only requirement.
miniz	Retained header dependency; its compression implementation wasn’t linked.
RLN	Built during SDK setup; the documented final cartridge used GNU linking.


Geolith’s upstream notices identify its incorporated CPU and sound components, which deserve their own credits when that code is included. GitHub

Still unconfirmed: Ghidra, IDA, x64dbg, Aseprite, Photoshop, Audacity, Blender, vasm, Asar, ca65, mkisofs, cdi4dc, scramble, and PyInstaller. I wouldn’t put those into an “actually used” credits list without checking the relevant source package. Likewise, I haven’t established PCSX2, PPSSPP, or a named Saturn/Sega CD emulator from the records checked.
