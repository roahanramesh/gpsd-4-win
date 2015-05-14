GPSd is required by several Open Source programs that deal with GPS receivers: navit, viking, gpsdrive, [GMapCatcher](http://code.google.com/p/gmapcatcher/) ... only to name a few.

Unfortunately, the [GPSd website](http://gpsd.berlios.de/) states:
_"No, we don't support Windows — get a better operating system."_ ; However, with an installed [cygwin](http://www.cygwin.com/) you can run GPSd under Windows.

<br>
<h2>Installation</h2>
Installing GPSd on Windows is now very simple:<br>
<ul><li>Just download and run the <a href='http://code.google.com/p/gpsd-4-win/downloads/list'>latest installer</a></li></ul>

<h2>Starting GPSd</h2>
<ul><li>Stop ALL programs using the GPS receiver.<br>
</li><li>Launch "GPSd for Windows"<br>
<ul><li>you should have a shortcut in your desktop.<br>
</li><li>or launch it directly "C:\cygwin\gpsd4win.bat"<br>
</li></ul></li><li>If the Windows-Firewall now issues a warning, click the "Don't block" button.<br>
</li><li>After some initial text on the console, nothing happens - that's ok!</li></ul>

<br>
<h2>Hints / Troubleshooting</h2>
<a href='http://code.google.com/p/gpsd-4-win/source/browse/trunk/binary/batch/gpsd4win.bat'>gpsd4win.bat</a> should auto-detect the COM port, if your GPS device is not detected you can set it manually!<br>
<br>
<ul><li>If you get an error "Could not find cygwin1.dll", then your probably not running in: c:\cygwin\bin<br>
</li><li>All gpsd console programs are closed by pressing Crtl-C in the corresponding console window.<br>
</li><li>Running the GPS receiver for the first time, it may take a few minutes before the receiver has a satellite fix.<br>
</li><li>In case your GPS gets confused, e.g. if you had run both gpsd and another software using the GPS, try to unplug and replug the GPS.<br>
</li><li>If you plug your GPS into a different USB port, it might get a new COM port number!<br>
</li><li>Bluetooth may use very high COM port numbers (COM40 !) that won't work with gpsd (or cygwin?) - try to set a lower COM port number in your Bluetooth software</li></ul>

<br><br>
<br><br>
This project was inspired from:<br>
<a href='http://home.arcor.de/ulf.lamping/gpsd/gpsd.html'>http://home.arcor.de/ulf.lamping/gpsd/gpsd.html</a>