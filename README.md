# Nala Phone Level

Quick planning survey of nala cross sections and L-sections using the phone's tilt sensor, a tape and two poles. It gives the height of each bank above the bed, bank-full depth, top width, flow area, HFL height and bed slope, with an error estimate for every reading.

**Open the app:** https://pmdsc2020.github.io/nala-phone-level/

## Files

| File | What it does |
|---|---|
| `index.html` | The whole app (camera crosshair, tilt sensor, calculations, drawings, exports) |
| `sw.js` | Keeps a copy on the phone so the app opens with no network in the field |
| `manifest.webmanifest` | Lets the phone install the app to the home screen |
| `icon.svg`, `icon-192.png`, `icon-512.png` | App icons |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

## Put it on GitHub Pages

1. On github.com, signed in as **pmdsc2020**, click **New repository**. Name it `nala-phone-level`, set it to **Public**, and create it.
2. Click **uploading an existing file**. Drag in all the files from this folder, including `.nojekyll` (turn on "show hidden files" if you can't see it). Click **Commit changes**.
3. Go to **Settings → Pages**. Under "Build and deployment", choose **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.
4. Wait 1–2 minutes. The app is live at `https://pmdsc2020.github.io/nala-phone-level/`.

## On the phone

1. Open the link in **Chrome** while you have network.
2. Tap the menu (⋮) → **Add to Home screen** / **Install app**.
3. Open it once from the home screen, tap **Calibrate**, and allow camera access when asked. Location is asked the first time you capture GPS.
4. After this the app opens without network. Survey data stays on the phone; use **Export & share → Backup (JSON)** after each field day.

## Updating the app later

Upload the new `index.html`, and in `sw.js` change `nala-phone-level-v1` to `v2` (then `v3`, and so on). Phones get the new version the next time they open the app with network, and again after one more reopen. Survey data on the phone is not affected.

## Accuracy

About ±3 cm at a 10 m sight and ±6 cm at 20 m with a steady hand, after calibration. Each instrument move adds its own error. Good for siting structures and planning; use an auto level for final estimates.

---
Jitendra Sonawane, Agriculture Engineer, 7720045808
