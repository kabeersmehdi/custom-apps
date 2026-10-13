# custom-apps

Small, self-contained web apps. Each one is a single HTML file with no build step and no dependencies.

## Apps

### Day Blocks: `day-planner/`

A daily time-blocking planner in a quiet, minimalist style: paper white, ink black and one orange, hairline rules, square blocks and serif date numerals. Works on desktop and phone, and installs to an iPhone home screen. The logo is a grey tile with white, orange and black boxes stacked like blocks on a day (`day-planner/icon.svg`, `apple-touch-icon.png`).

- **Create a block:** drag on empty time, click or tap an empty slot (1 hour), press `N`, or use the orange **+** button on a phone. Typing a name like "Lunch" or "Macro class" picks the matching type for you.
- **Move it:** drag the block (press and hold on a phone). **Resize it:** drag its bottom edge. Times snap to 15 minutes.
- **Edit it:** click the block to change the task, times, type, repeat, priority star or note.
- **Repeat:** never, every day, weekdays, weekly, or custom days. Editing or deleting a repeating block asks whether the change applies to *only this day* or *this and future days*. Dragging one changes that day only, with a one-tap *All future days* option.
- **Types:** Work (orange), School (black), Prayer (soft orange), Food (white box), Personal (grey), Buffer (hatched). Rename them in Settings. ★ Priority is a separate flag on any block.
- **Sleep schedule:** set wake-up and bedtime in Settings. Night hours fold away (with a button to show them), the day opens at wake-up, and the summary counts awake hours only.
- **Prayer times:** turn on in Settings to add Fajr, Dhuhr, Asr, Maghrib and Isha to every day, calculated on the device for the chosen location, method (ISNA by default) and Asr school. Each shows its window; tap to mark it prayed.
- **Stats (slides up):** tap or swipe up the **Stats** tab at the bottom, click the bars icon, or press `S`. Shows your average 24 hours over the last 7 days, 30 days or all time, split into sleep, work, school, prayer, food, personal, buffer and unplanned time (to the minute, always totalling 24h and 100%), plus a typical-day strip and how many prayers and blocks you marked done. Drag the handle down to close.
  - A day counts once you plan a timed block for it or check something off; repeating blocks alone don't count a day.
  - Each minute counts once. Where blocks overlap: prayer, then school, work, food, personal, buffer. Sleep comes from the sleep schedule; a prayer that falls during sleep is counted right after waking.
- **Backup / restore:** Settings → Your data → Copy backup, then Restore from backup on another device or copy of the app (for example from claude.ai to the home-screen app).
- **Plan ahead:** week strip, `←` `→`, or swipe sideways on a phone. An empty day offers to copy the previous day's blocks.
- Light, dark or system appearance.

The first launch shows an example day. Click **Clear examples** to start fresh.

**Where data lives:** blocks save in the browser's local storage on that device. When the app runs as a claude.ai artifact, blocks, repeats, prayer check-offs and settings also sync across every device signed in to the same Claude account.

## Running the apps

- **Locally:** open `day-planner/index.html` in any modern browser.
- **GitHub Pages:** Pages on a free GitHub account needs a public repo. In the repo: **Settings → General → Danger Zone → Change visibility → Public**, then **Settings → Pages → Source: Deploy from a branch → Branch: `main`, folder `/ (root)` → Save**. After a minute the planner is live at `https://kabeersmehdi.github.io/custom-apps/day-planner/` and every push to `main` updates it.
- **iPhone home screen:** open that URL in Safari, tap **Share → Add to Home Screen → Add**. It opens full-screen with the Day Blocks icon. Data in the home-screen app stays on that phone; use Settings → Your data to bring in a backup.
