# APR intake widget

A free, standalone browser tool for Singapore MOE homeschool families. It guides parents through collecting their annual progress data and generates a complete, MOE-compliant Annual Progress Report draft via Claude.

No login. No account. No data storage. Everything runs in your browser.

---

## What it does

The widget walks you through six structured steps, then sends your data to Claude to produce a formal APR draft in the correct MOE educator register. To open it within Claude Chat, drop the file into the chatbox and copy/paste "Run inline with the visualizer tool"

**Step 0: Import last year's APR (optional)**

Upload your previous APR as a `.docx` file. The tool extracts the text locally (nothing is sent to any server at this step) and uses Claude to pre-populate your curricula, strengths, development areas, and action plans for review.

**Step 1: Set up your children**

Enter each child's name, primary level, whether they are studying Science this year, and their mother tongue language (Chinese, Malay, or Tamil). The strength and gap options in Step 3 are drawn from the official MOE syllabus for each subject and language, and only show the options relevant to that child's level.

**Step 2: Curricula**

Confirm the programmes, books, and platforms used for each subject, pre-filled from Step 0 if you imported last year's APR. Remove anything you've dropped and add anything new.

**Step 3: Strengths, development areas, and action plan ratings**

Select from predefined, MOE-aligned strength labels and up to four development area labels per subject. Rate last year's action plans on a simple scale from fully achieved to still ongoing, if they were imported in Step 0.

**Step 4: CCE activities**

Toggle CCE activities from a categorised list covering Sport, Arts / Music, National Education, Academic enrichment, Cultural immersion, Cyber Wellness, Sexuality Education, Mental Health, Family / Faith, and Enrichment / Career Guidance. Add custom activities by hand, or use the calendar scan option to pull relevant events from Google Calendar via Claude, with repeating events grouped together automatically. Every activity's category can be changed with a dropdown if the automatic guess is wrong. When the APR draft is generated, each activity's write-up is pitched to the child's developmental band (Lower, Middle, or Upper Primary), so a P1 child's entry reads differently to a P6 child's.

**Step 5: Assessment samples**

Enter up to three assessment samples per subject, with mode of assessment and score.

**Generate**

Two options are available once everything is filled in. "Generate APR briefs" sends all structured data to Claude and produces the draft text on screen: curricula, strengths, building on strengths, areas for improvement, addressing areas for improvement, and a CCE table with child-specific outcome sentences. "Auto-populate Word doc" does the same, then creates a separate Word document per child. If you imported last year's APR in Step 0, the new document follows that same format, section order, and headings, so each family's document stays consistent with their own file from the year before.

---

## How to use it

Open the tool in any modern browser. No installation required.

You will need access to [Claude](https://claude.ai) in the same browser session for the AI-assisted steps: the Step 0 extraction, the Step 4 calendar scan, and the final generation. The tool uses Claude's `sendPrompt` function to pass structured prompts directly into your Claude conversation. You copy the generated output back into the widget where prompted.

If you are running the tool outside the Claude app, the AI-assisted steps fall back to manual entry. The tool remains fully usable.

---

## Privacy

No data entered into this tool is sent to any external server by the widget itself. The only external communication is the Claude prompts you choose to send, which go to Anthropic via your existing Claude session. The tool does not log, store, or transmit your child's data.

---

## Changelog

**v6.6.3, 5 July 2026**

CCE write-ups now match each child's age. When Claude writes up what a child learnt from an activity, it now writes at a level appropriate to Lower Primary (P1 to P2), Middle Primary (P3 to P4), or Upper Primary (P5 to P6). Younger children get simple, concrete descriptions of what they experienced. Older children get more reflective, values-based language. This applies to both the on-screen brief and the auto-generated Word document.

**v6.6.2, 5 July 2026**

Fixed a bug where general "arts" activities, such as "Achievers Arts Assessment", were being sorted into the wrong category because the matching only caught specific phrases like "art class", not the standalone word "art" or "arts".

**v6.6, 5 July 2026**

Two changes. First, activities imported from last year's APR are now sorted into the correct category automatically, the same as calendar imports already were, and a batch of extra keywords was added so things like floorball, hiking, election, movie, and science-related activities get sorted correctly rather than defaulting to a catch-all category. Second, the strength and gap tick-box lists for English, Maths, Science, and Mother Tongue were rewritten to use the official MOE syllabus wording, rather than labels written from personal teaching experience. Each option now only shows for the primary levels it applies to, for example algebra only appears at P6, and Science options only appear from P3 onwards. A mother tongue language setting (Chinese, Malay, or Tamil) was also added for each child, since some labels differ by language.

**v6.5, 4 July 2026**

Added a dropdown so the category of any CCE activity can be changed on the spot, whether it came from your calendar, from last year's APR, or was typed in by hand. Before this, the category was fixed once it was set.

**Earlier versions**

Changes made before v6.5 were not tracked in detail.

---

## Licence

AGPL-3.0. You are free to use, adapt, and build on this tool. Any modified versions must be published under the same licence with changes disclosed.

---

## Built by

[Ly-ann Tan Low](https://www.linkedin.com/in/ly-ann-tan-902b6822/), founder of LitLens Studio. Singapore, 2026.
