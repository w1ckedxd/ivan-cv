# Build & design notes

Internal notes for maintaining the CV. Not the public landing page — see
[`README.md`](README.md) for that.

| File | What it is |
|------|-----------|
| `cv-content.md` | **Source of truth.** Edit all text here first. Plain, easy to tweak. |
| `cv.html` | The **designed CV**. Open in a browser; also doubles as a portfolio piece. |
| `index.html` | Redirects the GitHub Pages root to `cv.html`. |
| `.nojekyll` | Tells GitHub Pages to serve the HTML verbatim (no Jekyll build). |

## Export to PDF
1. Open `cv.html` in Chrome.
2. `Cmd+P` → **Save as PDF**.
3. Margins *Default*, enable **Background graphics** (keeps the accent bar/box), paper **A4**.
4. It's tuned to land on **one page**. If a section splits awkwardly, trim a bullet.

## Fill the placeholders
Anything in `[ brackets ]` (orange on screen) is a real fact to fill in both
`cv-content.md` and `cv.html`:
- Surname, email
- Bot runtime (Node / Python)
- Start year for the freelance line
- Language levels (Russian / Georgian)

> ⚠️ The site is **public**, so these placeholders are currently visible on the
> live CV. Fill them before sharing the link widely.

---

## Design advice

The brief: a clean, recruiter/agency-friendly CV — explicitly **not** the Batumi
riso-print / broadsheet concept. A CV's job is the opposite of a personality
statement: get a busy recruiter or agency lead to "yes" in ~15 seconds. Here's the
thinking baked into `cv.html`.

**1. Restraint is the flex.** You sell that you do UI/UX *and* ship product. A loud
CV undercuts that. A calm, confident, perfectly-aligned CV reads "senior person who
makes deliberate choices." One accent color (teal `#0f766e`), generous whitespace,
tight hierarchy. The design *is* the portfolio piece.

**2. Scannable in one pass.** Name → title → specialty → projects, top to bottom.
Uppercase micro-labels for headers, bold the words that matter.

**3. Lead with the specialty, not a skills dump.** "One backend → web + PWA +
mobile" is rare, concrete, and sellable, so it gets its own highlighted box.

**4. Projects as proof.** Each leads with *what it is*, then bullets of *what's
technically hard* (synced cart across 3 surfaces, OTP auth, Docker/CI).

**5. ATS-safe by construction.** Single column, selectable text, logical order, no
text-in-images. Parses for machines, looks hand-designed to humans.

**6. The bot, handled carefully.** Framed as a *subscription conversational-AI
platform* — the genuine engineering story, none of the NSFW context. Keep a
separate, franker version only for contexts where it's relevant.

### Variants
- **Freelance-platform version:** this, as is.
- **Agency / white-label version:** swap "clients" for "partner teams," lead harder
  on reliability (Docker, CI/CD, monorepo).
- **Accent swap:** teal is default; `#c2410c` (burnt orange) or `#1d4ed8` (indigo)
  are one-line changes in `:root`.

### Avoid
Photos, skill "percentage" bars, dense two-column sidebars (ATS chokes on them),
more than one accent color, icons for every line, sub-11px print type.
