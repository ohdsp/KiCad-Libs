# README - Kicad-Libs  #

## Disclaimer ##
Copyright Paul Janicki 2016

Licensed under the TAPR Open Hardware License (www.tapr.org/OHL)

This documentation is distributed WITHOUT ANY EXPRESS OR IMPLIED WARRANTY, INCLUDING OF MERCHANTABILITY, SATISFACTORY QUALITY AND FITNESS FOR A PARTICULAR PURPOSE.

### What is this repository for? ###

**Quick summary**

These are the Kicad libraries that work with open hardware DSP designs in other repositories.

KiCad-Libs is designed to be placed in a directory such as "C:\Electronics\KiCad-Libs". Open hardware DSP projects would then be placed in "C:\Electronics\OHDSP\ *{project name}* ". Projects use relative paths for libraries and setting files up like this should make designs work without any changes to library paths.

If you create a new project with versions of KiCad upto and including 4.0.1-stable the schematic library list for a project should only contain this library and the built in power library. There may be conflicts with built in passive components if the default libraries are used as well, although you are free to experiment or modify this library for your own use (delete conflicting components).
