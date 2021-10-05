# DGAdmin
DGAdmin for TeknoMW3

- Originally forked from FredericaBernkastel's DGAdmin, InfinityScript 1.5 (1.5.0.29) port branch: https://github.com/FredericaBernkastel/codmw3-server-DGAdmin-plugin/tree/IS1.5

## Aim of my DGAdmin work
- Working admin plugin for TeknoMW3 AIZombies mode
    - AIZombies works with InfinityScript 1.5.3 only, requiring recompiling DGAdmin with that version of binary
    - Commands need to be created for DGAdmin that specifically exploit features of the AIZombies mode

## My modifications
- Recompiled with InfinityScript 1.5.3 (binary: `./DGAdmin/InfinityScript 1.5.3/InfinityScript_1.5.3.dll`)
- Added useful commands for TeknoMW3 AIZombies mode (see `./additional files/commands.md`)

## Work in progress
- Add more commands through reverse engineering AIZombiesSupreme.dll (i.e. via dnSpy)
- Make created commands less janky
- Keep up documentation on commands through `./additional files/commands.md`

## Build environment
- v3.5.1 (details from memory)
    - OS: Windows 10
    - IDE: Visual Studio Express 2015
- v3.5.1.1 to current build
    - OS: MacOS 11.3 Big Sur
    - IDE: Visual Studio 2019 for Mac (Community license)

## Todo
- [x] Decide on project license (FredericaBernkastel's DGAdmin used the GPL-3.0 License)
