# Changelog

## [Unreleased]
- WIP: connector panel board for easier mounting on enclosure

## [0.97] - 2021-12-10
### Added
- CHANGELOG.md format based on [Keep a Changelog](https://keepachangelog.com)
### Changed
- optimizing vias 
- small improvement on vcc tracks to led driver ic 
- other minor enhancements and improvements 

### Deprecated
### Removed
### Fixed
### Security

## [0.96] - 2021-12-07
### Added
### Changed
- better silkscreens at screw terminal connectors 
- thicker and better tracks to the LED outputs 
- other minor enhancements and improvements 
### Deprecated
### Removed
### Fixed
### Security

## [0.95] - 2021-12-06
### Added
### Changed
- minor enhancements and improvements
### Deprecated
### Removed
### Fixed
### Security

## [0.95] - 2021-12-04
### Added
- [lcsc](https://lcsc.com/) part number in bom.xlsx where possible trying to scope on pre building the board. Not including (not available, too expensive or better arrange locally) 
  - *espP32 mini* and *step down converter module 5V 1A* (better get them from [aliexpress](https://aliexpress.com))
- Usage of teardrops on round tht pads and smaller tracks for low power connections
- interactive bom (ibom.html) as help for component placement reference on board 
### Changed
- joined the free to use GPIOs, 5 Volt fused and ground header pins in one horizontal connector 
- using electrolyte capacitors with tht layout (formally smd) for better availability/prices and easier handling 
- new smd power inductors for better availability/prices and a bit more space on the board 
- new smd schotty power diodes for better availability/prices and easier handling and a bit more space on the board 
- Improved placement for led power components and optimized led power track routing





### Deprecated
### Removed
- after some discussions with others about the external 5Volt in function and considering my personal usage case, the decision was taken to remove this functionality. The benefit is arguable and very low, the complexity rises, better keep it simple.
### Fixed
### Security

## [0.93] - 2021-11-25
### Added
- First trial with external 5V in to keep the MCU powered on even when the bigger power supply is powered off 
- placing a small on broad double throw single pole switch to chose the matching MCU power source 
- setting up silkscreen indications near the dtsp switch 
- rerouting MCU power tracks 
- renaming exposed GPIO silkscreens for external relay 
### Changed
### Deprecated
### Removed
### Fixed
### Security

## [0.92] - 2021-11-16
### Added
### Changed
- minor enhancements and improvements
### Deprecated
### Removed
### Fixed
### Security

## [0.91] - 2021-11-12
### Added
### Changed
- minor enhancements and improvements
### Deprecated
### Removed
### Fixed
### Security

## [0.9] - 2021-11-11
### Added
### Changed
- focus on installing the board in a pre made enclosure with mounting hole distances 105mm/55mm 
- shrinking the board size 
- setting up a 4th mounting hole on the board and placing all of them at the correct place 
- adapting etch cuts with rounded corners to the matching size
- redoing **all component placement, all track routing and all silkscreens**, from zero 
- testing, measuring, checking heat dissipation with ir cam, rechecking power handling and long term tests once again 
### Deprecated
### Removed
### Fixed
### Security

## [earlier revisions]
- basically to do some fundamental testing/measuring, choosing the matching components, shrinking the board to a compact size while improving it's power throughput. 
- achieve the official permission to use the "made for ESPHome"-Logo, showing the project to specialists, getting their opinion and answer their questions 
- measuring, burning parts, rebuilding, ordering prototype boards, soldering them together, collecting information and throw the later prototype boards to trash moving on to the nest prototype revision ... ~ 50 or more iterations like this :-) 
- this stage is not published in the changelog as it is a creative and chaotic process.

