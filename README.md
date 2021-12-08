# sdlarch-visualstudio

This repo is simply putting sdlarch into a Visual Studio Solution. It also includes a pre-compiled Mesen Core, and ROM of From Below.

My hope is that one day this can be a "drag and drop" solution to porting NES games (and possibly other ROMs) to platforms like Steam, XBOX, Playstation and Switch.

Currently it is in a pretty rough state, but should run any NES game with keyboard input.

# sdlarch

sdlarch is a small libretro frontend (sdlarch.c has less than 1000 lines of
code) created for educational purposes. It only provides the required (video,
audio and basic input) features to run basic libretro cores and there's no UI
or configuration support.

## Building

Open sdlarch.sln in Visual Studio 2019. Select Debug | x64 config (I haven't setup up the others yet). Select Build -> Build Solution.

When running, you must pass 2 arguments to the command line (the project should already be setup to do this): the core to load, and the ROM to run.

## Running

    ./sdlarch <core> <uncompressed content>

