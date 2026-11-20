ISWAPPRO SHOPPING MASTER V23
Universal purchasing and shopping manager.

OPEN ON ANDROID
1. Export a JSON backup from your existing app before replacing anything.
2. Extract this ZIP using your phone's file manager.
3. Open the extracted folder.
4. Tap index.html and choose Chrome.
5. Your app data remains in the same browser storage key when opened in the same browser profile. If data does not appear, import your JSON backup from Insights & Reports.

BARCODE SCANNING
- Tap Scan barcode in the shopping item form or inventory form.
- V23 uses a delegated button handler so taps on the button and its contents are handled.
- The app checks camera API availability, secure context and BarcodeDetector support, and reports the reason if scanning cannot start.
- Allow camera permission when Chrome asks.
- For reliable live camera scanning, serve the extracted app from HTTPS or localhost. Chrome/Android may block camera access from a content:// local file.
- If live scanning is unavailable, type or paste the barcode into the barcode field and save the item.

PURCHASE LISTS
- General Shopping: groceries, household items, clothing, electronics, personal care, education/office and other purchases.
- Business Items: products, equipment, packaging, stationery and other business-related purchases.
- Tools & Project Items: building materials, electrical/plumbing supplies, tools and project supplies.
Lists stay separate. Changing tabs does not archive a list. Checkout archives only collected items; unchecked items remain active.

QUANTITY CONTROLS
Use + and − directly on each shopping-list row. Quantity updates are saved immediately. Whole units increment by 1; measured units increment by 0.1.

PROJECT STRUCTURE
index.html — Android-compatible self-contained app.
css/styles.css — matching editable stylesheet source.
js/app.js — matching editable JavaScript source.
assets/ — icons and images.
documentation/ — project and QA notes.

DATA & PRIVACY
Data is stored locally in this browser. No cloud sync or online payment is included. Export a JSON backup regularly. Keep the previous app folder until you verify the new version.


V24 BARCODE SCANNER NOTES
- The scan button now displays a specific diagnostic when camera access or barcode decoding is unavailable.
- Live scanning requires HTTPS or localhost, camera permission, and Chrome BarcodeDetector support for product barcode formats.
- Opening index.html from Android content:// storage may prevent camera access.
- If the browser reports that BarcodeDetector is unavailable, use manual barcode entry; this build does not download a decoder and therefore remains usable offline.
- For live scanning, publish this folder to a trusted HTTPS static host (for example GitHub Pages) and open the HTTPS address in Chrome.
