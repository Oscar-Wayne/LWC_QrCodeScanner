# LWC_QrCodeScanner
Qrcodescanner is a LWC for a salesforce1 , you can scan and open automatically the Qr scanned in your mobile.
Using the barcodescanner API
In the component JavaScript file, BarcodeScanner it's imported using the standar JavaScript "import", import the "getBarcodeScanner() factory function from the 
"lightning/mobileCapabilities".

Like this:
import { getBarcodeScanner } from 'lightning/mobileCapabilities';

Adding to JavaScript file this part of code:

```JavaScript
>// Here, we just display the scanned value

this.scannedBarcode = result.value;if(this.scannedBarcode.indexOf("http://")=== 0 ||this.scannedBarcode.indexOf("https://") ===0)
window.location.replace(this.scannedBarcode);
 ```      
 
#### you can open automatically the Qr scanned.    :shipit:                    
