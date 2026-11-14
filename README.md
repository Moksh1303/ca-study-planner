# Her CA Study Planner (free iPhone website)

## What is included
- Daily plan from 15 Nov 2026 through the January 2027 exams, based on the completed Excel planner.
- Audit, FM and SM syllabus checklist with completion percentages.
- Exam countdown.
- Subject-selectable stopwatch that continues while you switch tabs or lock the phone.
- Session history.
- One-hour daily Digital Marketing habit.
- Carry-forward action for missed daily tasks.
- JSON backup and restore.
- Offline cache after first load.

## Free hosting
This is a static website. It needs no paid server, database, account or subscription.

### Publish with GitHub Pages
1. Create a free GitHub account at https://github.com if she does not already have one.
2. Create a new public repository, for example `ca-study-planner`.
3. Upload every file in this folder to the repository root (`index.html`, `app.js`, `style.css`, `data.json`, `manifest.json`, `sw.js`, `icon.svg`).
4. In the repository, open Settings -> Pages.
5. Under Build and deployment, choose `Deploy from a branch`, select `main` and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish. The website URL will look like `https://USERNAME.github.io/ca-study-planner/`.

### Install on iPhone
1. Open the published link in Safari (not an in-app browser).
2. Tap Share.
3. Choose `Add to Home Screen`.
4. Confirm Add. Launch it from the new home-screen icon.

## Important data-storage note
Progress is stored locally in that iPhone's Safari website storage. It is not synced between devices or shared with another person. Export a JSON backup regularly from More -> Export backup. Import it later to restore progress. Avoid clearing Safari website data.

## Exam dates
The planner currently uses Audit: 10 January 2027 and FM + SM: 12 January 2027, as set in the Excel plan. Verify dates and timings against the student's official ICAI admit card before relying on them.

## Technical note
The live timer is implemented in JavaScript and persists its start timestamp. The displayed elapsed time recalculates when the app returns to the foreground. iOS may pause background page execution, but the recorded elapsed duration remains correct.
