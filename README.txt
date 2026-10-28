MY HEALTH TRACKER PWA — PHONE-ONLY SETUP

FILES
- index.html: the complete app
- manifest.webmanifest: install/app metadata
- sw.js: offline caching
- icons/: app icons

IMPORTANT
A PWA must be served from HTTPS (or localhost) for installation, service workers,
and notifications. Opening index.html directly from Downloads will not enable
all PWA features.

PHONE-ONLY PUBLISHING OPTION: GITHUB PAGES
1. In Chrome, open https://github.com and create/sign in to a free account.
2. Create a new public repository named my-health-tracker.
3. Upload the files from this folder, preserving the icons folder and its two PNG files.
   If uploading on mobile, use the repository's Add file / Upload files feature.
4. Open repository Settings > Pages.
5. Under Build and deployment, select Deploy from a branch, choose main and /(root), then Save.
6. Wait for GitHub Pages to publish and open the provided HTTPS website address.
7. In Android Chrome, open the website menu (three dots) and choose Install app or Add to Home screen.

INSTALL TEST
- Open the HTTPS website in Chrome.
- Use the three-dot menu > Install app (or Add to Home screen).
- Launch the home-screen icon.
- Test daily logs, reports, JSON backup and CSV export.

DATA
The app stores health entries in local browser storage on that device. Export JSON regularly.
Clearing site data may erase records. This version has no cloud sync.

LIMITATIONS
- The PWA sensor is experimental and cannot guarantee background step counting.
- The reminder is checked while the app page is open; it is not a reliable scheduled
  background alarm. Reliable background steps and scheduled reminders need native Android code.
