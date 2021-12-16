## Each folder stands for it's own revision showing the build's date

### board-view
show some 3D pictures of the board.

### bom
This is the parts list. *Download* the pdf file and get access to real offers in the column "buy suggestion".

### ibom
This is the interactive bill of materials which will help you placing the components on the board. It also shows more information about the component's form factor.

Here some [usage hints](https://github.com/openscopeproject/InteractiveHtmlBom/wiki/Usage#bom-page-mouse-actions).

### jlcpcb-bom.csv and jlcpcb-top-pos.csv
These 2 files can be used if you want jlcpcb.com to solder all SMD components on the board. Please upload bom.csv as BOM, top-pos.csv as CPL.
**ATTENTION**: All through hole components are *NOT* included in this process. Please arrange them nonetheless and complete the board by manualy soldering them!

### gerber
This can be used to order the board at jlcpcb.com or pcbway.com. All my tests where based on standard 1oz cupper thickness and showed positive results.
