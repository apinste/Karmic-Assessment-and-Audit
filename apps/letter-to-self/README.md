# Tranquil Edge Retreat · Letter to Self

A guided letter-writing app for the Letting Go phase of the karmic reset arc. Participants write a private letter to themselves about the pattern they are ready to put down. They bring the printed letter to the retreat and burn it at the fire on Day 3.

## What this is

A four-page single-file HTML application. No build step, no server, no dependencies. Same privacy posture as the audit: nothing is submitted, the letter saves to the participant's browser only.

## The flow

1. **Welcome.** Explains what the letter is, where it fits in the five-phase arc, and why we write it before the retreat. Ends with a Begin button.
2. **Arrive First.** Optional breathing visual and a 60-second ocean sounds clip to slow down before writing. Same components as the inventory app.
3. **Write.** Eight optional starter prompts (collapsible) plus a generous textarea. Auto-saves to localStorage every keystroke.
4. **Done.** Save as text file, print, revise, or close. Includes the next phases (Claiming and Integration) so participants see what comes after.

## Deploying to GitHub Pages

Same as the other apps. Already deployed as part of the parent repo.

## Configuration

```javascript
const RELEASE_DATE = new Date('2026-05-14T00:00:00');
const DUE_DATE = new Date('2026-09-09T23:59:59');
const RETREAT_DATE = new Date('2026-09-10T00:00:00');
const STORAGE_KEY = 'tranquil-edge-letter-v1';
```

`STORAGE_KEY` is unique to this app so it does not collide with the inventory or audit when all three are hosted on the same domain.

## Privacy

No identity required. No facilitator email. Nothing is uploaded. The letter exists only in the participant's browser until they print it or save it as a text file. Clearing browser storage erases the letter.

## Files

- `index.html`. The application.
- `audio/waves-60s.mp3`. Public-domain ocean recording, used by the Arrive First page. Duplicated from the inventory app's audio folder so this app is self-contained. See `audio/CREDITS.md`.
- `README.md`. This file.

## Editing the prompts

The eight starter prompts live in the `PROMPTS` array near the top of the `<script>` tag. Each is a single string. Add, remove, or reword them as you like.
