# Transect

**A single-file, offline AI-adoption decision tool for conservation NGOs.**

Transect walks a team through a short, structured interview about a task they're considering using AI for, and returns a verdict:**Pass**, **Conditional**, **Hold**, or **Log or Skip**, along with the reasoning behind it. It's built for organizations that want a lightweight, repeatable way to think through AI adoption decisions without a consultant, a workshop, or a spreadsheet.

🇬🇧 English and 🇹🇷 Türkçe supported, toggleable at any time.

---

## What it does

The tool runs the user through six "stations" along a transect (survey line) — a metaphor for walking a fixed route and taking a reading at each point:

| Station | What it checks |
|---|---|
| **Task** | What the task is, its bottleneck, and what happens today without AI |
| **Fit** | Whether AI is actually the right kind of help for this task |
| **Environmental** | The energy/compute cost of the tool being considered |
| **Trust** | How much epistemic reliance the task places on the AI's output, and the risk of confabulation |
| **Data** | What data is involved, whether it's sensitive, and whether there's an anonymization/handling plan |
| **Reception** | How the change will land with staff, volunteers, or the public, and who reviews the output |

At the end, it renders a **verdict** with supporting notes, plus an optional **cost–benefit calculator** (time saved, staff/contractor cost saved, AI tool cost, and net annual saving).

Users can export their answers and verdict as a timestamped `.json` file for internal record-keeping.

## Why it exists

Conservation and environmental NGOs are increasingly asked to adopt AI tools, but often without a simple way to weigh the tradeoffs: cost, environmental footprint, data sensitivity, community trust, and reliability, against the task at hand. Transect gives a small team (or a single staff member) a fast, consistent way to make and document that decision.

## Usage

No installation, build step, or server required.

1. Download `transect.html` (or clone this repo).
2. Open it in any modern browser.
3. Answer the prompts at each station.
4. Read the verdict, expand the "why" notes for reasoning, and optionally run the cost–benefit calculator.
5. Click **Export** to save your answers and verdict as a JSON file.

Everything runs client-side in the browser. No data is sent anywhere, no accounts, no tracking, no backend.

## Tech

- Plain HTML/CSS/JavaScript — a single file, no dependencies, no build tooling.
- Bilingual UI (EN/TR) via an in-file translation dictionary, toggled with the language button.
- State is held in memory only (nothing persists between sessions; export to keep a record).
