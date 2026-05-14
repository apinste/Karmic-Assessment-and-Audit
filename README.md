# Tranquil Edge Retreat

Pre-retreat reflection materials for a four-day Filipino Martial Arts retreat held September 10 to 13, 2026, at River Mountain, PA. The retreat is run for seven participants. The FMA training is the spine of the retreat. The reflection work is preparation.

This repository contains two web apps and a participant workbook. The web apps are designed to deploy to GitHub Pages with no build step.

## Repository layout

```
.
├── apps/
│   ├── kalooban-quiz/     # Pre-retreat inventory (swipe app, emails results)
│   └── karmic-audit/      # Private audit app (no submission)
├── workbook/              # Participant workbook .docx files
├── index.html             # Landing page that links to the two apps
└── PROJECT_NOTES.md       # Internal project notes
```

## The two apps

### `apps/kalooban-quiz/`. Pre-retreat inventory.

A swipe-style reflection. Fifty-six recognition statements across seven domains. Participants tap or swipe through, receive a brief reveal at the end, and email their result to the facilitators. Progress is saved to their browser so they can leave and return.

See `apps/kalooban-quiz/README.md` for deployment and configuration.

### `apps/karmic-audit/`. Private audit.

A deeper companion to the inventory. Eight open-ended questions per domain across seven domains. Nothing is submitted. The participant can use the web app, which auto-saves to their browser, or print a blank version to fill by hand. The audit is private by design.

See `apps/karmic-audit/README.md` for deployment and configuration.

## Deploying to GitHub Pages

1. Push this repository to GitHub.
2. Go to Settings, then Pages.
3. Under Source, choose "Deploy from a branch." Set branch to `main` and folder to `/ (root)`. Save.
4. Wait one or two minutes. The site will be live at `https://<your-username>.github.io/<repo-name>/`.
5. The root URL shows the landing page. The two apps are reachable at `/apps/kalooban-quiz/` and `/apps/karmic-audit/`.

## Configuration

Before you publish, open each app's `index.html` and edit the configuration block near the top of its `<script>` tag. Both apps share these dates:

```javascript
const RELEASE_DATE = new Date('2026-06-01T00:00:00');
const DUE_DATE = new Date('2026-08-31T23:59:59');
const RETREAT_DATE = new Date('2026-09-10T00:00:00');
```

The inventory app also has `FACILITATOR_EMAIL`, which is the address that receives participant results. The audit app has no submission and no facilitator email.

Each app uses its own `STORAGE_KEY` for localStorage, so the two apps can be hosted on the same domain without their saved state interfering.

## Voice and posture

The retreat materials follow a locked voice. Direct, no wellness clichés, no promises of transformation, no em-dashes anywhere. Before shipping any edit, search the file for the em-dash character (Unicode U+2014). The count should be zero. See `PROJECT_NOTES.md` for the full list of banned phrases and the reasoning behind the posture.

## Workbook

The `workbook/` folder contains the printable participant workbook as `.docx` files. They are built with the `docx` npm package but are easiest to edit directly in Word or LibreOffice for small changes. The aesthetic matches the web apps: Garamond, ember and gold accents, diamond ornaments, cream paper feel.

## License

These materials were written for the Tranquil Edge Retreat and its facilitators. Reuse outside that context should be cleared with the project owner.
