# Tranquil Edge Retreat — Project Notes

## What this project is

Custom retreat materials for **Tranquil Edge Retreat**, a 4-day Filipino Martial Arts retreat with karmic reflection work added in 2026 for the first time.

- **Dates:** September 10–13, 2026
- **Venue:** River Mountain at Sweet Root Creek, 3600 Black Valley Rd, Everett, PA 15537
- **Participants:** 7 (3 women, 4 men, separate pods)
- **Group mix:** Married long-term, dating, single, divorced. Salaried and business owners. One participant is adopted and does not know his biological family. All Western participants. Facilitators are Filipino but do not claim indigenous authority.

The FMA is the spine of the retreat. The karmic work is preparation, not the main event.

---

## Live deployment

- **GitHub repo:** `apinste/Karmic-Assessment-and-Audit` (public)
- **Repo URL:** https://github.com/apinste/Karmic-Assessment-and-Audit
- **GitHub Pages live root:** https://apinste.github.io/Karmic-Assessment-and-Audit/
- **Custom domain:** not yet wired. User will provide a subdomain (e.g. `pre-retreat.<theirsite>.com`); CNAME file goes in repo root, custom domain set in repo Settings → Pages, DNS configured at their provider.

App URLs:

- Landing: https://apinste.github.io/Karmic-Assessment-and-Audit/
- Inventory: https://apinste.github.io/Karmic-Assessment-and-Audit/apps/kalooban-quiz/
- Audit: https://apinste.github.io/Karmic-Assessment-and-Audit/apps/karmic-audit/
- Letter: https://apinste.github.io/Karmic-Assessment-and-Audit/apps/letter-to-self/

---

## The karmic reset arc (5 phases)

The whole journey, mapped. Each phase has retreat activities that serve it.

1. **Assessment.** See what is there. Inventory + audit (pre-retreat web apps).
2. **Acknowledgement and clearing.** Stop arguing with what is true. Karmic teaching, sound bath, body work, Inner Workshops Part 1 and 2 (Day 1–2 of retreat).
3. **Letting go.** Give the pattern to the fire. Letter to self **written pre-retreat** via the web app, brought to retreat, burned at the fire on Day 3 evening.
4. **Claiming.** Take up what is yours. Batok workshop on practice skin pads, Saturday evening at the fire. Group session, ~1 hour.
5. **Integration.** Carry it home. Seven domain rituals + weekly check-in + Sunday closing.

**CRITICAL:** Do NOT preview retreat content (Day 3 fire ritual, batok, claiming phase, integration phase) in the pre-retreat web apps. Participants discover those at the retreat. Cross-links may say "the letter comes after the audit" but not "you will burn it at the fire on Day 3."

---

## Voice and posture (locked)

Apply this everywhere user-facing. Verify before shipping any new content.

- Direct. No wellness clichés.
- **Banned phrases:** "hold space," "trust the process," "your truth," "manifest," "abundance," "limiting beliefs," "soul contracts."
- **No em-dashes anywhere in user-facing files.** Search with `grep -c "—" file.html` — must return 0. (PROJECT_NOTES is internal; em-dashes ok here.)
- Complete human sentences. No fragments. No clipped one-liner style.
- No promises of transformation. No three-night-reset language.
- Treat participants as adults who can handle truth.
- Core posture: *"We are not here to fix anything. We do not assume there is anything to fix."*
- Karma is acknowledged as a Sanskrit word that has traveled. Used because recognizable, not claimed as ours.
- Not a Filipino indigenous claim. Not Western positive thinking. Honest reflection in plain language.
- FMA is the spine. The karmic work prepares the warrior side.

**For prompts in the Letter to Self app specifically:**

- Prompts must invite reflection, not direct or instruct.
- No length caps ("in one or two sentences"), no style commands ("Direct. No softeners.", "Be specific.").
- People are processing real and often heavy material. Tone is respectful and understanding.
- Questions should sit as questions a thoughtful friend would ask, not tasks to complete.

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

## Retreat schedule (mapped to phases)

**River Mountain at Sweet Root Creek** · 3600 Black Valley Rd, Everett, PA 15537. Check-in 3pm Thursday Sept 10. Check-out 11am Sunday Sept 13.

Warrior sessions are locked (the bulk of the event). Other slots reorganized to follow the karmic reset arc.

**Thursday, September 10 — Phase 1 + 2 begin (Assessment + Acknowledgement)**

- 3:00–3:30 Check In
- 3:30–5:30 **Warrior Movement Workshop, Introduction** (locked)
- 5:30–6:00 River Mountain Orientation
- 6:00–7:00 Dinner
- 7:00–8:00 **Warrior Inner Workshop, Part 1** (locked) — karmic teaching, name the one karma you are bringing to the fire on Saturday
- 8:00–9:00 **Sound Bath** — clearing what was named

