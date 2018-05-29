# Docker Image to Build the Unreal Engine 4 Editor in Linux

## Obtaining the Source
Epic requires you to add your Github account name to your profile in order to access the engine's source code. Once you do, clone the source using the branch name that matches your image's tag.

For example, to clone v4.19:

`git clone --depth=1 -b 4.19 git@github.com:EpicGames/UnrealEngine.git`

## Running the Build
Once the code is cloned to your machine, run the image as follows to build the editor, using the same tag as the branch you cloned:

`docker run -it --rm -v ${PWD}/UnrealEngine:/opt/ue4 anpage/ue4:4.19`
