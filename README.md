# nepgDump - Nord Electro 3 Program Parameter Dump

## Purpose
This Python script extracts the parameter values from Nord Electro 3 program files and either prints them to screen or writes them to a .csv file for import in Excel. Single and multiple program files can be evaluated at once.

Knowledge of the program parameter settings, especially those not visualized on the NE3 panel, helps with modifying existing programs. It can be used for documentation purposes as well.

## Usage
For instructions on how to use the script see the following output created by typing `python nepgDump.py -h`:

```
usage: nepgDump.py [-h] [-d DST] [-f] SRC

positional arguments:
  SRC                source file (w/o ext) / src folder with option '-f'

optional arguments:
  -h, --help         show this help message and exit
  -d DST, --dst DST  writes results to <DST>.csv / <SRC>.csv with '-d $'
  -f, --folder       process all .nepg files in folder <SRC>
```

## Contents
Here is a short description of all files contained in this project:

| File                      | Description                             |
| ------------------------- | --------------------------------------- |
| nepgDump.py               | NE3 dump script (main module)           |
| nepgParser.py             | Parser module (imported by main module) |
| nepgOut.py                | Output module (imported by main module) |
| NE3 Template.xlsm         | Empty Excel template                    |
| NE3 Factory Programs.xlsm | Example Excel table                     |

## Requirements and compatibility
This Python script requires Python 2.7 being installed on your computer.

It has been tested with NE3 program files created by the Nord Sound Manager v6.74 and NE3 program files downloaded from the Nord Homepage. However, the script is assumed to be compatible with all existing versions of NE3 program files.

## Acknowledgement
Some basic ideas have been taken from a similar dump script for Nord Electro 4 program files. It has been written by Christian E. and can be found on GitHub by using the following link: https://github.com/10x10sw/NordUser/tree/master/DumpNE4P
