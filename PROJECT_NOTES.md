# Tranquil Edge Retreat — Project Notes

## What this project is

Custom retreat materials for **Tranquil Edge Retreat**, a 4-day Filipino Martial Arts retreat with karmic reflection work added in 2026 for the first time.

- **Dates:** September 10–13, 2026
- **Location:** River Mountain, PA
- **Participants:** 7 (3 women, 4 men, separate pods)
- **Group mix:** Married long-term, dating, single, divorced. Salaried and business owners. One participant is adopted and does not know his biological family. All Western participants. Facilitators are Filipino but do not claim indigenous authority.

The FMA is the spine of the retreat. The karmic work is preparation, not the main event.

---

## Voice and posture (locked)

Apply this everywhere. Verify before shipping any new content.

- Direct. No wellness clichés.
- **Banned phrases:** "hold space," "trust the process," "your truth," "manifest," "abundance," "limiting beliefs," "soul contracts."
- **No em-dashes anywhere.** Search the file with grep before shipping. `grep -c "—" file.html` should return 0.
- Complete human sentences. No fragments. No clipped one-liner style.
- No promises of transformation. No three-night-reset language.
- Treat participants as adults who can handle truth.
- Core posture: *"We are not here to fix anything. We do not assume there is anything to fix."*
- Karma is acknowledged as a Sanskrit word that has traveled. Used because recognizable, not claimed as ours.
- Not a Filipino indigenous claim. Not Western positive thinking. Honest reflection in plain language.
- FMA is the spine. The karmic work prepares the warrior side.

---

## Critical copyright/sourcing boundary

The user owns a 557-page karmic reset source book. **Do not reproduce or paraphrase its framework into deliverables.** This means:

- Do not build assessments that mirror the source's 7-domain × 12-question audit structure with paraphrased questions
- Do not build sections that walk through the source's 7-step protocol (See, Own, Feel, Understand, Amends, Choose, Walk Forward), even with rewording
- Do not include the source's specific resolution lines per karma type
- Do build wrapper documents with placeholder pages where the lead facilitator writes karma teaching from their sources
- Do write original ritual structures drawing on widely-known contemplative practices (mirror practice, candle for ancestors, weekly review, etc.)
- Do write original assessment prompts that don't map 1-to-1 to the source's questions

The Karmic Audit Worksheet (Tranquil-Edge-Karmic-Audit-Worksheet.docx) was built earlier in the project before this boundary was clear. It's structurally close to the source. User has it and may keep it as-is, but new work should not follow that pattern.

---

## Retreat schedule (confirmed)

- **Day 1 (half day):** Afternoon arrival + 2 night sessions. **Sound bath** is one of the night sessions (the big clearing piece, do this on Day 1)
- **Day 2 (full day):** FMA training + 2 night sessions. Group binding circle. Tattoo session (or stargazing storytelling)
- **Day 3 (full day):** FMA training + 2 night sessions. **Warrior Inner Workshop** (audit work). Nature walk to fire for letter-burning ritual
- **Day 4:** Morning FMA + short closing + breakfast + departures

**Naming:**
- *Warrior Movement Workshops* = FMA training
- *Warrior Inner Workshops* = karmic teaching/audit slots
- *Nature walk* = ends at fire in woods, letter-burning happens there
- *Stargazing* = usually storytelling, completely dark. Optional light karmic-themed story prompt
- *Tattoo session* = Filipino tattoo tradition. Honors lineage gifts. Separate from karmic release (release is for loops; tattoo is for claiming)

---

## Letter ritual design (final)

- Each participant writes a private letter **to themselves** about their own pattern. No ancestors in the letter (ancestors are honored at the tattoo session).
- No sharing required. Removes ego/performance.
- Burned at fire in woods at end of nature walk on Day 3 evening.
- Participants write in their room or hall, choose their space.
- Facilitators available in one room with tea, non-asymmetric so visiting doesn't signal struggle.
- Fire stays lit through the night. They burn when ready, not on a group clock.

---

## Deliverables shipped

### Web apps (deploy to GitHub Pages)

**`apps/kalooban-quiz/`** — Pre-Retreat Inventory (swipe app)
- 56 cards across 7 domains, swipe yes/sometimes/not-me/don't-know
- Header: "Tranquil Edge Retreat" / "Pre-Retreat Reflection"
- Buttons in order: Don't Know (left) / Not Me / Sometimes / Yes (far right)
- Inclusive language for cards (married/single/divorced/adopted situations)
- Reveal at end: karma teaching + top type + top domain
- Sharing required, participant chooses summary-only vs full-detail
- localStorage for save/resume
- Submits via mailto to **trainpekiti@gmail.com**
- Configuration block at top of `<script>`: FACILITATOR_EMAIL, RELEASE_DATE, DUE_DATE, RETREAT_DATE, STORAGE_KEY

**`apps/karmic-audit/`** — Private Audit App
- 8 open-ended questions per domain, 7 domains
- **No submission. No facilitator email. Strictly private.**
- Two paths: (1) Use the app (writes saved in browser, can print/save when done) or (2) Print blank to fill by hand (all 56 questions with writing lines, browser print)
- No identity required
- localStorage for save/resume
- Configuration block at top of `<script>`: RELEASE_DATE, DUE_DATE, RETREAT_DATE, STORAGE_KEY (different key than inventory)

### Workbook sections (.docx files)

