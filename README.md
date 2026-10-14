# Ivan — CV base

A clean, print-ready CV base. Three files, one job each.

| File | What it is |
|------|-----------|
| `cv-content.md` | **Source of truth.** Edit all text here first. Plain, easy to tweak. |
| `cv.html` | The **designed CV**. Open in a browser; it also doubles as a portfolio piece. |
| `README.md` | This file — how to use it + design notes. |

## Export to PDF
1. Open `cv.html` in Chrome.
2. `Cmd+P` → **Save as PDF**.
3. Set margins to *Default*, enable **Background graphics** (keeps the accent bar/box), paper **A4**.
4. It's tuned to land on **one page**. If a section splits awkwardly, trim a bullet.

## Fill the placeholders
Anything in `[ brackets ]` (orange on screen) is a real fact I didn't have from the
handoff — fill it in both files:
- Surname, email
- Bot runtime (Node / Python)
- Start year for the freelance line
- Language levels (Russian / Georgian)

---

## Design advice

You asked for direction, and explicitly **not** the Batumi riso-print / broadsheet
concept. Agreed — that look is a personality statement, and a CV's job is the
opposite: get a busy recruiter or agency lead to "yes" in ~15 seconds. Here's the
thinking baked into `cv.html`, plus options if you want to push it further.

**1. Restraint is the flex.** You're selling that you do UI/UX *and* ship product.
A loud CV undercuts that — it reads "designer who needs attention." A calm,
confident, perfectly-aligned CV reads "senior person who makes deliberate choices."
The design *is* the portfolio piece. One accent color (teal `#0f766e`), generous
whitespace, tight typographic hierarchy. Nothing decorative.

**2. Scannable in one pass.** A recruiter reads the left edge top-to-bottom. So:
name → title → specialty → projects, in that order. Uppercase micro-labels for
section headers, bold the words that matter (e.g. *designs and builds*, *one
WooCommerce backend*). Everything else recedes.

**3. Lead with the specialty, not a skills dump.** Your edge is "**one backend →
web + PWA + mobile**." That's a rare, concrete, sellable thing. It gets its own
highlighted box right after the summary so it can't be missed. Generic skill lists
are commodity; that sentence is not.

**4. Projects as proof, not résumé filler.** Each project leads with *what it is*,
then bullets of *what's technically hard about it* (synced cart across 3 surfaces,
OTP auth, Docker/CI). That's what convinces another dev or a technical buyer you're
real.

**5. ATS-safe by construction.** Single column, real selectable text, logical DOM
order, no text-in-images. It parses cleanly if a platform scans it, and it looks
hand-designed to a human. You don't have to choose.

**6. The bot, handled carefully.** I framed it as a *subscription conversational-AI
platform* — the genuine engineering story (persistent memory, adaptive personas,
recurring billing) with none of the NSFW context. On a general CV that's the right
call: it's impressive and client-safe. Keep a separate, franker version only for
contexts where it's relevant.

### If you want variants
- **Freelance-platform version:** this, as is.
- **Agency / white-label version:** swap the summary's "clients" framing for
  "partner teams," lead harder on reliability (Docker, CI/CD, monorepo).
- **One accent swap:** teal is the default; `#c2410c` (burnt orange) or `#1d4ed8`
  (indigo) are one-line changes in `:root` if you want a different temperature.

### What to avoid
Photos, skill "percentage" bars, dense two-column sidebars (ATS chokes on them),
more than one accent color, icons for every line, and any font smaller than ~11px
in print.
