MY FAMILY RECIPE BOOK — iPhone + Mac

WHAT IS INCLUDED
index.html (the application), manifest.webmanifest, service-worker.js, two icon PNG files.
No subscription, tracking, accounts, or remote recipe database.

MAC (simple local use)
Open index.html in a browser. Your Mac copy is stored in that browser.
If Safari restricts local file storage, use a local web server (see below).

IPHONE HOME SCREEN APP (FREE HTTPS HOSTING)
1. Create a free GitHub account if you do not already have one.
2. Create a PUBLIC repository, e.g. family-recipe-book-app.
3. Upload index.html, manifest.webmanifest, service-worker.js, icon-192.png, icon-512.png to the repository root.
4. In repository Settings > Pages, choose Deploy from a branch, main, /(root), then Save.
5. Wait for GitHub to provide your https://USERNAME.github.io/REPO/ address.
6. Open that address in iPhone Safari while online. Use Share > Add to Home Screen > Add.
7. Launch the Home Screen icon once while online; after successful caching the app shell works offline.
8. Open the same URL on your Mac for a browser-based Mac copy.

IMPORTANT PRIVACY
GitHub Pages hosts the application code, not the recipes you enter. Never upload your JSON backups or private photos to the public repository. Each browser/device stores its own recipes locally.

MOVE RECIPES AND SHOPPING LISTS BETWEEN DEVICES
1. On the device with the latest data, open Backup & help > Download complete backup (.json).
2. Save the JSON backup in iCloud Drive via Files on iPhone or Finder on Mac.
3. On the other device, Backup & help > Restore/import backup or recipe JSON.
4. Choose the file from iCloud Drive. Confirm importing recipes, plans, and groceries.
5. Keep dated backups in iCloud Drive, plus an occasional independent copy.

IMPORTANT: This is NOT automatic sync. Editing both copies separately can cause conflicts. Prefer one master device, and always export/import when switching devices. Importing recipes updates matching IDs, but the optional plan/list restore replaces those sections.

OFFLINE LIMITATIONS
The app needs one online visit to cache files on iPhone. Offline support depends on the browser retaining its website data; iOS may clear storage under pressure. Regular JSON backups are essential. Photos count toward browser storage limits.
Automatic photo-to-text recognition is NOT included; photos can be attached for reference, and ChatGPT can help transcribe them when online.

OPTIONAL LOCAL MAC TEST SERVER
From the unzipped folder in Terminal run: python3 -m http.server 8765
Then open http://localhost:8765/ in your Mac browser. This does NOT make it available on iPhone over HTTPS or install it as a PWA.
