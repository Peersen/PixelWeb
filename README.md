# PixelWebGV

This is a fork of PixelWeb for a specific apllication
three Columns in a cellar have each a circle opf WS2801 LED
Server is a Raspi3

*** This repo wont work for your application **

todo s:


- [ ] Pixelweb hinter einem anderen Server wie Apache, nginx o.ä. verstecken damit der anwender nicht auf einen Server mit sudo-rechten trifft.
- [x]config Menüpunkte vorm User verstecken

  -> html multiline comment aus den menüounkten in `/ui/index.html` machen

  -> siehe Zeile 58 + 65 in index.html

- [x] Link zum repository hinzugefügt
- [x] Link zu einer Anleitung
- [ ] den haupthelligkeitsregler aus den configbereich in einen anderen verlegen Autostart
- [ ] eine autostart queue erstellen die einge harmlose animationen enthält
- [ ] autostart queue bei jedem start aus einem entfernten Ordner kopieren oder allen usern die write rechte auf diese datei entziehen, das sie nicht versehentlich veränder/gelöscht wird

- [ ] automatisch die autsostart queue beim programmstart starten

- [ ] starte run-pixelweb via cronjob mit @reboot mit:

  `run-pixelweb /home/pi`

  damit der Server die config dateien nicht in /root/ ablegt

---

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
