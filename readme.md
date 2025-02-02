# Distance Randomizer
A Centrifuge plugin that randomizes Distance's Adventure mode. Almost all maps and abilities are
shuffled into a random order, requiring you to use some interesting strategies to complete some maps due to being less equipped than the developers intended.

There's now a website for the randomizer plugin at https://tiyenti.github.io/distrandomizer with more information!

## Installation
The latest version of the mod can be found and downloaded from the [releases page](https://github.com/Tiyenti/distrandomizer/releases).

See https://tiyenti.github.io/distrandomizer/install for instructions on how to install
the mod if you are unsure how to do this.

## Build instructions
Obviously, you will first need to clone the repo:

    $ git clone https://github.com/Tiyenti/distrandomizer.git

You will need to make sure the NuGet packages are present in  the solution folder:
Right-click on the solution in the `Solution Explorer` then click `Restore NuGet Packages`

distrandomizer is currently being developed with Visual Studio 2019 Community, so this is the reccomended IDE for developing/building the mod. Other IDE solutions may work as well
although they are not officially supported.

After compiling the plugin, the resulting `DistanceRando.Plugin.dll` assembly can
then be copied from the build directory to a new directory in the `[distance-path]/Centrifuge/Mods` directory alongside the `mod.json` manifest from the project root in the following structure:

    Distance_Data/
    ┕ Centrifuge
      ┕ GameSupport
        ┕ Centrifuge.Distance.dll
      ┕ Mods
        ┕ DistanceRando
          ┕ DistanceRando.Plugin.dll
          ┕ mod.json
        ┕ ...
      ┕ ...
    ┕ ...

From here, providing that everything is properly set up (with Centrifuge and the Distance GSL
installed), you should be able to launch the game with the compiled plugin.
