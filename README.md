# Shiba GD-IDE

The Sega Dreamcast uses a GD-ROM Optical Drive to read the game discs. Some clever people discovered that the optical drive uses connections similar to an IDE HDD.  
If you look for *Dreamcast HDD mod* on Google Images you'll see some crazy stuff. People were just soldering 40 pin flat ribbon cables to the motherboard or optical drive directly, which looks pretty cool to be honest.  

Some guys designed the GD-IDE which is a PCB, which is soldered on top of the optical drive of the Dreamcast, that allows you to plug in an IDE HDD.  
The Shiba GD-IDE is a complete redesign of GD-IDE board for the Toshiba GD-ROM Optical Drive.  

The name *Shiba GD-IDE* comes from the fact that the GD-ROM optical drive has a To**shiba** chip on it and the name of the original board. 

The original GD-IDE is designed by tawy / DragonCity.  
You can find the GD-IDE on DragonCity's webpage here: [Dreamcast GD-IDE](https://boutique-dragoncity.myshopify.com/collections/dreamcast/products/dreamcast-pcb-dreamcast-gd-ide-v3-connecteur-ide)

## Disclaimer

Obviously, I'm not responsible if this breaks your GD-ROM drive.  
At the time of writing (21/08/2020) the boards have not yet been tested.

## Compatible GD-ROM

The Shiba GD-IDE is only compatible with GD-ROM drive that have a Toshiba IC on top, like shown below.  
<img src="./pics/Toshiba board.png">  

## Shiba GD-IDE PCB

If you're going to buy some boards directly from a PCB fab, change the width of the board to 1mm.  
I'm using JLCPCB to make my boards and that's why I have added 'JLCJLCJLCJLC' on to the board as a place holder for their order number.  
It's kind of hidden under the 40 pin header, which is where I want it.  

Just like on the GD-IDE, you want to remove pin 20 from the header pins, to make it fit with DragonCity's ribbon cable.  

KiCad 3D model:  
<img src="./pics/Shiba GD-IDE front.png">  

<img src="./pics/Shiba GD-IDE back.png">  


FreeCAD 3D model:  
<img src="./pics/Shiba GD-IDE freecad model.png">

## GD-ROM drive Connector

The connector is apparently a Molex 0525840579 that you can find on digikey.  
I got the names of the Molex connections from the schematics found on [console5.com](https://console5.com/wiki/Dreamcast).  
  
The connections from the Molex connector to the IDE HDD I got from DragonCity's image below.  
<img src="./pics/Molex GD-ROM Connector.png">  
*Note: I have added the smaller numbers into the two columns to make it easier for me to map

All pinouts, pin names and connections to test points can be found in the text file in the docs folder, which looks like this:  
> ...
> 
> IDE HDD to Dreamcast GD-ROM TP:
> -------------------------------
> IDE 1 - ~RESET		A2		TP226 (not needed but provide bridge, see install tutorial GD-IDE from Dragoncity.fr)  
> IDE 2 - GND		A8/GND  
> IDE 3 - HD7		A4		TP229  
> IDE 4 - HD8		A5		TP231  
> IDE 5 - HD6		B4		TP230  
> ...  

## BOM

- PCB from any PCB fab you want. I personnaly use JLCPCB as they're cheap.  
- IDE flat ribbon cable, like the one sold by DragonCity here: [IDE cable](https://boutique-dragoncity.myshopify.com/collections/dreamcast/products/nappe-ide-80-pins-ata-133)  
- Optional: [IDE to SATA adapter](https://boutique-dragoncity.myshopify.com/collections/dreamcast/products/adaptateur-ide-sata-jm20330-jp103-5) also sold by DragonCity  

## License

CC BY 4.0  
See LICENSE.md