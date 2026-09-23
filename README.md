# HouseMade — Flat GitHub PWA v2

HouseMade is a completely self-contained installable PWA. No build step or server backend is required.

## GitHub Pages
1. Create/open a GitHub repository.
2. Upload **all files from this ZIP to the repository root** (do not upload the enclosing folder).
3. In GitHub: Settings → Pages → Deploy from a branch → `main` → `/ (root)`.
4. Open the resulting HTTPS URL on the phone/tablet.
5. iPhone/iPad: Share → Add to Home Screen. Android/desktop Chrome: Install app / Add to Home Screen.
6. The browser page intentionally shows installation instructions only. The HouseMade workspace opens in standalone/install mode.

## What works without a backend
- Daily / weekly / true calendar-month planner
- Weekly / biweekly / monthly recurring chores
- Quick Clean and Deep Clean profiles
- Editable master cleaning-step library
- Family assignments
- Generated copy/SMS/email/Alexa-ready reminder messages
- Local notification permission + reminders while HouseMade is running
- Timers, playlist links, sound effects and completion animations
- Offline use and device-local persistence
- Optional hashed local PIN

## Static-PWA limitation
A flat PWA cannot guarantee a scheduled SMS/email or a notification after the app has been fully closed by the operating system. HouseMade therefore uses one-tap SMS/email handoff and local notifications while the installed PWA is active/running. Fully automatic external messaging would require a backend/provider.

## Icon
The icon is a simplified traditional bell/fan-shaped feather duster, flipped 180° from the earlier concept: white silhouette on flat HouseMade lavender.
