# Changelog

## [Unreleased]
### To be added
- Bigger 5V buck converter to serve additional power consumption of the addressbale LEDs
- Deep diving once again into tests with infrared thermal cam on the very last revision. Don't get me wrong, this has been done with positive results in earlier revisions and it's only been improved. Documentation and publication is lacking though
- Wiki and step by step guide. I know I'm lazy at documentation, just more fascinated in getting things up, running and QCed :-)
- Tests with all the external sensor/actor stuff with pir motion sensor and rotary encoder on 10 meter distant from board. Since the connectors have changed with v0.99 and debouncing/hum filter has dropped in with v0.991 I'll have to wait until these parts and the new board version are here first

## [0.996] - 2022-02-03
### Added
### Changed
- better zone handling around the mounting holes
- wider radius on many rounded corners for trackes, better track fillets
- better placement on some debouncing filter components, shortening tracks
- some minor cosmetics all around the board
### Deprecated
### Removed
### Fixed
### Security

## [0.995] - 2022-01-15
### Added
- Introducing a data bus for adressable LEDs on 6 pin JST XH connector going to encoder
- Simple level shifter 3.3V to 5V for data line
- Selectable data line attenuation 33Ω (short cable) or 253Ω (long cable) with pin header jumper
- Addtitional resettable fuse for LED power line
### Changed
- new buck converter delivering more power for the adressable LEDs on the controller
- new placment for power supply, debouncing filter and connector components
- rerouting all tracks on these components
### Deprecated
### Removed
### Fixed
### Security

## [0.994] - 2022-01-07
### Added
- Adding push button on the board (parallel to the one in the rotary encoder)
### Changed
- Fillet tracks for all tracks
- Minor routing improvments all over the board
### Deprecated
### Removed
### Fixed
- Eliminating some courtyard overlap errors by slightly changing component placements
- Adding decoupling resistors in PWM lines
### Security

## [0.993] - 2022-01-07
### Added
- Introducing fillet tracks (rounded corner in tracks)
### Changed
- Moving the light power components to the board's edge => larger power zone in the middle, lowering resistance
- Redoing all the zones, reconnecting some tracks
- Revamping the buzzard labels near the screw terminals
### Deprecated
### Removed
### Fixed
### Security


## [0.992] - 2022-01-05
### Added
- Introducing small buzzard labels near the screw terminals
- Introducing thermal reliefs on though hole and smd solder pads when in a zone
### Changed
- minor changes of placement of some vias, moving away from silk screens
### Deprecated
### Removed
### Fixed
### Security

## [0.99r2] - 2021-12-16
### Added
- introducing jlcpcb-smd-bom.csv BOM and jlcpcb-top-pos.csv CPL for the SMD assembly of the board by jlcpcb. **ATTENTION**: All through hole components are NOT included in this per-assembly process. Please complete the board by manually soldering them
### Changed
### Deprecated
### Removed
### Fixed
### Security

## [0.99] - 2021-12-13
### Added
### Changed
- using horizontal JST connectors near the board edge to enable connecting the pir sensor and rotary encoder easily thru the enclosure
- new placement for the esp32 giving space for the JST connectors near the board edge
- rerouting all tracks around the JST connectors and esp32
- minor improvments in the 5 Volt line, better componenent placement and track routing
### Deprecated
### Removed
### Fixed
### Security

## [0.98] - 2021-12-12
### Added
### Changed
- new power inductor Bourns SRN6045 for better availabilty (widley spread in different stocks).
- Alternative inductor is GLE GCNR6045 with same characteristics and dimensions
- spreading out ground area on front and back layer
- silkscreen near screw terminal connectors LED1 - LED4 rotated for better readability
- new graphics for board dimensions and mounting hole distances
### Deprecated
### Removed
### Fixed
### Security

## [0.97] - 2021-12-10
### Added
- introducing CHANGELOG.md with format based on [Keep a Changelog](https://keepachangelog.com)
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
- [lcsc](https://lcsc.com/) part number in bom.pdf where possible, trying to scope on pre building the board. Not including (not available or too expensive, better get them from [aliexpress](https://aliexpress.com))
  - ESP32 mini
  - step down converter module 5V 1A
- first time usage of teardrops on round tht pads
- introducing the interactive bom (ibom.html) as help for component placement reference on board
### Changed
- joined the free to use GPIOs, 5 Volt fused and ground header pins in one horizontal connector
- using electrolyte capacitors with tht layout (formally smd) for better availability/prices and easier handling
- new smd power inductors for better availability/prices and a bit more space on the board
- new smd schotty power diodes for better availability/prices and a bit more space on the board
- smaller tracks for low power connections
- improved placement for led power components
- optimized led power track routing
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
- focusing on installing the board in a pre made enclosure with mounting hole distances 105-55mm
- shrinking the board size
- setting up a 4th mounting hole on the board and placing all of them at the correct place
- adapting edge cuts with rounded corners to the matching size
- redoing **all component placement, all track routing and all silkscreens** from almost zero
- testing, measuring, checking heat dissipation with ir cam, rechecking power handling and long term tests once again
### Deprecated
### Removed
### Fixed
### Security

## [earlier revisions]
- basically doing some fundamental testing/measuring, choosing the matching components, shrinking the board to a compact size while improving it's power throughput
- achieving the official permission to use the "made for ESPHome"-Logo
- showing the project to specialists, getting their opinion and answering some questions
- measuring, burning parts, rebuilding, ordering prototype boards, soldering components, collecting information and throw the earlier prototype boards to trash moving on to the next prototype revision ... ~ 25 or more iterations like this
- this stage is not published in the changelog as it is a creative and chaotic process.

