CALM & RESTORE PWA

FILES
- index.html: the application
- manifest.webmanifest: install metadata
- service-worker.js: offline cache
- icons/: Android and maskable app icons

DEPLOYMENT
1. Upload the CONTENTS of this folder together, preserving the icons folder.
2. Serve the folder from an HTTPS website. Do not open index.html as file:// when testing installation.
3. Visit the HTTPS address in Chrome on Android.
4. Tap Install app inside Calm & Restore, or use Chrome menu > Install app / Add to Home screen.
5. Open it once online so its core files can be cached. It can then reopen offline.

TEST LOCALLY ON A COMPUTER
From this folder run: python3 -m http.server 8080
Then visit http://localhost:8080 in Chrome. Localhost is allowed for PWA development.

UPDATES
If files change, increment CACHE in service-worker.js (for example calm-restore-v2) before uploading.

DATA
User entries remain in localStorage for that browser/device. Use the built-in JSON export regularly. Clearing site/app storage can erase local data.
