# Awesome N64 Development

A curated list of Nintendo 64 development resources including toolchains, documentation, emulators, example code, and more!

## Contents

* [Documentation](#documentation)
* [Emulators](#emulators)
* [Reverse Engineering](#reverse-engineering)

## Documentation

* [Ultra64](https://ultra64.ca/) - An absolute wealth of documentation including official development manuals, as well as SDK downloads and reference material
* [Nintendo 64 Architecture](https://copetti.org/projects/consoles/nintendo-64/) - An overview of the console architecture
* [N64brew Wiki](https://n64brew.dev/) - The N64brew community wiki
* [N64dev](http://n64dev.org/) - Useful N64 hacking links
* [Console Protocols](https://sites.google.com/site/consoleprotocols/home) - Nintendo 64 hardware info, memory map, PIF boot stage reference, and JoyBus I/O documentation
* [N64 ROM Formats](http://n64dev.org/romformats.html) - A short N64 ROM format quick reference sheet
* [N64 ROM Formats Explained](https://www.reddit.com/r/emulation/comments/7hrvzp/the_three_different_n64_rom_formats_explained_for/?st=jn9t30t4&sh=1951de19) - Details the three commonly encountered Nintendo 64 ROM formats (use Big Endian/.z64)
* [Accessory Reference](http://github.com/joeldipops/TransferBoy/blob/master/docs/TransferPakReference.md) - Guide on how to communicate with the Transfer Pak and Rumble Pak
* [Hack64](https://hack64.net/wiki/doku.php?id=nintendo_64) - A variety of documentation on RCP data structures, compression, assembly, and more
* [64dd.org](https://64dd.org) - Nintendo 64DD documentation, emulators, homebrew, and tools
* [64DD wiki](https://github.com/LuigiBlood/64dd/wiki) - Documentation on 64DD hardware, disks, and related cartridges

## Videos

* [Installing the Nintendo 64 Development Kit](https://www.youtube.com/watch?v=84wk0mZ8gfM) - How to install the Nintendo 64 Software Development Kit under Windows 2000 and 98SE and build sample code. Also generally works under Windows XP.
* [Behind The Code](https://www.youtube.com/c/BehindTheCode001/videos) - Gerry O'Brien's YouTube channel, with a number of videos discussing Nintendo 64 development with NuSystem and the official SDK, development hardware, audio processing, and more
* [Building cen64 for Speed and Preservation](https://www.youtube.com/watch?v=lvr6-6U0ck8) - Tyler Stachecki and Mike Ryan discuss making the cen64 emulator fast without compromising on accuracy
* [REcon 2015 - Reversing the Nintendo 64 CIC](https://www.youtube.com/watch?v=HwEdqAb2l50) - Mike Ryan, Marshall Hecht, and John McMaster talk about reverse engineering and cloning a 20 year old copy protection chip (the N64 CIC)
* [Programming for Nintendo 64](https://www.youtube.com/watch?v=aKXEooIPwP0) - Damjan Nesic goes through the basics of programming for Nintendo 64 using C and a Windows XP virtual machine

## Toolchains

* [Official Nintendo 64 SDKs](https://ultra64.ca/resources/software/) - Official Nintendo 64 Software Development Kits for Windows and SGI IRIX
* [n64sdkmod](https://github.com/CrashOveride95/n64sdkmod) - A `libultra` SDK for the modern era, supported on Debian-based Linux distros
* [N64 SDK Easy Install CD](https://mega.nz/#!AOYDkSxA!MuAqt8iRBk0GGbaqaXVYB9tfZxsquKg5QkbCRL3VOLM) - An ISO image made by AlphaTango and CrashOveride to simplify installation of the official SDK. Works on Windows 98-XP.
* [n64chain](https://github.com/tj90241/n64chain) - A development toolchain based on GCC that does not depend on any proprietary Nintendo library
* [modern-n64sdk](https://github.com/trhodeos/modern-n64sdk) - Describes how to get a modern build of GCC cross-compiling on a modern OS (Linux, Windows, macOS)
* [portable-n64-toolchain](https://github.com/Mr-Pnut/portable-n64-toolchain) - A Dockerized toolchain based on modern-n64sdk
* [mips64-gcc-toolchain](https://github.com/N64-tools/mips64-gcc-toolchain) - Windows and Linux scripts to automate building of a modern MIPS64 GCC toolchain for Nintendo 64 cross compilation
* [glankk/n64](https://github.com/glankk/n64) - A collection of files and tools used to compile and test code for the Nintendo 64
* [n64devkit-everdrive](https://github.com/werkn/n64devkit-everdrive) - A development environment for containerized homebrew development using the EverDrive 64 X7 and `libdragon`

## Assemblers

* [ARM9/bass](https://github.com/ARM9/bass) - A fork which has been updated with Nintendo 64 MIPS/RSP/RDP output
* [Screwaround64](https://github.com/superjack111/screwaround64) - An interactive assembler for Nintendo 64
* [lips](https://github.com/notwa/lips) - A MIPS R4300i assembler written in Lua
* [naken_asm](https://github.com/mikeakohn/naken_asm) - An assembler for a variety of CPUs including standard MIPS III (Nintendo 64 CPU) and RSP

## Emulators

### Actively Maintained

* [Project64](https://www.pj64-emu.com) ([GitHub](https://github.com/project64/project64)) - An open-source emulator for Windows and (soonTM) Linux/Android.
* [mupen64plus](https://mupen64plus.org) ([GitHub](https://github.com/mupen64plus)) - A more recently updated fork of Mupen64 for Linux, Mac OSX, FreeBSD, and Windows. No GUI is included, so you can use simple64, RMG, or the RetroArch core for a UI.
* [simple64](https://simple64.github.io/) ([GitHub](https://github.com/simple64/simple64)) - A fork of Mupen64Plus that is easy to use and also more accurate.
* [Mupen64+ Reverser Edition](https://www.retroreversing.com/mupen64RE) - A fork of the Mupen64Plus emulator tailored for reverse engineering.
* [Rosalie's Mupen GUI](https://github.com/Rosalie241/RMG) - a GUI for Mupen64Plus that works on Windows. One of the easiest and best ways to use Mupen64Plus with a GUI!
* [ModLoader64](https://modloader64.com) ([GitHub](https://github.com/hylian-modding/ModLoader64)) - A wrapper for Mupen64plus that enables modding through plugins written in TypeScript
* [ares](https://ares-emu.net) - A low-level, accurate multi-system emulator with good support for N64. Available in sources and binary distributions for Windows, Mac and Linux. It includes a CPU and RSP recompiler, and emulates RDP with Vulkan (via Parallel-RDP).
* [Dillonb's dgb-n64](https://github.com/Dillonb/n64) - A low-level, accurate N64 emulator for Windows and Linux. It includes a CPU recompiler, and emulates RDP with Vulkan (via parallel-RDP).

### Works In Progress

* [Kaizen (previously Gadolinium)](https://github.com/SimoneN64/Kaizen) - Work-in-progress emulator written in C++, able to already play some commercial games and replay Mupen TAS movies
* [Gopher64](https://github.com/gopher64/gopher64) - An N64 emulator written in Rust by the developer of Simple64, able to already play some commercial games at decent speeds!

### Unmaintained

* [UltraHLE](https://en.wikipedia.org/wiki/UltraHLE) - An early emulator for Windows. Though closed-source, [the source leaked in 2002](https://web.archive.org/web/20020812020546/http://www.emulation64.com/freeflow-page.html).
* [Not64](https://github.com/extremscorner/not64) - A fork of Wii64
* [cen64](https://github.com/n64dev/cen64) - A [cycle-accurate](https://retrocomputing.stackexchange.com/questions/1191/what-exactly-is-a-cycle-accurate-emulator) An emulator for Windows, Linux, and Mac. While currently not fast enough to play games at full speed, it aims for perfect emulation by emulating the hardware inside of the console down to the register-transfer level. Widely used to test ROMs in lieu of or before using real hardware.

## Development Hardware

* [64drive](http://64drive.retroactive.be/) - A flash cartridge with USB support targeted at developers. Currently near impossible to get new, or expensive second hand.
* [EverDrive 64 X7](https://krikzz.com/store/home/55-everdrive-64-x7.html) - A flash cartridge with USB support for development
* [Brutzelkarte](https://github.com/jago85/Brutzelkarte_PCB) - An open-source (hardware and software) FPGA-based flash cartridge
* [UltraHDMI](http://ultrahdmi.retroactive.be/) (periodically in stock at [Game-Tech](https://www.game-tech.us/product/ultrahdmi/)) - A board that can be installed into the console to capture the digital output of the RCP and send it out a Mini HDMI connector to a modern TV. Convenient for connecting a real console to a nearby monitor while viewing the best possible output signal.
* [N64RGB](https://etim.net.au/shop/shop.php?crn=209&rn=548&action=show_detail) - An N64RGB mod that supports every motherboard revision and works pretty well.
* [UltraSave](http://64drive.retroactive.be/features.php#ultrasave) - A device that works with the 64drive to transfer saves from real cartridges
* [GameShark 3.0+](https://hackaday.com/2019/01/11/nintendo-64-homebrew-via-game-shark/) - A method of running homebrew via a GameShark
* [sm64gameshark](https://sites.google.com/site/sm64gameshark/resources/transfering-codes-over-usb) - How to transfer GameShark codes from USB to parallel, and how to identify GameShark cartridges with functional parallel ports
* [gs_libusb](https://github.com/hcs64/gs_libusb) - GameShark Pro utilities using libusb over a USB parallel port adapter
* [ED64 Plus](https://ed64p.com/) - A Chinese clone of the Everdrive 64 at a much cheaper price point. It also has a disconnected USB port with a missing FT245R chip that [can be reattached](https://odysee.com/@backofficeshow:f/everdrive-ed64-nintendo-64-teardown:0) for theoretical added functionality.

## Tools and Libraries

### Development Cartridge Loaders

* [g64drive](https://github.com/rasky/g64drive) - Linux/Mac tool for operating a 64drive development cartridge
* [ed64](https://github.com/anacierdem/ed64) - Tools to develop on an EverDrive 64 cartridge
* [loader64](https://github.com/jsdf/loader64) - A USB uploader for EverDrive 64
* [UNFLoader](https://github.com/buu342/N64-UNFLoader/) - A universal flash cart ROM uploader (64drive, EverDrive 64 V3, EverDrive 64 X7 and SummerCart64) and debug library

### Flashcart menu software

* [N64FlashcartMenu](https://github.com/Polprzewodnikowy/N64FlashcartMenu) - Universal flashcart menu with aim to support most of the N64 flashcarts on the market

### Asset Conversion and Viewing

#### 3D

* [64Drive Viewer](https://www.youtube.com/watch?v=yUX1Vga6amg) - Preview textures, images, sounds, and 3D models on hardware with a 64drive over USB
* [Blen64](https://github.com/GCaldL/Blen64) - Blender scripts to export meshes to draw lists as header files
* [Blender64](https://github.com/engerb/Blender64) - A Python tool to export Blender 3D models to F3DEX2 microcode display lists
* [blend2niff](https://github.com/1r3n33/blend2niff) - A Blender add-on to export to [NIFF2](http://n64devkit.square7.ch/niff/index.htm) (Nintendo Intermediate File Format 2)
* [Sausage64](https://github.com/buu342/Blender-Sausage64) - A Blender plugin to export "sausage link" style character models with animations
* [Fast64](https://github.com/Fast-64/fast64) - A Blender plugin to preview and export meshes as F3D display lists for decomp and homebrew projects.
* [objn64](https://github.com/n64dev/objn64) - Wavefront `.obj` model converter that generates optimized displaylists for compilation with `libultra`
* [Obj2N64DL](https://github.com/pseudophpt/Obj2N64DL) - Another Wavefront `.obj` to displaylist converter
* [Max_To_N64](https://github.com/MrQuetch/Max_To_N64) - Scripts to export models from 3DS Max to C
* [N64_3DRenderingTest](https://github.com/tfcat/N64_3DRenderingTest) - A basic model viewer using NuSystem

#### 2D

* [n64texconv](https://github.com/coleferg/n64texconv) - A Python tool to convert PNG to RGBA(16/32), CI(4/8), and I(A)(4/8)
* [png2n64](https://github.com/matthieularere/png2n64) - A Python 3 script to convert PNG images to 16 bit RBGA
* [png2c](https://github.com/selfVSmind/png2c) - A C++ command line tool to convert PNG images to `libultra`-compatible texture header files
* [GML-N64TextureConverter](https://github.com/buu342/GML-N64TextureConverter) - Converts standard image formats to Nintendo 64 compatible C header files
* [n64CIconverter](https://github.com/darklink623/n64CIconverter) - Converts standard image formats to Nintendo 64's [Color Index (CI) format](https://n64squid.com/homebrew/n64-sdk/textures/image-formats/#CI)
* [N64GFXCookie](https://github.com/LuigiBlood/N64GFXCookie) - Nintendo 64 CI8 format graphics viewer/editor
* [n64rawgfx](https://github.com/Octocontrabass/n64rawgfx) - A tool to export and import uncompressed/raw graphics from ROMs
* [Texture64](https://github.com/queueRAM/Texture64) - A texture ripper and editor with support for multiple formats
* [ImageMerge](https://github.com/TheRDavid/ImageMerge) - Converts two 8-bit images into 2-bit images and packs them into 1 image to save space in a ROM
* [Spritemapper](https://github.com/TheRDavid/Spritemapper) - Arranges a directory of equally-sized images into a sprite map and compresses it
* [xo-tt64](https://github.com/xoorath/xo-tt64) - Converts input images to .c files of the same name
* [mkspriten64](https://github.com/nathanduma/mkspriten64) - Windows equivalent to the SGI program `mksprite`. Converts .png to a .h header and .c source file.
* [mksprite2](https://github.com/farisawan-2000/mksprite2) - A Python 3 script to create sprite and background objects for use with S2DEX microcode

### Audio Playback and Editing

* [N64-Tools](https://github.com/jombo23/N64-Tools/tree/master/N64%20Midi%20Tool) - A tool to extract and import audio from many games that make use of the MIDI format
* [libmad-n64](https://github.com/parasyte/libmad-n64) - [libmad](https://www.underbit.com/products/mad/) with MIPS patches, for MPEG audio playback
* [seq64](https://github.com/sauraen/seq64) - A full-featured editor for sequenced music in first-party games
* [N64-SoundTester](https://github.com/buu342/N64-SoundTester) - A ROM that allows you to test out N64 Sound Tools sample banks and tune them directly on your console or emulator, avoiding lengthy turnaround times
* [ultra_mpeg](https://github.com/devwizard64/ultra_mpeg/) - An MPEG-1/2 decoder library
* [ANMP](https://github.com/derselbst/ANMP) - A multi-channel loopable video game music player, with support for various Nintendo 64 audio formats
* [midicvt](https://github.com/lambertjamesd/midicvt) - An open source replacement for `midicvt` to create MIDI files compatible with `libultra`
* [sfz2n64](https://github.com/lambertjamesd/sfz2n64) - Converts SFZ files to a format the Nintendo 64 can use as part of instrument banks

### Debugging

* [Project64 EmuScripts](https://github.com/LuigiBlood/EmuScripts/tree/master/N64/Project64) - Scripts for debugging under Project64 emulation
* [n64rd](https://github.com/parasyte/n64rd) - Remote debugger for GameShark 3.2 hardware over a parallel interface
* [webserial-ed64log](https://github.com/jsdf/webserial-ed64log) - An ed64log client using Web Serial API
* [ed64-gdb](https://github.com/networkfusion/ed64-gdb) - A GDB stub for debugging with an EverDrive 64 V3
* [gdbstub-ed64](https://github.com/murachue/gdbstub-ed64) - Another EverDrive 64 GDB stub
* [N64-GDB-stub](https://github.com/Hazematman/N64-GDB-stub) - A GDB stub that works with a modified version of the cen64 emulator

### ROM Manipulation

* [spicy](https://github.com/trhodeos/spicy) - An open-source replacement of the official SDK's `mild.exe` (referenced by `$(MAKEROM)` in many Makefiles). Packs object files into an N64-compatible ROM.
* [makeromOpen](https://github.com/fraser125/makeromOpen) - Another open-source makerom replacement (work in progress)
* [makemask](https://github.com/trhodeos/makemask) - An open-source replacement of the official SDK's `makemask.exe`. Adds a mask to a compiled ROM which pads the file to fill the entire cartridge space, adds a CIC version, and adds informational headers to the file. Typically run immediately after `mild.exe`. More on this tool at [N64Squid](https://n64squid.com/homebrew/n64-sdk/software/mipse-ultra-gcc/makemask/).
* [Tool N64](https://www.zophar.net/utilities/n64aud/tool-n64.html) - A tool to display ROM information and perform byte reordering
* [Real N64 CRC Tool v2](https://www.smwcentral.net/?p=section&a=details&id=8799) - A tool to check, calculate, and set ROM checksums and extract the bootcode of ROM files
* [rom64](https://github.com/mroach/rom64) - A tool to identify and parse ROM header information
* [romjudge](https://github.com/jkbenaim/romjudge) - A utility to judge an N64 ROM for correctness
* [leotools](https://github.com/jkbenaim/leotools) - Work with 64DD disk images and the files contained therein
* [n64splat](https://github.com/ethteck/n64splat) - A ROM splitting tool to assist with decompilation and modding projects
* [seq64/n64checksum](https://github.com/sauraen/seq64/blob/master/Source/n64checksum.cpp) - Source for a tool to calculate and set ROM checksums
* [Info64](https://www.smwcentral.net/?p=section&a=details&id=5737) - A tool to display and set ROM header information and checksums
* [N64ShellPreview](https://github.com/Random06457/N64ShellPreview) - A Windows Shell Extension to display ROM information in Explorer's preview pane
* [ipl3hasher](https://github.com/awygle/ipl3hasher) - GPU-accelerated hash collision finder for the IPL3 boot code

### Development Libraries

* [libdragon](https://github.com/DragonMinded/libdragon) - An open-source library for Nintendo 64 development
* [libn64](https://github.com/tj90241/n64chain/tree/master/libn64) - An open-source library for Nintendo 64 development, part of `n64chain`
* [pseultra](https://github.com/pseudophpt/pseultra) - A collection of tools used to develop software for the Nintendo 64 that are distinct from the official SDK
* [libreultra](https://github.com/n64decomp/libreultra) - A decompilation of the Nintendo 64 standard SDK library, `libultra`
* [ultralib](https://github.com/decompals/ultralib) - A reverse engineering of `libultra`
* [framework64](https://github.com/matthewcpp/framework64) - An asset pipeline and C library to simplify game creation (uses n64sdkmod)
* [n64ut](https://github.com/n64ut) - An in-progress set of modern Nintendo 64 libraries
* [libhfx](https://github.com/Hazematman/libhfx) - An in-progress open source library for 3D graphics
* [S2DEX Text Engine](https://github.com/someone2639/S2DEX-Text-Engine) - A text engine powered by the S2DEX microcode

## Reverse Engineering

### Projects

#### Game Decompilation

* [AeroGauge](https://github.com/LLONSIT/AeroGauge) - An in-progress decompilation of _AeroGauge_
* [Banjo-Kazooie](https://gitlab.com/banjo.decomp/banjo-kazooie) - An in-progress decompilation of _Banjo-Kazooie_
* [Banjo-Tooie](https://github.com/mr-wiseguy/banjo-tooie) - An in-progress decompilation of _Banjo-Tooie_
* [Blast Corps](https://gitlab.com/retroplastic/blastcorps) - An in-progress decompilation of _Blast Corps_
* [Bomberman 64](https://github.com/bomberhackers/bm64) - An in-progress decompilation of _Bomberman 64_
* [Bomberman Hero](https://github.com/bomberhackers/bmhero) - An in-progress decompilation of _Bomberman Hero_
* [Castlevania 64](https://github.com/blazkowolf/cv64) - An in-progress decompilation of _Castlevania 64_
* [Conker's Bad Fur Day](https://github.com/mkst/conker) - An in-progress decompilation of _Conker's Bad Fur Day_
* [Diddy Kong Racing](https://github.com/DavidSM64/Diddy-Kong-Racing) - An in-progress decompilation of _Diddy Kong Racing_
* [Donkey Kong 64](https://gitlab.com/dk64_decomp/dk64) - An in-progress decompilation of _Donkey Kong 64_
* [Doom 64](https://github.com/Erick194/DOOM64-RE) - A **complete** reverse engineering of _Doom 64_
* [Dr. Mario 64](https://github.com/angheloalf/drmario64) - An in-progress decompilation of _Dr. Mario 64_
* [F-Zero X](https://github.com/bttrdrgn/f-zerox) - An in-progress decompilation of _F-Zero X_
* [GoldenEye 007](https://gitlab.com/kholdfuzion/goldeneye_src) - An in-progress decompilation of _GoldenEye 007_
* [Harvest Moon 64](https://github.com/harvestwhisperer/hm64-decomp) - An in-progress decompilation of _Harvest Moon 64_
* [Knife Edge: Nose Gunner](https://github.com/disi33/KE-NG_Reversing) - Configures a reverse engineering environment (Mupen64+ RE, Ghidra, etc.) for _Knife Edge: Nose Gunner_
* [Kirby 64: The Crystal Shards](https://github.com/farisawan-2000/kirby64) - An in-progress decompilation of _Kirby 64: The Crystal Shards_
* [Mario Kart 64](https://github.com/n64decomp/mk64) - An in-progress decompilation of _Mario Kart 64_
* [Mario Party](https://github.com/Rainchus/mp1) - An in-progress decompilation of _Mario Party_
* [Mischief Makers](https://github.com/blackgamma7/mischief-makers) - An in-progress decompilation of _Mischief Makers_
* [Mystical Ninja Starring Goemon](https://github.com/fluvian/mnsg) - An in-progress decompilation of _Mystical Ninja Starring Goemon_
* [Neon Genesis Evangelion 64](https://github.com/farisawan-2000/evangelion) - An in-progress decompilation of _Neon Genesis Evangelion 64_
* [Paper Mario](https://github.com/pmret/papermario) - A **complete** decompilation of _Paper Mario_
* [Perfect Dark](https://gitlab.com/ryandwyer/perfect-dark) - A **complete** decompilation of _Perfect Dark_ (see also [pdtools](https://gitlab.com/ryandwyer/pdtools))
* [Pokémon Puzzle League](https://github.com/angheloalf/puzzleleague64) - An in-progress decompilation of _Pokémon Puzzle League_
* [Pokémon Snap](https://github.com/ethteck/pokemonsnap) - An in-progress decompilation of _Pokémon Snap_
* [Pokémon Stadium](https://github.com/pret/pokestadium) - An in-progress decompilation of _Pokémon Stadium_
* [Quest 64](https://github.com/Mallos31/Quest) - An in-progress decompilation of _Quest 64_
* [Rocket: Robot on Wheels](https://github.com/RocketRet/Rocket-Robot-On-Wheels) - An in-progress decompilation of _Rocket: Robot on Wheels_
* [Shadowgate 64](https://github.com/Rainchus/shadowgate64) - An in-progress decompilation of _Shadowgate 64_
* [Space Station Silicon Valley](https://github.com/mkst/sssv) - An in-progress decompilation of _Space Station Silicon Valley_
* [Star Fox 64](https://github.com/sonicdcer/sf64) - An in-progress decompilation of _Star Fox 64_
* [Super Mario 64](https://github.com/n64decomp/sm64) - A **complete** decompilation of _Super Mario 64_
* [Super Smash Bros.](https://github.com/vetritheretri/ssb-decomp-re) - An in-progress decompilation of _Super Smash Bros._
* [Superman 64](https://gitlab.com/farisawan-2000/superman) - An in-progress decompilation of _Superman 64_
* [Wave Race 64](https://github.com/LLONSIT/wr64) - An in-progress decompilation of _Wave Race 64_
* [Yoshi's Story](https://github.com/decompals/yoshis-story) - An in-progress decompilation of _Yoshi's Story_
* [Zelda OOT](https://github.com/zeldaret/oot) - An in-progress decompilation of _The Legend of Zelda: Ocarina of Time_
* [Zelda MM](https://github.com/zeldaret/mm) - An in-progress decompilation of _The Legend of Zelda: Majora's Mask_

#### Other

* [n64-kicad](https://github.com/nterry/n64-kicad/) - A set of KiCad files detailing the Nintendo 64 hardware
* [N64 Uncompiled Source Code](http://shygoo.net/n64-uncompiled/) - Various source code and related material discovered in various ROM images
* [nus-cpu](https://github.com/dmkfasi/nus-cpu) - A condensed, modular re-creation of the Nintendo 64 motherboard
* [shogihax](https://cturt.github.io/shogihax.html) - Details a remote code execution exploit of the Nintendo 64 via the _Morita Shogi 64_ cartridge and its dialup modem
* [Ultra FP64](http://www.ultrafp64.com/) - A work in progress FPGA Nintendo 64
* [UltraCIC](https://github.com/mikeryan/UltraCIC) - A clone of the CIC copy protection chip

### Guides and Reference

* [n64-decompiling](https://www.retroreversing.com/n64-decompiling) - An overview of decompiling Nintendo 64 ROMs with Ghidra
* [awesome-decompilation](https://github.com/nforest/awesome-decompilation/blob/master/README.md) - A curated list of awesome decompilation resources and projects

### Tools and Disassemblers

* [N64LoaderWV](https://github.com/zeroKilo/N64LoaderWV) - Nintendo 64 ROM loader for the [Ghidra](https://github.com/NationalSecurityAgency/ghidra) reverse engineering tool
* [RI Probe](https://www.romhacking.net/homebrew/102/) - A ROM that dumps RDRAM values onscreen for debugging and exploring
* [n64sym](https://github.com/shygoo/n64sym) - Scans a RAM dump for symbols from a given library or object file
* [Online Disassembler](https://onlinedisassembler.com/odaweb/) - A lightweight, online service for when you don't have the time, resources, or requirements to use a heavier-weight alternative
* [Compiler Explorer](https://godbolt.org) - Explore how your C, C++, Rust, or other compiled language code ends up looking after compilation
* [mips_to_c](https://github.com/matt-kempster/mips_to_c) - An open-source MIPS decompiler, useful for understanding and reimplementing N64 games' behavior in C
* [GEDecompressor](https://github.com/jombo23/N64-Tools/tree/master/GEDecompressor) - Decompressor for a wide variety of compression formats used across various titles
* [asm-differ](https://github.com/simonlindholm/asm-differ) - A `diff` script for MIPS assembly
* [decomp-permuter](https://github.com/simonlindholm/decomp-permuter) - A tool to randomly permute C files to better match a target binary
* [openocd_n64](https://github.com/juchong/openocd_n64) - An [OpenOCD](http://openocd.org/doc/html/About.html) configuration for the Nintendo 64 CPU

## Programming

### Assembly

* [PeterLemon/N64](https://github.com/PeterLemon/N64) - Nintendo 64 bare metal MIPS assembly programming reference
* [Fraser N64](https://www.youtube.com/channel/UC3tcfSES8CB45DmTbHhUP1w) - YouTube channel featuring Nintendo 64 assembly programming
* [N64 Assembly Language Tutorial](https://sites.google.com/site/consoleprotocols/home/homebrew/n64-assembly-home) - Fraser's detailed Nintendo 64 assembly programming guide
* [N64-ASM-Tutorial](https://github.com/fraser125/N64-ASM-Tutorial) - The support files for N64 Assembly Language Tutorial
* [N64 ASM Tutorials](https://patater.com/gbaguy/n64asm.htm) - Nintendo 64 assembly language programming tutorials by Mike Huber (mirrored by Jaeden Amero)
* [n64-assembly](https://github.com/is06/n64-assembly) - A [Visual Studio Code](https://code.visualstudio.com/) extension that provides language support and theme for the Nintendo 64 assembly language
* [n64-asm-timing](https://github.com/pdrome/n64-asm-timing) - Nintendo 64 CPU instruction timing
* [n64ops](https://github.com/mikeryan/n64dev/tree/master/docs/n64ops) - R4300i, RCP, and RSP opcode details
* [neon64v2](https://github.com/hcs64/neon64v2) - An original Nintendo Entertainment System emulator, written in assembly
* [cubeworld](https://gitlab.com/is06/cubeworld) - The beginnings of an experimental game, written in assembly
* [sodium64](https://github.com/Hydr8gon/sodium64) - A SNES emulator for the N64, written in assembly

### C

#### Guides

* [N64 Homebrew Starter Guide](https://drive.google.com/drive/folders/1rOE2zYV2RPPx-2NHRGiGZ-RFx6w_6dAI) - Buu342's guide to creating an N64 game with the official SDK
* [Implementation of Sounds Using the Nintendo 64 Sound Tools](https://docs.google.com/document/d/1d1qKxMh3q_89w9N76xL9bXRqkXe1ylcDnAtg3cgu5s8) - Buu342's guide to implementing sound in your ROM with the Nintendo 64 Sound Tools
* [N64Squid Homebrew](https://n64squid.com/homebrew/n64-sdk) - Development walkthrough using the NuSystem library that's part of the official SDK
* [moria.us #nintendo-64](https://www.moria.us/tags/nintendo-64) - A series of blog posts covering a broad range of Nintendo 64 development topics

#### Example Code

* [ultra64demos](https://github.com/shlomnissan/ultra64demos) - Original SGI Nintendo 64 technical demos
* [n64-sdk-demo](https://github.com/jsdf/n64-sdk-demo) - jsdf's detailed example with heavily-commented source showing basic usage of the official SDK and the NuSystem library
* [N64brew Game Jam 2023](https://github.com/N64brew-Game-Jam-2023) - N64brew Game Jam 2023 submissions
* [brick64](https://github.com/allie/brick64) - A homebrew 3D brick-breaker game using the official SDK
* [goose64](https://github.com/jsdf/goose64) - jsdf's _Untitled Goose Game_ "demake"
* [helloworld](https://github.com/loociano/n64dev/tree/master/helloworld) - Hello World example using NuSystem and S2DEX microcode
* [Controller-Pak-Manager](https://github.com/manfriedn64/Controller-Pak-Manager) - A ROM that presents graphical user interface to manage Controller Pak data
* [shibamatch](https://github.com/einhov/shibamatch) - A Shiba Inu-themed memory match game
* [ochim](https://github.com/murachue/ochim) - An up to 4 player action puzzle game
* [UltraEd](https://github.com/deadcast2/UltraEd/) - An in-progress level editor and game engine
* [n64zlibbench](https://github.com/clbr/n64zlibbench) - A zlib benchmark with result display
* [gb64](https://github.com/lambertjamesd/gb64) - A Nintendo Game Boy emulator that runs on real hardware
* [mvs64](https://github.com/rasky/mvs64) - A NeoGeo emulator
* [n64-gba](https://github.com/Dillonb/n64-gba) - A proof of concept Game Boy Advance emulator (only runs ARMWrestler, a CPU exercise ROM)
* [platformer64](https://github.com/lambertjamesd/platformer64) - An in-progress adventure platformer
* [Memory64-N64](https://github.com/vieux/Memory64-N64) - A Simon style memory game with Rumble Pak support, using libdragon
* [Mine64](https://github.com/SiliconSloth/Mine64) - A Minecraft clone, using Nintendo's NuSystem library
* [64doom](https://github.com/jnmartin84/64doom) - A source port of the original _DOOM_
* [cmake-demo-rom](https://github.com/N64-tools/cmake-demo-rom) - Demonstrates building toolchains and a ROM using CMake and `libdragon`
* [n64_controller_test](https://github.com/Ryzee119/n64_controller_test) - A simple homebrew ROM built with `libdragon` to perform some basic controller tests
* [ultra64-templates](https://github.com/stefanmielke/ultra64-templates) - Game templates/starting points for use with n64sdkmod
* [wolf64](https://github.com/9nova/wolf64) - A port of _Wolfenstein 3D: Spear of Destiny_, adapted from Wolf4SDL and using `libdragon`.
