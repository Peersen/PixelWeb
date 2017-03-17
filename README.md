
This is a fork of PixelWeb for a specific apllication
three Columns in a cellar have each a circle opf WS2801 LED
Server is a Raspi3 

to Dos:
-make Pixelweb autostart on Port 80
-hide config tabs of webmenu after manually setting up network config
-(auto) generate an empty autostart qeue on startup if it not exists
-automatically start autostart que on boot 

PixelWeb is a dynamic graphical interface for our super flexible animation SDK, [BiblioPixel](http://github.com/maniacallabs/BiblioPixel). It runs everywhere BiblioPixel does and provides an easy to use web-based interface to nearly everything BiblioPixel can do. This not only allows local system control but via any other computer on the same network<sup>&dagger;</sup>.  

## Installation

*Note: Manual install is possible but using pip is highly recommended and all that will be covered in the documentation. Also, Windows users should exclude "sudo" from all commands.

PixelWeb Requires Python 2.7 and is not compatbile with Python 3.x. If you do not have Python installed or are unsure, visit [python.org/downloads](http://python.org/downloads) and follow the instructions.*

Installing PixelWeb is easy:
```
sudo pip install PixelWeb
```

Once the install is complete run the following command:
```
sudo run-pixelweb
```
On every run, PixelWeb will automatically check if the system has the required dependencies and install them. This includes [BiblioPixelAnimations](http://github.com/maniacallabs/BiblioPixelAnimations), our animation repository. It contains the initial animations that will be available through the interface. Please see the Wiki on how to add your own animations.


<sup>&dagger;</sup> Note that PixelWeb is designed to be used like a desktop application by a single user at a time, despite being accessible from multiple systems at once. There is currently no mechanism to keep multiple interface instances in sync.
