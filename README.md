# angular2-qrscanner
QrScanner will scan for a QRCode from your Web-cam and return its
string representation by drawing the captured image onto a 2D Canvas
and use [@LazarSoft/jsqrcode](https://github.com/LazarSoft/jsqrcode) to check for a valid QRCode every *Xms*

```html
   <qr-scanner
      [debug]="false"        <!-- debug flag for console.log spam              (default: false) -->
      [canvasWidth]="640"    <!-- canvas width                                 (default: 640) -->
      [canvasHeight]="480"   <!-- canvas height                                (default: 480) -->
      [mirror]="false"       <!-- should the image be a mirror?                (default: false) -->
      [stopAfterScan]="true" <!-- should the scanner stop after first success? (default: true) -->
      [updateTime]="500"     <!-- miliseconds between new capture              (default: 500) -->
      (onRead)="decodedOutput(string)"></qr-scanner>
```

I fixed the bugs:
A private variable to public 
Moved version.getversion to upper one 
