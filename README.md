# [Open Hardware DSP Platform](http://www.ohdsp.org)
## KiCad-Libs
### KiCad libraries for use with revision 1.1 and newer boards only
---
# README
### Disclaimer
Copyright Paul Janicki 2019

Licensed under the TAPR Open Hardware License (www.tapr.org/OHL)

This documentation is distributed WITHOUT ANY EXPRESS OR IMPLIED WARRANTY, INCLUDING OF MERCHANTABILITY, SATISFACTORY QUALITY AND FITNESS FOR A PARTICULAR PURPOSE.

### What is this repository for?

**Quick summary**

These KiCad libraries are for use with Open Hardware DSP revision 1.1 or newer schematic and PCB designs. 

For older version of projects (revision 1.0) please check out the older version of the KiCad-Libs.

This also contains the BOM generation plugin under the "Plugins" folder. This can be added to eeschema by going to Tools -> Generate Bill of Materials -> Add Plugin and browsing to the Plugins folder.
Example Command Line: xsltproc -o "%O.csv" "C:\Electronics\KiCad-Libs\Plugins\OHDSP_BOM_Generation_V2.xsl" "%I"
This will generate an .xml and .csv BOM file in the directory containing the project .pro file. The CSV file uses the semicolon seperator ";".

The library should be stored in a directory such as "C:\Electronics\KiCad-Libs" on a windows system. OHDSP projects are then stored in "C:\Electronics\OHDSP\ *{Project Name}* ". Projects use relative paths for libraries where possible and so should work when setup this way, however see each project README.md file for detailed library setup information.

If you create a new project with versions 4 of KiCad the schematic library list for a project should only contain this library. There may be conflicts with built in passive components if the default libraries are used as well. There should not be any problems with KiCad 5 versions.