**Friday, September 11 — Phase 2 deepens (Acknowledgement and Clearing)**

- 7:30–8:30 Single Stick Flow (Arnis Yoga)
- 9:30–12:00 **Warrior Movement Workshop, Part 1** (locked)
- 1:00–5:00 **Warrior Movement Workshop, Part 2** (locked)
- 5:00–6:00 Rest
- 7:00–9:00 **Warrior Inner Workshop, Part 2** (locked)
- 9:00–9:45 Stargazing Meadow Ceremony (post-workshop, weather permitting)

**Saturday, September 12 — Phase 3 + 4 (Letting Go + Claiming)**

- 7:30–8:30 Single Stick Flow
- 9:30–12:00 **Warrior Movement Workshop, Part 3** (locked)
- 1:00–3:00 **Warrior Movement Workshop, Part 4** (locked)
- 3:00–4:30 Philippine Cultural Studies — frames batok and lineage
- 4:30–6:00 **Nature Walk → Fire → Letter Burning** (Letting Go)
- 6:00–7:00 Dinner
- 7:00–8:00 Campfire Sessions — sit with what was released
- 8:00–9:00 **Batok Workshop on practice skin pads** (group, simultaneous, ~1 hour) — Claiming

**Sunday, September 13 — Phase 5 (Integration)**

- 7:30–8:30 Sacred Wellness
- 9:30–11:00 **Pekiti Tirsia Kali Theories + Closing** — name one ritual you will start on Monday
- 11:00 Check Out

**Naming:**

- *Warrior Movement Workshops* = FMA training
- *Warrior Inner Workshops* = karmic teaching/audit slots
- *Nature walk* = ends at fire in woods, letter-burning happens there
- *Campfire Sessions* = sit with the fire after the release ritual
- *Batok Workshop* = Filipino tattoo tradition on practice pads (not body marking). Group session, claiming gesture, ~1 hour. Tools: skin pads provided.

---

## Letter ritual design (final)

- Each participant **writes a private letter to themselves** about their own pattern. No ancestors in the letter (ancestors are honored at the tattoo session).
- **Written pre-retreat** via the Letter to Self web app, with a guided fill-in-the-blank template. Can be revised as many times as desired before arrival.
- They bring the printed letter (or text file) to the retreat.
- Burned at fire in woods at end of nature walk on Day 3 evening.
- Participants choose their own moment to burn it. Fire stays lit through the night. No group clock.
- Facilitators available in one room with tea, non-asymmetric so visiting doesn't signal struggle.
- No sharing required. Removes ego/performance.

---

## Deliverables shipped

### Web apps (live on GitHub Pages)

**Landing page** — `index.html` at repo root

- Three cards (numbered One/Two/Three) linking to inventory, audit, letter
- Same visual aesthetic as the apps
- Footer: River Mountain location and dates

**`apps/kalooban-quiz/`** — Pre-Retreat Inventory (swipe app)

- 56 cards across 7 domains, swipe yes/sometimes/not-me/don't-know
- Header: "Tranquil Edge Retreat" / "Pre-Retreat Reflection"
- Welcome → identity (name + email) → **Arrive First** (guided breathing visual + 60s ocean audio prep) → swipe → reveal → share
- **Privacy note** on welcome screen explains: browser-only save, results shared only when participant clicks Send
- Reveal: top karma type + top domain + breakdowns
- Share: choose summary-only or full result
- Submits via mailto to **trainpekiti@gmail.com**
- Cross-links to audit and letter on welcome and post-completion screens

**`apps/karmic-audit/`** — Private Audit App

- 8 open-ended questions per domain, 7 domains
- **No submission. No facilitator email. Strictly private.**
- Two paths: web app (auto-saves to browser) or print blank to fill by hand
- Print speed optimized: 400ms timeout removed, double-rAF + busy indicator toast on click
- **Print tip** on print-prep screen: tells participants to uncheck "Headers and footers" in browser print dialog so URL doesn't show on each page (mitigates github.io URL appearing on printouts until custom domain is wired)
- Question text upright Garamond (was italic, hard to read)
- Cross-links to inventory and letter on welcome and post-completion screens

**`apps/letter-to-self/`** — Letter to Self app (added this session)

