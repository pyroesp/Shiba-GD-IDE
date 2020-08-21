# Shiba GD-IDE

The Shiba GD-IDE is a complete redesign of GD-IDE board for the Toshiba GD-ROM Optical Drive.  
The GD-IDE allows you to plug in an IDE HDD into your dreamcast.  

The original GD-IDE is designed by tawy / DragonCity.  
You can find it here : [Dreamcast GD-IDE](https://boutique-dragoncity.myshopify.com/collections/dreamcast/products/dreamcast-pcb-dreamcast-gd-ide-v3-connecteur-ide)

## Disclaimer

Obviously, I'm not responsible if this breaks your GD-ROM drive.  
At the time of writing (21/08/2020) the boards have not yet been tested.

## Shiba GD-IDE PCB

KiCad 3D model:  
<img src="./pics/Shiba GD-IDE front.png">  
  
<img src="./pics/Shiba GD-IDE back.png">  


FreeCAD 3D model:  
  
<img src="./pics/Shiba GD-IDE freecad model.png">

## Compatible GD-ROM

The Shiba GD-IDE is only compatible with GD-ROM drive that have a Toshiba IC on top.  
<img src="./pics/Toshiba board.png">  

## GD-ROM drive Connector

The connector is apparently a Molex 0525840579 that you can find on digikey.  
I got the pinouts from the schematics found on [console5.com](https://console5.com/wiki/Dreamcast).  
  
The connection to the IDE HDD I got from DragonCity's image below.  
<img src="./pics/Molex GD-ROM Connector.png">  


All pinouts and connections to test points can be found in the text file in the docs folder.

## License

CC BY 4.0  
See LICENSE.md