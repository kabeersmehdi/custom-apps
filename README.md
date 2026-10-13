# custom-apps

Small, self-contained web apps. Each one is a single HTML file with no build step and no dependencies.

## Apps

### Day Blocks: `day-planner/`

A daily time-blocking planner styled after Apple Calendar's day view, in black, white and orange.

- **Create a block:** drag on empty time, click an empty slot (1 hour), or press `N`.
- **Move it:** drag the block. **Resize it:** drag its bottom edge. Times snap to 15 minutes.
- **Edit it:** click the block to change the task, times, type, notes, or mark it done.
- **Types:** Priority (solid orange), Work (orange tint), Personal (black/white), Buffer (hatched gray).
- **Read your day at a glance:** hours planned, blocks done, what's on now and what's next, and a bar showing time by type.
- **Plan ahead:** use the week strip or `←` `→`. An empty day offers to copy the previous day's blocks.
- **On a phone:** tap empty time to add a block, tap a block to edit it, and press and hold a block to move it.
- Light and dark mode follow your system; the moon/sun button overrides it.

The first launch shows an example day. Click **Clear examples** to start fresh.

**Where data lives:** blocks save in the browser's local storage on that device. When the app runs as a claude.ai artifact, it also syncs across every device signed in to the same Claude account.

## Running the apps

- **Locally:** open `day-planner/index.html` in any modern browser.
- **GitHub Pages:** in the repo, go to **Settings → Pages**, set **Source** to "Deploy from a branch", and choose `main` / `(root)`. The planner is then served at `https://<user>.github.io/custom-apps/day-planner/`.
- **iPhone home screen:** open the hosted URL in Safari, then tap **Share → Add to Home Screen**. It opens full-screen like an app.
