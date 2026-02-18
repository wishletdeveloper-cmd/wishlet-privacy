# Wishlet — Privacy & Terms (GitHub Pages)

Use this folder as a **standalone GitHub repo** to host your Privacy Policy and Terms of Service for App Store Connect and in-app links.

## Quick setup

1. **Create a new repo on GitHub** (e.g. `wishlet-privacy` or `wishlet-legal`). Do not add a README (you’ll push this folder).

2. **Push this folder** as the repo root:
   ```bash
   cd wishlet-privacy-pages
   git init
   git add .
   git commit -m "Initial: Privacy and Terms for Wishlet"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Repo → **Settings** → **Pages**
   - Source: **Deploy from a branch**
   - Branch: **main** (or **master**), folder **/ (root)**
   - Save. Wait 1–2 minutes.

4. **Your URLs** (replace `YOUR_USERNAME` and `YOUR_REPO_NAME`):
   - Privacy: `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/privacy/`
   - Terms: `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/terms/`

5. **In the Wishlet app:** Open `friendsaction/Services/APIConfig.swift` and set:
   - `privacyPolicy` = your privacy URL
   - `termsOfService` = your terms URL  

   Then in **App Store Connect** → your app → **App Information**, set **Privacy Policy URL** to the same privacy URL.

## Before release

- In `privacy.md` and `terms.md`, replace `support@wishlet.app` and `privacy@wishlet.app` with your real support and privacy contact.
