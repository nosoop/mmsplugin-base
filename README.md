# Metamod:Source Plugin Template

A project repository template that builds Metamod:Source plugins using [AMBuild].

## Building

1. Get the requirements for [Building SourceMod][].  (Following that process will download the
necessary HL2SDK branches, Metamod:Source, and AMBuild.)
2. Run the following set of commands:

    # clone this repository to mmsplugin-sample (or start a new project based off of the template and clone it)
    git clone https://github.com/nosoop/mmsplugin-base mmsplugin-sample
    
    # create a build directory
    cd mmsplugin-sample
    mkdir build
    cd build
    
    # configure the build with the appropriate paths and the SDKs you'd like to build with, then build
    python ../configure.py --hl2sdk-root ${PATH_CONTAINING_HL2SDK_DIRS} -s ${SDK_VALUES} --mms-path ${PATH_TO_MMSOURCE}
    ambuild

[AMBuild]: https://github.com/alliedmodders/ambuild
[Building SourceMod]: https://wiki.alliedmods.net/Building_SourceMod

## License

This repository is derived from [`metamod-source/sample_mm`][], and as such is in the public
domain.

[`metamod-source/sample_mm`]: https://github.com/alliedmodders/metamod-source
