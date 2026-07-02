# APR Intake Widget

A free, standalone browser tool for Singapore MOE homeschool families. It guides parents through collecting their annual progress data and generates a complete, MOE-compliant Annual Progress Report draft via Claude.

No login. No account. No data storage. Everything runs in your browser.

---

## What it does

The widget walks you through five structured steps, then sends your data to Claude to produce a formal APR draft in the correct MOE educator register.

**Step 0 — Import last year's APR (optional)**
Upload your previous APR as a `.docx` file. The tool extracts the text locally (nothing is sent to any server at this step) and uses Claude to pre-populate your strengths, development areas, and action plans for review.

**Step 1 — Set up your children**
Enter each child's name, primary level, and whether they are studying Science this year.

**Step 2 — Curricula**
List the programmes, books, and platforms used for each subject.

**Step 3 — Strengths, development areas, and action plan ratings**
Select from predefined MOE-aligned strength and gap labels per subject. Rate last year's action plans if they were imported in Step 0.

**Step 4 — CCE activities**
Toggle CCE activities from a categorised list aligned to the MOE CCE framework. Add custom activities, or use the calendar scan option to pull relevant events from Google Calendar via Claude.

**Step 5 — Assessment samples**
Enter up to three assessment samples per subject, with mode of assessment and score.

**Generate**
Sends all structured data to Claude, which produces a complete APR draft: curricula, strengths, building on strengths, areas for improvement, addressing areas for improvement, and a CCE table with child-specific outcome sentences.

---

## How to use it

Open the tool in any modern browser. No installation required.

You will need access to [Claude](https://claude.ai) in the same browser session for the AI steps: the Step 0 extraction, the Step 4 calendar scan, and the final generation. The tool uses Claude's `sendPrompt` function to pass structured prompts directly into your Claude conversation. You copy the generated output back into the widget where prompted.

If you are running the tool outside the Claude app, the AI-assisted steps fall back to manual entry. The tool remains fully usable.

---

## Privacy

No data entered into this tool is sent to any external server by the widget itself. The only external communication is the Claude prompts you choose to send, which go to Anthropic via your existing Claude session. The tool does not log, store, or transmit your child's data.

---

## Licence

AGPL-3.0. You are free to use, adapt, and build on this tool. Any modified versions must be published under the same licence with changes disclosed.

---

## Built by

[Ly-ann Tan Low](https://www.linkedin.com/in/ly-ann-tan-902b6822/), founder of LitLens Studio. Singapore, 2026.