- Guided letter-writing app. Participant writes pre-retreat, brings to retreat.
- Welcome → optional Arrive First (breathing + ocean prep, skippable) → Write (inline letter template) → Done (print/save)
- The Write view IS the letter: name input as inline blank in "Dear ___,", seven prompts as prose lead-ins each followed by a dashed-bottom-border textarea. Closes with "Love,\n[name]" — signature updates live as user types name.
- Auto-saves each blank to browser as participant types
- Print/save composes the letter cleanly: greeting, prose lead-ins, answers, "Love, [name]" signoff
- Migration from older single-textarea draft handled
- Includes phase teaching but **no retreat-content spoilers** (no Day 3, fire, batok, claiming, integration mention)
- Prompts are invitational, not prescriptive

### Cross-app conventions (in all three apps)

- **Topbar brand "◆ Tranquil Edge Retreat"** is a clickable home link to the landing page (`../../`). Hover changes color to ember. Auto-save means leaving mid-flow loses no progress; participants can return to the same URL.
- **Custom in-app modal** replaces every browser-native `confirm()` and `alert()`. Native dialogs always show "apinste.github.io says: ..." which we want to hide. Modal is a styled card on a dimmed blurred backdrop, ember accent border, two buttons. Backdrop click and Escape cancel; Enter confirms.
- **Marcellus SC** is the small-caps font (replaced Cormorant SC, which was too thin at small sizes on the dark ground).
- **`--paper-faded` brightened** from `#8a8273` / `#6d6859` to `#c0b6a0` for stronger contrast on small text.
- Header sizes 0.8 → 0.92rem, footer 0.7 → 0.85rem, letter-spacing tightened from 0.3em to 0.18em across all apps.

### Audio asset

- **`apps/kalooban-quiz/audio/waves-60s.mp3`** and **`apps/letter-to-self/audio/waves-60s.mp3`** — 60-second ocean clip, ~720KB, 96kbps mp3 stereo
- Source: Wikimedia Commons File:Waves.ogg (public domain, recorded on Lake Ontario shore by user Dsw4)
- Trimmed and faded with ffmpeg (`-ss 30 -t 60`, 2s fade in, 3s fade out)
- See `audio/CREDITS.md` in each app folder
- Both copies must be replaced together if the audio is swapped

### Workbook sections (.docx files in `workbook/`)

