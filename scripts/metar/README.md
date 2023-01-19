# WX

A python script that pulls weather data from aviationweather.gov and prints to the console the METAR or TAF you are looking for.

## Installation

### ZSH
1. Download and add this script to whereever you keep your custom scripts e.g. `/Users/user_name/bin`. Make sure no file  extensions have been added.
    - If you have not set up a custom script before, create a bin folder where your .zshrc file is. and add the script there. Then update your path in the .zshrc to include that bin folder.
2. At the top of the file, add your path to python prefixed by `#!` e.g. `#!/usr/bin/python3`.

This script can also be run as a regular python script by adding the `.py` extension and running as you would normally run a pythons cript.

## Usage

`wx <MODE (METAR or TAF)> <ICAO Code>` - Returns the METAR or TAF for the specified airport. The code and mode are case insensitive.

### Example
```zsh
$ wx metar kbos
KBOS 190454Z 28009KT 10SM CLR 06/01 A2989 RMK AO2 SLP121 T00560006 401110044
KBOS flight conditions are  VFR
```

```zsh
$ wx taf kbos
KBOS 190540Z 1906/2012 29010KT P6SM SKC FM192000 19004KT P6SM VCSH OVC110 FM192300 13004KT 5SM -RA BR OVC030 FM200100 10007KT 2SM -RA BR OVC008 FM200700 05012G19KT 2SM -RA BR OVC008
```