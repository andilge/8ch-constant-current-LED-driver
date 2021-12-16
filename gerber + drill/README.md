## Each folder stands for it's own revision showing the build's date

### board-view
show some 3D pictures of the board.

### bom
This is the parts list. *Download* the pdf file and get access to real offers in the column "buy suggestion".

### ibom
This is the interactive bill of materials which will help you placing the components on the board. It also shows more information about the component's form factor.

Here some [usage hints](https://github.com/openscopeproject/InteractiveHtmlBom/wiki/Usage#bom-page-mouse-actions).

### jlcpcb-bom.csv and jlcpcb-jlcpcb-top-pos.csv
These 2 files can be used if you want jlcpcb.com to partially build the board. Please upload bom.csv as BOM, top-pos.csv as CPL
**ATTENTION**: the ESP32 (U10), 5V voltage converter (U200) and horizontal JST and Dupont board connectors (J110, J120, J130) are NOT included (I recommend buying from aliexpress.com and complete by soldering these through hole components yourself)!

### gerber
This can be used to order the board at jlcpcb.com or pcbway.com. All my tests where based on standard 1oz cupper thickness and showed positive results.
