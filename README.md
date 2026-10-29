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

   REMAINING KNOWN BUGS:

   DARK GALLON MAY ADD LOAD TIME WHEN USING ALT PALETTE'S.
   DEE's FULL BLOCK ANIMATION.

OTHER NATIVE SHORTCUTS RETAINED
• EX Options: Options + hold L and R + A; also accessible in the expanded menu.
• Oboro Bishamon: Bishamon + hold START + attack.
• Shadow: Random + START five times + attack.
• Marionette: Random + START seven times + attack.
• Alternate stage palette: hold START when confirming the Versus stage.

##This is an unofficial, fan-made patch for Vampire Chronicle for Matching Service. I do not own the original game, its characters, artwork, music, or other original assets. All copyrights and trademarks belong to Capcom, SEGA, and their respective owners##

##This project is not affiliated with, endorsed by, or sponsored by Capcom or SEGA. The patch is provided “as is,” without warranty. Please use it with a legally obtained copy of the original game.##

**DEVELOPMENT & TOOL CREDITS**

Dreamcast — SFZ2A GOLD, SFA3 Upper, Ultra SFII
Tool / project	What we used it for
KallistiOS (KOS)	Dreamcast SDK, hardware interfaces, graphics, audio, controllers, and VMU support.
GNU GCC and GNU Binutils — SH-4 toolchain	Compiling, assembling, linking, and inspecting Dreamcast executables.
Flycast	Runtime testing, debugging, screenshots, and performance checks.
NJEMU / inherited CPS2 emulator source	Emulator foundation used in the experimental CPS2-to-Dreamcast work.
Python	Build automation, ROM preparation, graphics conversion, profiling, and packaging.
FFmpeg	Audio conversion and ADX decoding/preparation.


Official project references: KallistiOS, Flycast. GitHub

CPS1 / CPS2 / expanded CPS2 — Alpha projects, Hyper Anthology, SFZ2A GOLD, Vampire Savior, Gouki XT
Tool / project	What we used it for
MAME	Custom drivers, hardware emulation, ROM audits, debugging, tracing, captures, and performance analysis.
FinalBurn Neo (FBNeo)	Reference emulation, compatibility checks, and instrumented CPU/video/audio tracing.
MAME 2010 libretro core	Earlier combat, character-selection, and regression testing, including SFZ2A GOLD.
MAME Lua scripting	Automated inputs, memory observation, execution probes, and repeatable tests.
chdman — MAME tools	Extracting and inspecting CHD donor discs.
GNU GCC / G++ and Binutils	Emulator builds and native 68000 assembly/build work.
MinGW-w64	Building Windows executables.
LLVM lld	Linking particular Windows MAME builds.
GENie	Generating MAME build projects.
GNU Make	Building emulators and supporting tools.
Python	ROM reconstruction, relocation, graphics/audio conversion, patch generation, and audits.
NumPy / SciPy	Numerical checks and captured-audio analysis.


FinalBurn Neo; chdman belongs to the MAME project. We are Team FBNeo. · GitHub

Neo Geo MVS / AES / CD — SFII CE, Rainbow, Hyper Fighting / NEO SF2HE
Tool / project	What we used it for
MAME	Neo Geo cartridge testing, hardware behavior checks, debugging, and captures.
FinalBurn Neo	Reference behavior and instrumented Neo Geo tracing.
chdman	Neo Geo CD data-track extraction and independent extraction verification.
Capstone	68000 disassembly and binary analysis in the cartridge-conversion tools.
GNU m68k Binutils	Assembling, linking, and inspecting native 68000 code.
Lua — through MAME	Input automation, CPU history, and read-only state tracing.
Python	CD resource extraction, code relocation, graphics packing, tile mapping, and ROM generation.


Capstone’s official name is Capstone Disassembly Framework. The Ultimate Disassembler

Atari Jaguar — Samurai Shodown and Fight for Life REMIXED
Tool / project	What we used it for
BigPEmu — Rich Whitehouse	Jaguar runtime testing, debugging, captures, and performance checks.
Jaguar SDK — cubanismo/jaguar-sdk	Build environment, startup code, hardware definitions, samples, and supporting tools.
RMAC	Jaguar GPU/DSP and 68000 assembly.
GNU m68k GCC and Binutils	Compiling, linking, and inspecting Jaguar target code.
JagCrypt / pc_jagcrypt	Preparing signed Jaguar cartridge images.
RetroHQ Jaguar GameDrive BIOS API / bindings	GameDrive file access and cartridge integration where applicable.
Python	Asset conversion, compression, ROM construction, verification, and packaging.
GNU Make	SDK and tool builds.


Those SDK/compiler entries are explicitly documented in the Samurai Shodown records; they shouldn’t automatically be attributed to every Fight for Life revision. Official references: Jaguar SDK, pc_jagcrypt, BigPEmu. GitHub

SNES / Super FX 2 — Samurai Shodown zoom work
Tool / project	What we used it for
Snes9x	SNES and Super FX runtime testing and debugging.
libretro API / Snes9x libretro core	Scripted execution, inputs, captures, and inspection.
Python	ROM patching, renderer generation, asset extraction, and verification.
NumPy	Pixel, tile, and numerical processing.
Pillow	Image conversion, scaling, palette handling, and comparison images.
GNU Make / host compiler tools	Building the retained emulator sources.


The saved Super FX checkpoint identifies a specific Snes9x nightly, so credit Snes9x without treating every official release as equivalent. Official Snes9x repository. GitHub

NAOMI / donor-platform extraction — Upper, PS2 Anthology, Saturn material
System / work	Tools confirmed in the records
NAOMI / SFA3 Upper	Flycast, chdman, Python, custom SH-4 tracing/patching and resource tools.
PS2 Alpha Anthology extraction	chdman, Python, FFmpeg, custom ISO9660/AFS/PZZ/MOMO extraction tools.
PZZ format research	infval’s pzzcompressor_jojo — documented as a related-format reference.
Saturn Gold title/resource recovery	Custom extraction/decompression and graphics-conversion tools; a named Saturn emulator wasn’t established by the records checked.


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
