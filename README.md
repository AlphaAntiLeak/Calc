# Simply Recycle — Netlify Pack

This folder contains everything you need to deploy the AMS247-style web app.

## Files
- `index.html` — single-page app with:
  - Sleek animated **login screen**
  - Cloud-only **orders** stored in **Firebase Firestore**
  - **Barcode** generator (Code 128) + **Share/Print**
  - Built-in **Scanner** using the browser camera
  - **Prices** editor with **cloud sync**
  - Material **icons** (inline SVG)
- `firestore.rules` — copy/paste into Firebase → Firestore → Rules.

## Firebase Setup (quick)
1. **Auth → Sign-in methods → Enable Email/Password**
2. **Add user**: use your admin email (e.g., `zoptris@gmail.com`) and password.
3. **Firestore**: create database → **Production**.
4. **Rules**: paste `firestore.rules` (edit the allowed email if needed).
5. Open the site — the app uses a **pre-baked config** (from `index.html`).

## Netlify Deploy
- Drag & drop this folder in Netlify, or push to a repo and connect.
- Requires HTTPS (Netlify provides it) for camera/scanner.

## Optional
- In `index.html`, you can replace the pre-baked Firebase config block if your project changes.
