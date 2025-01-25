# SV08-PZ-Probe
E3D Revo PZ-Probe for the Sovol SV08

## Project Aims
1. To swap the supplied hot end and Z probe for the E3D Revo PZ-Probe.
2. To use as many of the existing parts as possible.
3. To work with the Sovol branch of Klipper.
4. 3D printed parts should not require support.

## New 3D printed parts 
The new 3d printed parts can be found in the STEP directory.  As most modern slicers can open STEP files directly this is the preferred format for this project.

The parts should be orientated correctly on import as shown below. All parts have been designed so that support is not required, provided your printer can cope with small bridges.

### Print Orientation
![Part orientation](./assets/PartOrientation.png)

The prototype was printed in PETG on a Bambu Labs A1 mini, 0.16mm layer height, 3 wall loops, 100% infill.  If your Sovol SV08 has an enclosure or you plan on printing high temperature filamanets, ASA or ABS would be preferred.

Bambu Slicer project files (.3mf) for the parts are available in the 3mf folder.

## Printed Part Preparation

### Heat set inserts

The parts are designed around M3 x 6mm unflanged inserts, except for the upper two on the main mount, that should be M3 x 5mm.  If preferred, 5mm long inserts can be used in all locations. Alternatively, 6mm inserts can be used everywhere, if you don't mind them sticking out a little from the main mount.  

All inserts should sit level or below the face of insertion.  Any plastic the bulges up should be removed, so that parts fir together without gaps.

#### Main Mount

The main mount upper inserts need to be aligned with the inside of the mounting slot for maximum strength and ease of assembly.  See the image below.

<img alt="SV08-PZ-Mount-Inserts" src="./assets/SV08-PZ-Mount-Inserts.jpg" height="480"> <img alt="SV08-PZ-Mount-Align" src="./assets/SV08-PZ-Mount-Align.jpg" height="480">

#### Fan mount with nozzles

<img alt="SV08-PZ-Nozzle-Inserts" src="./assets/SV08-PZ-Nozzle-Inserts.jpg" height="480">

#### Fan mount interface

Make sure the inserts sit below the mating face and remove any plastic preventing the mating face from sitting flat, to ensure an airtight seal with the nozzles.

<img alt="SV08-PZ-Interface-Inserts" src="./assets/SV08-PZ-Interface-Inserts.jpg" width="480">

#### Cable clamp

The cable clamp uses a sacrificial layer to support the counterbored screw holes.  This will need to be drilled through.

<img alt="SV08-PZ-Clamp-Insert" src="./assets/SV08-PZ-Clamp-Insert.jpg" align="top" height="240">  <img alt="SV08-PZ-Clamp-Drilling" src="./assets/SV08-PZ-Clamp-Drilling.jpg" align="top" height="240">

### Magnets

This design uses 4mm diameter x 3mm long neodium magnets.  I used these ones https://www.amazon.co.uk/dp/B0C81HTXTV

It is important to ensure that the magnets are inserted the correct way round.  The easiest way to ensure this is to snap the magnet to an already mounted one on the tool head and mark the non-contact face with a permanent marker.  The marked face goes at the bottom of the hole on the cover. With care, for some of the magnets, it is possible to push the mounting hole over the magnet while it is snapped in place.

#### Cover

Try to keep all the magnets orientated the same way.

<img alt="SV08-PZ-Cover-Magnets" src="./assets/SV08-PZ-Cover-Magnets.jpg" height="480">

#### Fan mount interface

Snap a magnets to each of the lower pair in the cover.  Slide the interface into the cover and press the two parts together.  Once the magnets are partially seated in the fan interface it can be removed and pressed against a flat surface to fully seat them.

<img alt="SV08-PZ-Interface-Magnets" src="./assets/SV08-PZ-Interface-Magnets.jpg" width="480">

## Stripping the exiting toolhead

1. Disconnect the large fan and remove it from the cover.

    <img alt="Cover screws" src="./assets/CoverScrews.jpg" height="480">
    
