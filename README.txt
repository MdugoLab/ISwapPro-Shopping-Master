ISWAPPRO SHOPPING MASTER V26
HTTPS CAMERA DEPLOYMENT & ANDROID TEST

LOCAL TEST
1. Keep your previous version and export a JSON backup from Insights & Reports.
2. Extract this ZIP fully using the Android Files app. Do not open index.html inside the ZIP preview.
3. Open the extracted index.html in Chrome. Shopping lists and manual barcode entry should work.
4. Camera access may be blocked for a local content:// file. This is a browser security restriction, not necessarily an app fault.

PUBLISH TO GITHUB PAGES (HTTPS)
1. Open the ISwapPro-Shopping-Master repository on GitHub. Do not change the separate Career Hub repository.
2. Upload/replace the V26 project files in the repository root. Keep index.html at the root and preserve the css/ and js/ folders.
3. Open repository Settings > Pages.
4. Under Build and deployment, choose Deploy from a branch.
5. Select branch main and folder /(root), then Save.
6. Wait for GitHub Pages deployment to complete. Open: https://mdugolab.github.io/ISwapPro-Shopping-Master/
7. In Android Chrome, open the HTTPS page, tap the site controls icon beside the address, open Permissions, set Camera to Allow, then reload. If prompted, choose Allow while using the site.
8. Open Add Item or Inventory > Scan barcode. Grant camera access. Point the rear camera at a clear EAN/UPC barcode in good light. Tap Stop camera when finished.

CAMERA TROUBLESHOOTING
- “Not a secure context”: use the HTTPS GitHub Pages address, not the local file.
- “Permission denied”: Chrome site settings > Camera > Allow, then reload. Also check Android Settings > Apps > Chrome > Permissions > Camera.
- “Camera busy”: close Camera, WhatsApp, or other apps using the camera.
- “BarcodeDetector unavailable” or unsupported format: camera may work but this Chrome build lacks a compatible built-in barcode decoder. Manual barcode entry remains available. A future fallback decoder can be bundled if required.
- HTTPS is necessary but does not guarantee BarcodeDetector support.

DATA WARNING
Local file storage and the GitHub Pages website have different browser origins. Data stored in the local-file version may not automatically appear on the HTTPS website. Export JSON from the old version and import it on the HTTPS version if needed. Keep your previous folder until you confirm the data is present.

PROJECT STRUCTURE
index.html
css/styles.css
js/app.js
manifest.webmanifest
sw.js
README.txt / README.md / VERSION.txt

SCOPE
Universal purchasing and shopping management only. No accounting, invoicing, payroll, CRM, booking, or catering workflows.
