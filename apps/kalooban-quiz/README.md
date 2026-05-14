# Tranquil Edge Retreat · Pre-Retreat Reflection

A single-page swipe-style reflection app for participants to complete before the retreat. No build step, no server, no dependencies. Just a single `index.html` file you can host anywhere that serves static files.

This README covers deploying to GitHub Pages, which is the simplest free option.

## What this is

Fifty-six recognition statements across seven domains. Participants swipe or tap through them, get a brief reveal at the end, and send their result to the facilitators by email. Their progress is saved to their browser between sessions so they can leave and return.

## Deploying to GitHub Pages

1. **Create a new repository** on GitHub. Public or private both work for Pages; public is free, private requires GitHub Pro or Team.

2. **Add `index.html`** to the root of the repository. That is the only file required.

3. **Go to Settings, then Pages.** Under "Source," choose "Deploy from a branch." Choose your default branch (usually `main`) and folder `/ (root)`. Click Save.

4. **Wait one or two minutes.** GitHub will build and publish the site. The URL will be something like `https://yourusername.github.io/your-repo-name/`.

5. **Send that URL** to participants when you are ready.

## Before you deploy

Open `index.html` in any text editor and edit the configuration block at the top of the `<script>` tag. The settings are:

```javascript
const FACILITATOR_EMAIL = 'facilitator@example.com';
const RELEASE_DATE = new Date('2026-06-01T00:00:00');
const DUE_DATE = new Date('2026-08-31T23:59:59');
const RETREAT_DATE = new Date('2026-09-10T00:00:00');
const STORAGE_KEY = 'tranquil-edge-reflection-v1';
```

**`FACILITATOR_EMAIL`**. Where participant results are sent. When a participant clicks "Send to Facilitators," their email client opens with the result pre-filled, addressed to this email.

**`RELEASE_DATE`**. Before this date, the welcome screen shows "Opens [date]" and the Begin button is disabled.

**`DUE_DATE`**. After this date, the welcome screen notes the window has closed, but participants can still complete the reflection if they want to.

**`RETREAT_DATE`**. Used in the closing message. Not strictly required but lets the app reference the retreat date naturally.

**`STORAGE_KEY`**. The localStorage key used to save participant progress. Bump the version number (`v1` to `v2`) if you want existing participants to start fresh.

## How submission works

When a participant clicks "Send to Facilitators," the page opens a `mailto:` link with the result pre-filled in their default email client. The participant sees the email before sending and can review or edit. They click send. You receive the email at the address you configured.

This is the simplest approach. A few characteristics worth knowing:

- The participant needs a working email client configured on their device. On phones this is usually fine. On laptops without a desktop mail app, the link may open a webmail compose window or do nothing.
- Participants choose between "summary only" and "full result." Either way, the email is the delivery mechanism.
- There is no database. Results live in the emails you receive.

If you want a more robust setup later, replace the `submitShare` function with a `fetch()` call to a Google Sheets webhook, a Google Form endpoint, or a service like Formspree. The data structure is already built (see `buildSummary` in the source).

## Privacy

The app stores progress in the participant's browser using localStorage. Nothing is uploaded anywhere until the participant clicks "Send to Facilitators," and even then, only the participant's own email client transmits the data. There is no analytics, no tracking, no third-party scripts.

The submission email contains the participant's name, email, completion timestamp, top karma type, top domain, and weighted breakdowns by type and domain. If the participant chose "Share full result," the email also includes their answer to each card. Otherwise, individual card answers stay on their device.

## Testing locally

Open `index.html` in any browser. That is it. The app runs entirely client-side. You can swipe through, complete the flow, and watch what happens when you click Send. (The email client will open with the message pre-filled.)

To test the pre-release state, change `RELEASE_DATE` to a date in the future. To test the post-due state, change `DUE_DATE` to a date in the past.

## Resetting between tests

To clear your progress and start fresh, open the browser's developer console and run:

```javascript
localStorage.clear()
```

Then reload the page.

## Customizing

The 56 cards are defined in the `CARDS` array near the top of the `<script>` tag. Each card has an `id`, `domain`, `type` (personal, ancestral, or collective), and `text`. To edit, add, or remove cards, edit that array.

The visual design uses CSS custom properties at the top of the `<style>` block. Colors, fonts, and spacing are all there.

## Browser support

Tested on recent versions of Chrome, Firefox, Safari, and Edge. Uses standard ES6, pointer events, and localStorage. No build step means no transpilation, so very old browsers (pre-2018) may have issues.

## What is in this folder

- `index.html`. The application. Single file, no dependencies.
- `README.md`. This file.