2. Remove the standard nozzle and heatsink assembly as shown in this video:
   
   [![Nozzle change video](http://img.youtube.com/vi/bAOVA6bL-Jw/0.jpg)](http://www.youtube.com/watch?v=bAOVA6bL-Jw)
   
4. Remove the small fan from the heatsink.  Keep the screws.
   
   <img alt="Nozzle screws" src="./assets/NozzleScrews.jpg" height="480">
   
7. Unscrew the Z-Probe and disconnect the cable. Remove the cable clamp. You can optionally disconnect the power and usb connections for clearer access.
   
   <img alt="Toolhead screws" src="./assets/ToolheadScrews.jpg" height="480">

## PZ-Probe Assembly

Align the coldside on the mount so that the cable points away from the fan ring and assemble using M3x6 buttonhead screws.  The two side screws are placed in their cut-outs and the hex driver engages in their heads through the holes in the top.

<img alt="SV08-PZ-Assembly1" src="./assets/SV08-PZ-Assembly1.jpg" height="480"> <img alt="SV08-PZ-Assembly2" src="./assets/SV08-PZ-Assembly2.jpg" height="480">

Mount the PZ-probe board in place using the M2 capheads supplied with the board.  These screws will cut their own threads in the mount.

<img alt="SV08-PZ-Assembly3" src="./assets/SV08-PZ-Assembly3.jpg" height="480">

Loop the ribbon cable around and connect tto the pz-probe board.  Use a small zip tie to hold it in place.

<img alt="SV08-PZ-Assembly4" src="./assets/SV08-PZ-Assembly4.jpg" height="480"> <img alt="SV08-PZ-Assembly4a" src="./assets/SV08-PZ-Assembly4a.jpg" height="480">

Using the original 2 screws attach the cold end cooling fan.  4 holes are available but only two are needed.  The screws will cut their own thead.

<img alt="SV08-PZ-Assembly5" src="./assets/SV08-PZ-Assembly5.jpg" height="480">

The PZ-Probe comes with a short length of bowden tube. Cut this to 33.5mm, and insert through the mount until it bottoms in the heatsink.  

<img alt="SV08-PZ-Assembly6" src="./assets/SV08-PZ-Assembly6.jpg" height="480">

Insert the bowden tube into the toolhead as shown below and push up.  The mount will snap over the original heatsink mount. If the mount doesn't seat completely, trim a small amount off of the bowden tube and try again. 

<img alt="SV08-PZ-Assembly7" src="./assets/SV08-PZ-Assembly7.jpg" height="480"> <img alt="SV08-PZ-Assembly8" src="./assets/SV08-PZ-Assembly8.jpg" height="480">

Use two M3x20 and one M3x8 screws to secure the mount.  The screws enter from the opposite side compared to the original heatsink.

<img alt="SV08-PZ-Assembly9" src="./assets/SV08-PZ-Assembly9.jpg" height="480">

Combnine the part cooling fan interface and nozzle items together with three M3x8 countersunk screws

<img alt="SV08-PZ-Assembly10" src="./assets/SV08-PZ-Assembly10.jpg" height="480">

Fix this to the main mount with two M3x8 countersunk screws.  The next stage is the wiring and it's handy to have the fan mount in place to determine the wire lengths.

<img alt="SV08-PZ-Assembly11" src="./assets/SV08-PZ-Assembly11.jpg" height="480">

Slot the 5020 fan into the interface and fix with M3x25 screws and washers.  The washers help protect the fan case from splitting from the screw heads. 

<img alt="SV08-PZ-Assembly12" src="./assets/SV08-PZ-Assembly12.jpg" height="480">

The new screw clamp can be fitted at this stage with M3x12 screws or left until after the wiring is completed.

<img alt="SV08-PZ-Assembly13" src="./assets/SV08-PZ-Assembly13.jpg" height="480">

Test fit the cover to ensure the magnets snap together. An M3x8 screw can be used to permanently fix the cover.

<img alt="SV08-PZ-Assembly14" src="./assets/SV08-PZ-Assembly14.jpg" height="480">

This completes the mechanical assembly.

## PZ-Probe Wiring

The Sovol SV08 uses a variety of connectors. While the existing probe connector can be harvested, a second one is required for 5V power taken from the spare UART. Both connectors are JST-GH plugs with 1.25mm pin spacing: 5 pin for the probe and 4 pin for the UART. I used this kit from Amazon https://www.amazon.co.uk/gp/product/B0CW2NKVL7

<img alt="Toolhead Board" src="./assets/Toolhead board.jpg" height="480">

Threee ground pins are available. I used the one on the UART to keep the wiring neat for the later addition of an X-axis limit microswitch.

# Hotend Wiring

If you don't have the right connectors on hand, harvest the ones from the Sovol heater and thermister.  Cut them off keeping 15mm to 20mm of wire tails attached.  Fit the E3D Revo hotend to the heatsink. The Revo has Molex connectors fitted and comes with extension cables.  For the initial setup I used the extension cables, but later removed them, cutting off the Molex, and soldering the cables to the toolhead connector tails, making sure there was a little slack in the cables once connected.

