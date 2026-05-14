# Tranquil Edge Retreat · Karmic Audit

A private audit tool for participants to use before the retreat. Eight open-ended questions per domain, seven domains. The audit is private. Nothing is sent.

This is a companion to the inventory app (the swipe-style reflection). The inventory gives a fast read and sends results to the facilitators. This audit is the deeper companion. It stays with the participant.

## What this is

A single-page HTML application. No build step, no server, no dependencies. Just `index.html` hosted anywhere that serves static files.

The participant has two paths:

**Use the web app.**
1. Welcome screen
2. Pick one of seven domains
3. Write through eight questions for that domain (auto-saves to their browser as they type)
4. Review what they wrote
5. Mark the domain complete
6. Print what they wrote, save as a text file, or just close the tab
7. Return another day to audit a different domain if they want

**Print blank to fill by hand.**
1. Welcome screen
2. Click "Print blank to fill by hand"
3. Browser opens print dialog with a clean printable layout: all seven domains, all 56 questions, writing lines between each
4. They print it, fill it in with a pen, bring it to the retreat or keep it at home

Both paths produce the same outcome: the participant has their own audit, written by them, kept by them. No data leaves their device.

## Deploying to GitHub Pages

Same approach as the inventory app.

1. Create a new repository on GitHub. Public or private both work for Pages.
2. Add `index.html` to the root.
3. Settings, then Pages. Source: deploy from branch. Branch: `main`, folder: `/ (root)`. Save.
4. Wait one to two minutes. The site goes live.
5. Send the URL to participants.

## Before you deploy

Edit the configuration block at the top of the `<script>` tag in `index.html`.

```javascript
const RELEASE_DATE = new Date('2026-06-01T00:00:00');
const DUE_DATE = new Date('2026-08-31T23:59:59');
const RETREAT_DATE = new Date('2026-09-10T00:00:00');
const STORAGE_KEY = 'tranquil-edge-audit-v1';
```

No facilitator email is configured because nothing is sent. The audit is private by design.

The `STORAGE_KEY` is different from the inventory app's key, so the two apps can live on the same domain without their saved state interfering.

## Privacy

This is the central feature, not a footnote.

- The app stores progress in the participant's browser using localStorage.
- Nothing is uploaded anywhere. There is no server.
- No analytics, no tracking, no third-party scripts.
- The participant can clear their own browser storage at any time.
- The audit is not submitted, not emailed, not shared.

The welcome and several other screens reinforce this directly so participants understand it before they begin writing.

## The eight questions per domain

Original to this work, written in the voice of the retreat: direct, inclusive of the group's mixed situations (married, single, adopted, salaried, business-owner), without wellness clichés.

To edit the questions, find the `DOMAINS` array at the top of the `<script>` tag. Each domain has a `questions` array you can edit.

## Testing locally

Open `index.html` in any browser. Walk through both paths. Try the print dialog to see the printable blank layout.

To clear progress between tests:

```javascript
localStorage.clear()
```

Run that in the browser console, then reload.

## Browser support

Tested on recent Chrome, Firefox, Safari, and Edge. Uses standard ES6, localStorage, and the browser's native `window.print()`. No transpilation, so very old browsers may have issues.

## What is in this folder

- `index.html`. The application.
- `README.md`. This file.

## Difference from the inventory app

| Feature | Inventory (swipe) | Audit (this app) |
|---|---|---|
| Submission | Email to facilitators | None |
| Identity required | First name + email | No identity needed |
| Length | 10-15 minutes | 30-60 minutes per domain |
| Format | 56 yes/sometimes/no/idk cards | Eight open-ended questions per domain |
| Frequency | Done once | Done one domain at a time, over weeks |
| Privacy | Result shared with facilitators | Strictly private |
| Print option | No | Yes, for filling by hand |
