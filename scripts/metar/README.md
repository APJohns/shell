# METAR

A python script that pulls the METAR data from aviationweather.gov and prints to the console the metar you are looking for and whether the airport is currently VFR or IFR.

## Installation

### ZSH
1. Download and add this script to whereever you keep your custom scripts e.g. `/Users/user_name/bin`. Make sure no file  extensions have been added.
    - If you have not set up a custom script before, create a bin folder where your .zshrc file is. and add the script there. Then update your path in the .zshrc to include that bin folder.
2. At the top of the file, add your path to python prefixed by `#!` e.g. `#!/usr/bin/python3`.

This script can also be run as a regular python script by adding the `.py` extension and running as you would normally run a pythons cript.

## Usage

`metar <ICAO Code>` - Returns the metar for the specified airport. The code is case insensitive.

### Example
```
$ metar kbos
KBOS 081454Z 31019G26KT 10SM FEW060 FEW250 10/02 A3015 RMK AO2 PK WND 31031/1357 SLP209 T01000017 51013
KBOS flight conditions are  VFR
```