# Panchayat Scheme Finder (prototype)

Trilingual (English / Bengali / Hindi) web app with voice input and read-aloud.
Sample data only: 12 schemes with simplified rules. Verify against official sources before real use.

## Files
index.html, manifest.json, sw.js, icon-192.png, icon-512.png (keep all in the repo root)

## Put it on GitHub as a website
1. Create a new public repository on github.com.
2. Upload all 5 files to the repository root ("Add file" > "Upload files").
3. Settings > Pages > Source: "Deploy from a branch", Branch: main, folder: / (root) > Save.
4. After a minute your site is live at https://YOUR-USERNAME.github.io/REPO-NAME/
   (Voice input needs https, which GitHub Pages provides. Use Chrome on Android/desktop.)

## Make an Android APK
Option A (easiest): go to pwabuilder.com, paste your GitHub Pages URL, click Start, then
"Package for stores" > Android > Generate. Download the zip; it contains an .apk (for testing) and an .aab.
Option B: use Bubblewrap (npm i -g @bubblewrap/cli; bubblewrap init --manifest=YOUR_URL/manifest.json; bubblewrap build).
For a quick demo without an APK: open the site in Chrome on the phone > menu > "Install app" / "Add to Home screen".

## Editing schemes
In index.html, edit the S array (name, benefit, documents, rule) and the D array for documents.
