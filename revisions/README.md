# Each folder stands for it's own revision showing the build date

## folder jlcpcb-board-prod
### gerber, drill and map files
The zip file contains it all. No need to unpack, it can be uploaded to the board manufacturer as it is.

### bom.csv and top-pos.csv
These 2 files can be used if you want jlcpcb.com to solder all SMD components on the board. Please upload bom.csv as BOM, top-pos.csv as CPL.
**ATTENTION**: All through hole components are *NOT* included in this BOM and the pre-assembly process. Please complete the board by manualy soldering them!

## folder pcbway-board-prod
### gerber, drill and map files
The zip file contains it all. No need to unpack, it can be uploaded to the board manufacturer as it is.

### board-view pngs
Preview pictures of the board.

### bom.pdf
This is the list with all parts and some installation material. *Download* the file and get access to real offers in the column "purchase" (suggestive).

### ibom.html
This is the interactive bill of materials which will help you placing the components on the board. It also shows more information about the components' footprint designators.

Here some [usage hints](https://github.com/openscopeproject/InteractiveHtmlBom/wiki/Usage#bom-page-mouse-actions).
