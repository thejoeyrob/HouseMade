# HouseMade v3 — Flat GitHub PWA

HouseMade v3 is a self-contained installable Progressive Web App designed to run from a flat static host such as GitHub Pages.

## Publish
Upload these files to the root of the GitHub Pages repository and enable Pages for the branch/folder you use:
- index.html
- styles.css
- app.js
- manifest.webmanifest
- sw.js
- icon-192.png
- icon-512.png
- apple-touch-icon.png

The normal browser view intentionally shows only installation guidance. The full HouseMade workspace opens from the installed PWA.

## v3 highlights
- Premium redesigned Home dashboard with upcoming tasks and a quirky weekly progress board.
- Schedule renamed to **Planner**.
- Planner includes Day, Week and Month diary/calendar views with previous/next navigation.
- Floating `+` opens a planner window that can place one chore on multiple days and multiple times.
- Weekly, biweekly, monthly and one-week-only recurrence options.
- Planner chores can be assigned to one or several family members.
- Family assignments automatically form a **Prompt Queue**, ready for future native Apple notification/action integration.
- Prompt Queue currently supports generated reminder copy, SMS handoff, email handoff, Alexa-ready copy text and local PWA notifications where supported.
- **Your Button** generates a random self-care reminder, appreciation note or small treat/reset suggestion.
- **Clean Break** mini-game: a five-stage retro handheld cleaning game. Collect mess, grow your cleaning trail, avoid obstacles and clear Bedroom → Kitchen → Bathroom → Living Room → Garage.
- Game controls include both a left-side touch joystick and right-side Up / Down / Left / Right buttons, plus keyboard arrows.
- Improved visual room imagery, richer cards, transitions, quote presentation and completion feedback.
- Quote refresh is now a small arrow rather than an “Another” text button.
- Existing Quick Clean / Deep Clean customization, timers, playlist links, sounds, gold completion and offline local persistence remain intact.

## Important flat-PWA limitation
GitHub Pages is static hosting. HouseMade can prepare reminder queues and can show local notifications while the installed PWA is active and the browser/runtime permits them. It cannot guarantee background scheduled delivery after iOS fully terminates the PWA, and it cannot silently send SMS/email without a server/provider.

The Planner and Prompt Queue data model is deliberately structured so those actions can later be connected to an Apple-native wrapper, push service or messaging backend without redesigning the planner itself.


## v3.1 game controls
- Replaced joystick + small D-pad with one large four-way control pad.
- Pointer-down input and a short direction queue improve rapid cornering and Right-button response.
- Playfield wraps at all four edges: exiting one side re-enters from the opposite side.


## v3.2 game display update
- Clean Break now opens as a dedicated edge-to-edge full-screen game surface instead of a scrolling modal.
- HouseMade page scrolling and overscroll are locked while the game is open.
- The game screen and four-way controls scale to the available device height, including landscape layouts and safe areas.
- Closing the game restores the normal HouseMade workspace.