All use the same visual aesthetic: Garamond font, ember (#c4773a) and gold (#9a7a40) accents, cream paper feel, diamond ornaments, US Letter, 1.125" margins.

- **Tranquil-Edge-Karmic-Audit-Worksheet.docx** — 84-question audit (structurally close to source, see boundary note)
- **Tranquil-Edge-Letter-To-Self.docx** — 8 pages. Cover, framing with optional starter prompts, 6 lined writing pages. Originally meant for tear-out; now superseded by the Letter to Self web app for most participants.
- **Tranquil-Edge-Under-The-Stars-Teaching.docx** — Facilitator stargazing teaching. Built before stargazing's role shifted to a brief weather-permitting close to Friday night; may need repurposing.
- **Tranquil-Edge-Inner-Workshop-Part-One.docx** — 5 pages. Cover, **karma teaching placeholder** (lead facilitator writes), posture page, 4-day shape, notes space.
- **Tranquil-Edge-Inner-Workshop-Part-Two.docx** — 6 pages. Cover, what tonight is for, **audit-debrief teaching placeholder**, how the evening moves, posture reminders, bridge to letter.
- **Tranquil-Edge-Notes-Section.docx** — 8 pages. Light category labels (From the sessions, Things to remember, Questions, To carry home, Notes).
- **Tranquil-Edge-After-The-Retreat.docx** — 18 pages. Cover, what this is, first week home + writing space, **integration teaching placeholder**, returning to your audit, the slow drift, weekly check-in question, **seven domain rituals** (one page each), closing, writing space.

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

1. **Custom domain on GitHub Pages** — User to provide subdomain (e.g. `pre-retreat.<theirdomain>.com`). Add CNAME file at repo root, configure in repo Settings → Pages, set DNS at their domain provider. Removes "github.io" from URLs and from browser-printed page headers.
2. **Section 6: Letter pages integration** — Letter-to-Self standalone .docx exists; needs section divider/renumbering to fit workbook flow. May skip if the web-app letter replaces the printed page for all participants.
3. **Section 7: Philippine Cultural Studies wrapper** — 3-5 pages, cover + placeholders for tattoo / batok teaching (lead facilitator writes), structured space for participant reflection.
4. **Front matter** — Cover for whole workbook, table of contents, welcome page, schedule at a glance (4-5 pages). User said they will handle workbook title later.
5. **Possible voice update** — `Pag-aayos-ng-Kalooban-Facilitator-Guide.docx` and `Pag-aayos-ng-Kalooban-Student-Workbook.docx` (from earlier work) may need alignment with new voice/posture and the no-spoiler convention.
6. **Workbook front matter on five-phase arc** — Optional one-page handout describing the five phases and how they map to the schedule. Content already drafted in conversation, can be turned into a .docx page or website page next session.

---

## Tech stack

- **HTML apps:** Vanilla JS, no framework, no build step. Single `index.html` per app. Pointer events for swipe gestures. CSS transitions for animations.
- **Fonts:** Cormorant Garamond (display), Lora (body), **Marcellus SC** (small caps — replaced Cormorant SC for legibility on dark backgrounds at small sizes). Imported from Google Fonts in CSS.
- **Visual aesthetic:** Dark navy background (#0a0a0c, #14141a), warm paper text (#e8e2d5), ember accent (#c4773a, #d4884a), gold accents (#9a7a40, #c4a560), brighter paper-faded (#c0b6a0) for small text.
- **In-app modal pattern:** Custom modal replaces native `confirm()` / `alert()` so the github.io URL never appears in dialogs. Lives in each app file. Promise-based, supports backdrop click + Escape (cancel) and Enter (confirm).
- **Print busy indicator:** Toast appears immediately on print click. Replaces the old 400ms timeout with a double-rAF chain so the dialog opens fast with visible feedback.
- **docx files:** Built with docx-js (`docx` npm package). Easier to edit the `.docx` directly in Word/LibreOffice if it's a small change. Build scripts not yet in repo.
- **docx writing lines:** Built as tables with single row and bottom border. Avoids border-merging issue from consecutive bordered paragraphs.

---

## Configuration values used

```javascript
// In all three web apps
const RELEASE_DATE = new Date('2026-05-14T00:00:00');  // currently open
const DUE_DATE = new Date('2026-09-09T23:59:59');      // day before retreat
const RETREAT_DATE = new Date('2026-09-10T00:00:00');

// Inventory app only
const FACILITATOR_EMAIL = 'trainpekiti@gmail.com';
const STORAGE_KEY = 'tranquil-edge-reflection-v1';

// Audit app only
const STORAGE_KEY = 'tranquil-edge-audit-v1';

// Letter app only
const STORAGE_KEY = 'tranquil-edge-letter-v1';
```

Each `STORAGE_KEY` is unique so the three apps do not collide on localStorage when hosted on the same domain.

---

## When refining

- All three web apps are single-file HTML. Open in any editor / browser as static files. Live preview works.
- The `CARDS` array (inventory), `DOMAINS` array (audit), and `FIELDS` + `LETTER_INTROS` (letter) are the easiest things to edit. Each is at the top of the `<script>` tag.
- The `:root` CSS variable block controls all colors. Change one, everything updates.
- Before shipping any edit, run two checks:
  - `grep -c "—" path/to/index.html` — must return 0 (no em-dashes)
  - `grep -ciE "hold space|trust the process|your truth|manifest|abundance|limiting beliefs|soul contracts" path/to/index.html` — must return 0 (banned phrases)
- For .docx files, you'll need to rebuild from source `.js` files in Node with the docx-js library if you want programmatic changes. Simpler to edit the `.docx` directly in Word/LibreOffice for small changes.
- The visual design language is consistent across HTML apps and docx files. Same colors, same fonts, same diamond ornaments. Maintain this when adding new pieces.

---

## File structure

```
karmic-reset-bundle/
├── index.html                    # Landing page (3 cards)
├── README.md                     # Repo-level README
├── PROJECT_NOTES.md              # This file
├── .gitignore
├── apps/
│   ├── kalooban-quiz/            # Inventory app (swipe, submits to email)
│   │   ├── index.html
│   │   ├── README.md
│   │   └── audio/
│   │       ├── waves-60s.mp3
│   │       └── CREDITS.md
│   ├── karmic-audit/             # Private audit app (no submission)
│   │   ├── index.html
│   │   └── README.md
│   └── letter-to-self/           # Letter to Self app (private, guided)
│       ├── index.html
│       ├── README.md
│       └── audio/
│           ├── waves-60s.mp3     # duplicated from inventory for self-containment
│           └── CREDITS.md
└── workbook/                     # Participant workbook .docx files
    ├── Tranquil-Edge-Inner-Workshop-Part-One.docx
    ├── Tranquil-Edge-Inner-Workshop-Part-Two.docx
    ├── Tranquil-Edge-Letter-To-Self.docx
    ├── Tranquil-Edge-Notes-Section.docx
    ├── Tranquil-Edge-After-The-Retreat.docx
    ├── Tranquil-Edge-Karmic-Audit-Worksheet.docx
    └── Tranquil-Edge-Under-The-Stars-Teaching.docx
```

---

*Last updated: end of session, May 14, 2026 (commit `ab36f3c` — modal + home link added). Repo is at `apinste/Karmic-Assessment-and-Audit`, live on GitHub Pages.*
