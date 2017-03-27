# Interface board for Digilent Analog Discovery 2

[![Join the chat at https://gitter.im/analogdiscovery2io/Lobby](https://badges.gitter.im/analogdiscovery2io/Lobby.svg)](https://gitter.im/analogdiscovery2io/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

**Please note that this is totally untested - will update when confirmed**

A board to interface anything that uses 3.5mm mono jacks (synthesisers etc) with the Digilent Analog Discovery 2 oscilloscope/wave generator/logic analyser.

Provides access to both scope channels, wave generators, triggers plus DIO 0 to 7 via 3.5mm mono jacks. DIO 8 to 15 and V+/V-/Ground via pin headers. The negative differential scope channels are connected to ground.

Note that the wave generator can output -+5V, however the DIO only 3.3V. This board does not implement any kind of level shifting, so if you're testing inputs with the output of the DIO channels then your module needs to work with 3.3V gates/triggers.

Connects directly to the AD2 with a female header. I made this as an edge connector — so you can use a 2x15 or two 1x15 straight headers.

Note; the digital I/O (including triggers) on the AD2 supports overvoltage up to -+20V. Rev-b includes resistors on all jack sockets except the scope channels. Suggest 1k on the wave generator (denoted with a dot) and 10k on the DIO.

There are 3mm holes in each corner for stand offs to support the board.

* 14 qty Thonkiconn jack sockets; https://www.thonk.co.uk/shop/3-5mm-jacks/
* 1 qty single row 15-pin female header (cheaper) -or- double row 2x15 female header (a bit more expensive)
* 4 qty 3x1 pin headers (female if you want to use male-male jumpers wires etc)
* 1 qty 9x1 pin headers (female if you want to use male-male jumpers wires etc)
* 2 qty 1k 0603 resistor
* 10 qty 10k 0603 resistor
* 4 x M3 stand offs plus screws
