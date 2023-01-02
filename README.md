# KiCad Coils: generated footprints for placing coils in your PCB

This is a set of footprints and symbols for placing coils in PCBs produced using KiCad.
The footprints are generated using my fork of the [kicad-coilgenerator](https://github.com/cst0/kicad-coil-generator) project. If you need
a coil not found here, my recommendation would be to tweak the parameters there and generate
your own set of footprints (it's pretty easy).

The footprints are generated using the following parameters:

- Minimum trace width of 0.128mm (5 mils)
- Minimum trace spacing of 0.128mm (5 mils)
- Coil inner radius of 1.0, to provide a bit of space for vias, etc.
- Outer radii ranging from 10mm to 100mm, in increments of 5mm
- Spiral and Square coils

These are the minimum parameters specified by a handful of manufacturer guidelines,
but double-check that they are suitable for your needs. To avoid multi-layer confusion,
I've only generated single-layer coils. If you want more layers, just drop more coils
on top of each other in your PCB. This will require placing multiple coils in the schematic.

The symbol is a generic coil symbol, and so only one is necessary. To use it,
place the coil symbol in your schematic. When pairing the symbol to a footprint,
select the footprint best suited for your design. The footprint names provide
details on the coil parameters: they are of the form `coil_<coil shape>_<outer radius>_<trace width>`.
