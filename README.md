## xc3sprog ##

Suite of utilities for programming Xilinx FPGAs, CPLDs, and EEPROMs with the Xilinx Parallel Cable and other JTAG adapters under Linux (and now macOS).

Forked from [original xc3sprog project](http://xc3sprog.sourceforge.net/) (source available over SVN [at SourceForge](https://sourceforge.net/p/xc3sprog/code/HEAD/tree/)), with improved compatibility with macOS.

All documentation in this file relates to macOS installation and usage. For Linux and Windows, please see the [original `README` file](README.old).


### Quick Start ###

1. Make sure you have [installed Homebrew](https://brew.sh/)
2. `brew install bunkyr/core/xc3sprog`


### Usage ###

1. Connect board to computer over USB
2. Using Vivado (in a VM), generate a bitstream for a project, making sure that the output `.bit` file is copied or synced to your host computer
3. `xc3sprog -c {cable} {path/to/bitfile.bit}`

This has primarily been tested on a Nexys A7 board (cable type `nexys4`). All other utilities provided by the original xc3sprog should work as documented elsewhere in this repository, but no guarantees are provided and no testing with other boards has been performed.
