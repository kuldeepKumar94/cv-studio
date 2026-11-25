# Instructions for AI agents (Claude Code, Copilot, etc.)

## Project
CV Studio is one self-contained `index.html` (HTML, CSS, vanilla JS). Keep it dependency-free unless the owner asks otherwise.
The owner is a Belgium-based full-stack developer (.NET, React, TypeScript, Azure). The CV targets the Belgian market.

## Rules
- Never invent facts, dates, employers or metrics. Mark gaps as `[placeholder]`; the checks panel flags them.
- Keep the data model in `draft()` as the single source of truth. Preview, checks and backup all read the state object `S`.
- Wrap every localStorage access in try/catch.
- After any change, test: edit a field, reload, print preview (no blank pages, 2 pages max), dark mode, mobile width.
- Keep the print CSS free of grid layouts; grid fragmentation caused blank pages.
- Use plain typographic quotes in visible text.

## Backlog (pick one per task)
1. Split into modules and add a minimal build (Vite) only if needed.
2. Add tests (Playwright) for editing, autosave and print page count.
3. Job-tailoring agent: paste a job posting, get a reordered skills list and rewritten summary, never adding unsupported claims.
4. Import from LinkedIn PDF export (parse the PDF text into the data model).
5. Multiple CV versions (EN/NL, one-page, per application) stored as named JSON files.
6. Export to .docx and plain text for ATS upload.
7. Improve checks: date overlaps, gaps over 3 months, bullets without verbs or numbers, ATS keyword coverage.
