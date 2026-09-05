<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works

ECE298A-F2025 Analog Tile, 2026/09/05

https://app.tinytapeout.com/projects/4917

A. Circuit Description

1. Flip-flops 1 and 2
Marco Volpini and Mounib Jamous (2 designs)
https://github.com/MounibJa/SRAM-NMOS-CELL

2. Flip-flop 3
Robert Tang
https://github.com/robertyt33/TinyTapeout-ECE298A

3. Precharge circuit
David Gao and David Ye
https://github.com/davvdf/SRAM_precharge_access

4. Differential Amplifier 1a
Ernest James (EJ) Ramas and Ethan Pang
https://github.com/ejramas/TT_RAM-SRAM-Sense_Amp

5. Differential Amplifier 2
Harry Wang and Benjamin Zeng
https://github.com/hapsdoifh/ECE298A-Sense-Amp-Project

The floorplan of the ECE298A analog tile on Skywater Sky26b tapeout (May 18, 2026) is shown in an 
image in the /docs folder on github. All ‘UI_in’ inputs, except UI_in[4], are buffered by x8-sized inverters. 
The global supply (VDPWR) is 1.8V. There are 5 analog I/Os: UA_[0] to UA_[4]. All unused outputs 
are connected to ground (VGND).

Differential amplifier inputs and outputs are selected via control lines UI_in[0] and UI_in[1] and CMOS 
analog switches as 2:1 multiplexers. 

The flip flops are driven from input UI_in[2] to UI_in[4]. Digital outputs are buffered by a x1/x3 inverter 
cascade to outputs UO_out[0] to UO_out[7] for readout.

## How to test

Digital inputs and outputs are driven and analyzed from the TT testboard and microcontroller 
interface to a laptop.

Analog inputs are sourced from a signal generator or DC power supply. 
Outputs are analyzed using an oscilloscope and multimeter.


## External hardware

Signal generator, oscilloscope, multimeter
