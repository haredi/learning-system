# Progress

Maintained by the `/learn` skill. Read at the start of every session, updated after step 5. Confidence is honest, not encouraging: `solid` / `ok` / `shaky`.

**Current is one line, not a log.** It names the topic and the step in progress, plus anything needed to resume. Detail about what went wrong belongs in `state/WEAK-SPOTS.md` when the topic closes.

**Keep progress lightweight.** Update it only when a lesson closes or a two-round re-test identifies a weak spot. Record the next topic, confidence, and specific gap; do not turn each lesson into a task log or require a real-world exercise or formal code review to mark it complete. `./check.sh` caps this file at 150 lines.

## Current

One line per track; a lesson changes only its own track's line.

**java** — Topic: 01 — Types, values and references. Step: 3 (exercise written to IDE scratches learn/01-types-values-references/Main.java, 3 bugs, awaiting attempt; base level).

**react** — Topic: R01 — JSX. Step: not started.

**delivery** — Topic: D01 — Images, containers and the Dockerfile. Step: not started.

**node** — Topic: N01 — The event loop and async code. Step: not started.

Last review: —

## Level

Scale: `beginner` → `intermediate` → `advanced` → `senior`; a trailing `+` means close to the next.
Measured by a placement quiz, not claimed. Re-assess when a curriculum track (A, B, … ) closes. `progress.ps1` prints this column; a track with no row is not assessed yet. *Topics* are the curriculum IDs that close the gap; the progress band counts how many of them are done.

| Track | Level | Assessed | Topics | To reach the next level |
|---|---|---|---|---|

## Completed

| # | Topic | Date | Confidence | Notes |
|---|---|---|---|---|

## Scratched

Fast batch pass only (`/scratch`): seen once, quizzed once, not practised. Still open for a full lesson.

| # | Topic | Date | Quiz |
|---|---|---|---|

## Notes to self

Teaching preferences. These are starting defaults — change any of them as you learn what works for you.

- **Teaching language: English + light Egyptian Arabic.** Arabic for the room: framing,
  encouragement, corrections ("خلينا نشوف", "واضح كده؟", "برافو"). **Technical content stays
  English**: code, terms, the step-1 explanation, and the reasoning for *why* something breaks —
  that is the vocabulary the interview itself uses.

- **Never mix Arabic and English in the same line.** A line is either pure Arabic or pure English;
  mixed right-to-left lines get scrambled in the terminal. A sentence worth memorising is given
  twice — the English line, then the Arabic line directly underneath it. Nothing technical is ever
  spelled in Arabic letters: write "الـ constructor", not "الكونستركتور".

- **Every topic gets an Egyptian Arabic explanation** under its own heading (`بالمصري`): 3–5 lines
  retelling the mental model and the trap, with a blank line between Arabic lines. In scratch it
  ends every block; in a lesson it ends step 1.

- **Every topic's English part is one idea per line.** Shape, in order, each label bold on its own
  line: **In one line:** the takeaway · **How it works** 2–4 one-sentence bullets · **⚠️ Trap:**
  one line, then a `❌`/`✅` code block · **🎤 Interview:** numbered points · then `بالمصري`.

- **Keep lessons to 20–30 minutes.** Five steps, no mandatory real-world task, no drilling one
  detail past two rounds. If a concept will not fit, split it into two lessons.

- **The real-world detour is the exception, not the routine.** Take it only when it clears the bar
  in `core/METHODOLOGY.md`. A lab extract is illustration only; exercises use a neutral domain.

- **Symptom-driven exercises** — bug reports to trace, not TODOs to fill.

- **The summary card is step 4, and it is not optional.**

- **The interview PDFs in `sources/` take priority** for the java track. `state/SOURCES.md` maps
  every question to a topic and decides what comes next. Before step 2, open the mapped question in
  the PDF (`pdftotext -layout`) and build steps 2 and 5 from what it actually asks.
