![](../../workflows/gds/badge.svg) ![](../../workflows/docs/badge.svg)

# Tiny Tapeout ECE298A Analog Tile, 2026/05/18

- [Read the documentation for project](docs/info.md)

https://app.tinytapeout.com/projects/4917

A. Circuit Descriptions

1. Flip-flops 1 and 2
Marco Volpini and Mounib Jamous (2 designs)
https://github.com/MounibJa/SRAM-NMOS-CELL

2. Flip-flop 3
Robert Tang
https://github.com/robertyt33/TinyTapeout-ECE298A

3. Precharge circuit
David Gao and David Ye
https://github.com/davvdf/SRAM_precharge_access

4. Differential Amplifier 1
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


## Analog projects

For specifications and instructions, see the [analog specs page](https://tinytapeout.com/specs/analog/).

## Enable GitHub actions to build the results page

- [Enabling GitHub Pages](https://tinytapeout.com/faq/#my-github-action-is-failing-on-the-pages-part)

## Resources

- [FAQ](https://tinytapeout.com/faq/)
- [Digital design lessons](https://tinytapeout.com/digital_design/)
- [Learn how semiconductors work](https://tinytapeout.com/siliwiz/)
- [Join the community](https://tinytapeout.com/discord)
