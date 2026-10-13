# custom-apps

Small, self-contained web apps. Each one is a single HTML file with no build step and no dependencies.

## Apps

### Day Blocks: `day-planner/`

A daily time-blocking planner styled after Apple Calendar's day view, in black, white and orange. Works on desktop and phone.

- **Create a block:** drag on empty time, click or tap an empty slot (1 hour), press `N`, or use the orange **+** button on a phone.
- **Move it:** drag the block (press and hold on a phone). **Resize it:** drag its bottom edge. Times snap to 15 minutes.
- **Edit it:** click the block to change the task, times, type, repeat, priority star or note.
- **Repeat:** never, every day, weekdays, weekly, or custom days. Editing or deleting a repeating block asks whether the change applies to *only this day* or *this and future days*. Dragging one changes that day only, with a one-tap *All future days* option.
- **Types:** Work (solid orange), School (black/white), Faith (orange tint), Personal (gray), Buffer (hatched). Rename them in Settings. ★ Priority is a separate flag you can put on any block.
- **Sleep schedule:** set wake-up and bedtime in Settings. Night hours fold away (with a button to show them), the day opens at wake-up, and the summary counts awake hours only.
- **Prayer times:** turn on in Settings to add Fajr, Dhuhr, Asr, Maghrib and Isha to every day. Times are calculated on the device for the chosen location (Raleigh, Cary, Chapel Hill, Durham, Charlotte, New York or custom coordinates), method (ISNA by default) and Asr school. Each shows its window, a tap marks it prayed, and the summary tracks x/5 prayed.
- **Read your day at a glance:** hours planned of hours awake, blocks done, priorities left, what's on now and next, next prayer, and a bar showing time by type.
- **Plan ahead:** week strip, `←` `→`, or swipe sideways on a phone. An empty day offers to copy the previous day's blocks.
- Light, dark or system appearance.

The first launch shows an example day. Click **Clear examples** to start fresh.

**Where data lives:** blocks save in the browser's local storage on that device. When the app runs as a claude.ai artifact, blocks, repeats, prayer check-offs and settings also sync across every device signed in to the same Claude account.

## Running the apps

- **Locally:** open `day-planner/index.html` in any modern browser.
- **GitHub Pages:** in the repo, go to **Settings → Pages**, set **Source** to "Deploy from a branch", and choose `main` / `(root)`. The planner is then served at `https://<user>.github.io/custom-apps/day-planner/`.
- **iPhone home screen:** open the hosted URL in Safari, then tap **Share → Add to Home Screen**. It opens full-screen like an app.