All use the same visual aesthetic: Garamond font, ember (#c4773a) and gold (#9a7a40) accents, cream paper feel, diamond ornaments, US Letter, 1.125" margins.

- **Tranquil-Edge-Karmic-Audit-Worksheet.docx** — 84-question audit (structurally close to source, see boundary note)
- **Tranquil-Edge-Letter-To-Self.docx** — 8 pages. Cover, framing with optional starter prompts, 6 lined writing pages. Tear-out for the fire on Day 3.
- **Tranquil-Edge-Under-The-Stars-Teaching.docx** — Facilitator stargazing teaching. Note: built before stargazing's role shifted; may need repurposing.
- **Tranquil-Edge-Inner-Workshop-Part-One.docx** — 5 pages. Section 4 of workbook. Cover, **karma teaching placeholder** (lead facilitator writes), posture page, 4-day shape, notes space.
- **Tranquil-Edge-Inner-Workshop-Part-Two.docx** — 6 pages. Section 5 of workbook. Cover, what tonight is for, **audit-debrief teaching placeholder**, how the evening moves, posture reminders, bridge to letter.
- **Tranquil-Edge-Notes-Section.docx** — 8 pages. Section 9. Light category labels (From the sessions, Things to remember, Questions, To carry home, Notes).
- **Tranquil-Edge-After-The-Retreat.docx** — 18 pages. Section 8. Cover, what this is, first week home + writing space, **integration teaching placeholder**, returning to your audit, the slow drift, weekly check-in question, **seven domain rituals** (one page each), closing, writing space.

### The seven domain rituals (in After-The-Retreat.docx)

Original compositions. Drawing on widely-known contemplative practice forms, not from source.

1. **Relationships** — Monthly one-sentence about own side of one relationship. Read six in order after six months.
2. **Money & Earning** — Anchored to recurring money moment. One breath before, notice during, name one feeling after.
3. **Health & Body** — Hand on chest + belly, three breaths, ask body one question, listen.
4. **Purpose & Work** — Weekly review on a chosen day. Three questions (what felt mine, what felt borrowed, what small thing moves toward mine).
5. **Family & Ancestry** — Candle or window, one minute acknowledging line behind, no asking.
6. **Self & Identity** — Mirror practice, one minute looking + one true thing said out loud. Then walk away.
7. **Spirit & Connection** — Design own practice, 5 minutes for 30 days.

---

## What's still to build (handoff TODO)

1. **Section 6: Letter pages integration** — Letter-to-Self standalone exists; needs section divider/renumbering to fit workbook flow
2. **Section 7: Philippine Cultural Studies wrapper** — 3-5 pages, cover + placeholders for tattoo teaching (user writes), structured space for participant reflection
3. **Front matter** — Cover for whole workbook, table of contents, welcome page, schedule at a glance (4-5 pages). User said they'll handle workbook title later.
4. **Possible voice update** — Pag-aayos-ng-Kalooban-Facilitator-Guide.docx and Pag-aayos-ng-Kalooban-Student-Workbook.docx (from earlier work) may need alignment with new voice/posture

---

## Tech stack

- **HTML apps:** Vanilla JS, no framework, no build step. Single `index.html` per app. Pointer events for swipe gestures. CSS transitions for animations.
- **Fonts:** Cormorant Garamond (display), Garamond (body), Cormorant SC (small caps). Imported from Google Fonts in CSS.
- **Visual aesthetic:** Dark navy background (#0a0a0c, #14141a), warm paper text (#e8e2d5), ember accent (#c4773a, #d4884a), gold accents (#9a7a40, #c4a560).
- **docx files:** Built with docx-js (`docx` npm package). Easier to edit the `.docx` directly in Word/LibreOffice if it's small changes.
- **docx writing lines:** Built as tables with single row and bottom border. Avoids border-merging issue from consecutive bordered paragraphs.

---

## Configuration values used

```javascript
// In both web apps
const RELEASE_DATE = new Date('2026-06-01T00:00:00');
const DUE_DATE = new Date('2026-08-31T23:59:59');
const RETREAT_DATE = new Date('2026-09-10T00:00:00');

// Inventory app only
const FACILITATOR_EMAIL = 'trainpekiti@gmail.com';
const STORAGE_KEY = 'tranquil-edge-reflection-v1';

// Audit app only
const STORAGE_KEY = 'tranquil-edge-audit-v1';
```

---

## When refining in JetBrains

A few practical notes:

- Both web apps are single-file HTML. Open in WebStorm/PHPStorm/IntelliJ as static files. Live preview in browser works.
- The `CARDS` array (inventory) and `DOMAINS` array (audit) are the easiest things to edit. Each card/question is a one-line addition.
- The `:root` CSS variable block controls all colors. Change one, everything updates.
- Before shipping any edit: `grep -c "—" index.html` should return 0 (no em-dashes).
- For docx files, you'll need to rebuild source `.js` files in Node with the docx-js library if you want to make programmatic changes. Easier to just edit the `.docx` directly in Word/LibreOffice if it's small changes.
- The visual design language is consistent across HTML apps and docx files. Same colors, same fonts, same diamond ornaments. Maintain this when adding new pieces.

---

## File structure

```
Karmic Reset/
├── apps/
│   ├── kalooban-quiz/        # Inventory app (swipe, submits to email)
│   │   ├── index.html
│   │   └── README.md
│   └── karmic-audit/          # Private audit app (no submission)
│       ├── index.html
│       └── README.md
├── workbook/                  # Participant workbook .docx files
│   ├── Tranquil-Edge-Inner-Workshop-Part-One.docx
│   ├── Tranquil-Edge-Inner-Workshop-Part-Two.docx
│   ├── Tranquil-Edge-Letter-To-Self.docx
│   ├── Tranquil-Edge-Notes-Section.docx
│   ├── Tranquil-Edge-After-The-Retreat.docx
│   ├── Tranquil-Edge-Karmic-Audit-Worksheet.docx
│   └── Tranquil-Edge-Under-The-Stars-Teaching.docx
└── PROJECT_NOTES.md           # This file
```

---

*Last updated: project transfer to JetBrains, May 2026*
