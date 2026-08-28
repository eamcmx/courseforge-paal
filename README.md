# CourseForge PAAL

Turn a teacher's **syllabus + materials** into a complete **gold-standard, AI-augmented course set**:
per session an interactive lecture, a teacher deck, gated worked solutions, a hidden instructor key and
an 80%-gating formative quiz, ready to mount on Moodle.

It runs on **your own Claude account** (the `claude` CLI, no API key) and writes everything to a folder
on your computer for you to upload.

*Progressive AI-Augmented Learning* is not an add-on chapter here. Each session carries its stage of the
arc, from AI as consultant, through assistant, to co-developer, with the guided prompts, the reality-check
step and the co-development log woven into the session itself. Before building, a consultation reads the
whole curriculum and reasons about **where AI belongs** in it, topic by topic.

## Download

From the **[Releases page](../../releases)**, download **CourseForge-PAAL-Setup-…-x64.exe** and run it.

Windows 10/11, 64-bit. It installs per user, so no administrator rights are needed, and it adds a Start
menu shortcut. At the SmartScreen prompt click **More info**, then **Run anyway**: the installer is unsigned.

Run the installer normally. The silent `/S` switch does not work on these builds.

## One-time setup on each machine

**Just one thing:** the **Claude CLI and your Claude account.** Install the `claude` CLI, then in the app
click **Connect Claude** and complete the one-time *"Log in with your Claude account"* step. No API key.

First time on a computer? Follow **[claude-setup.md](claude-setup.md)**, about 5 minutes.

Python is bundled inside the app, so there is nothing to install for reading PDF, Word or PowerPoint files
or for the quality checks. Use **Settings**, then **Check Claude connection**, to confirm.

## How to use it

1. **Connect Claude** on the first run.
2. **＋ New course**, then paste or load the **syllabus** and set programme, level, ECTS and language.
   The **field of study** sets the discipline style, so a Language or Management course gets no formulas
   forced into it. The **study form** decides the shape of the course (see *Distance courses* below).
3. **Review the plan.** It mirrors the syllabus, and nothing is generated until you **Approve**.
4. Per session, drop the teacher's **materials** or attach a ready-made **lecture HTML**, then **Generate**.
   Live progress shows the current step, what the agent is doing, and elapsed time.
5. *(Optional)* On a generated session, click **🎙 Podcast** for a two-host episode about that topic.
6. **Export & MOUNTING.md**, then follow the generated sheet to mount the parts on Moodle, including the
   80% quiz gate and the reveal-on-pass settings.

Generation runs **one session at a time** on your Claude account and typically takes 10 to 30 minutes per
session. CourseForge **enriches the teacher's own material** rather than inventing generic content, and it
will not mark a session done until it passes the quality gates.

## Distance courses

Choosing **Distance** as the study form is not just a label. It rebuilds the shape of the whole course.

- **The course becomes a calendar of weeks.** Credits decide how many: **3 ECTS runs over 8 weeks, 6 ECTS
  over 16**. The wizard shows the week count as soon as you type the credits.
- **One topic per week, studied in two parts.** Part 1 opens the topic and builds the ideas, part 2 applies
  and consolidates them and closes the week. A week is never two unrelated topics stitched together.
- **No teacher deck.** Nobody is presenting, so everything a presenter would have said belongs in the
  interactive lecture. A distance session ships four parts instead of five.
- **Written for someone studying alone.** The prose is checked for classroom language and rewritten if it
  slips in.
- **Mounting follows the calendar:** one Moodle section per week, with that week's two parts inside it.

Materials are still attached per part, so a 3 ECTS distance course means attaching materials to sixteen parts.

## Readability

All student-facing prose is scored (Flesch Reading Ease, Flesch-Kincaid, Gunning Fog, SMOG, Coleman-Liau)
and simplified if it drifts out of range, because most of our students are not native English speakers.
Any generated session can be re-checked, and simplified on request, without regenerating it.

## Editing a page without regenerating it

Every generated lecture, worked-solutions and instructor-key file carries a hidden edit mode. Open the file,
press <kbd>Ctrl+Shift+E</kbd>, enter the course's edit password, click any text and edit it, then export a
clean updated copy ready to re-upload. Formulas and interactive widgets keep working, and students never see
the mode.

## Troubleshooting

- **"Claude: not connected"** → open a terminal, run `claude`, finish the login, then click **Re-check**.
  Not installed yet? See **[claude-setup.md](claude-setup.md)**; the native installer needs no Node.js.
- **"The engine was not found"** → Settings is pointing at a folder from an older install. Clear the
  **engine folder** field and save, and the app finds its own engine again.
- **A build stopped partway** → nothing is lost. Sessions that finished stay finished, and starting again
  resumes at the first one that did not.
- **A session will not finish** → it re-authors on a failed gate. Check the live activity feed and re-run it.

The full manual is inside the app under **Help**, and can be saved as a standalone file from there.

---

© 2026 Emmanuel A. Merchán-Cruz. All rights reserved.

CourseForge PAAL is the exclusive property of Emmanuel A. Merchán-Cruz, sole author and owner, covering the
application, its source, and the prompts, templates, quality gates and design system it uses. It is not open
source, and no right to copy, redistribute, resell or create derivative works from it is granted.

Copyright in the application is separate from copyright in what you make with it: the lectures, decks,
solutions, keys and quizzes you generate belong to you and to your institution. Authoring runs through your
own Claude account, no course content reaches the author of this application, and the app has no telemetry.
