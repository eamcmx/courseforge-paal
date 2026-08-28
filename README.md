# CourseForge PAAL

Turn a teacher's **syllabus and materials** into a complete **gold-standard, AI-augmented course set**:
per session an interactive lecture, a teacher deck, gated worked solutions, a hidden instructor key and an
80%-gating formative quiz, ready to mount on Moodle.

It runs on **your own Claude account** (the `claude` CLI, no API key) and writes everything to a folder on
your computer for you to upload. Full guidance lives inside the app under **Help**.

## Licensed software

CourseForge PAAL runs only on a computer it has been licensed for. On first launch it shows your **machine
ID**; send that to Emmanuel A. Merchán-Cruz to receive a key, then paste the key to activate. Activation is
checked entirely offline. You can see your machine ID and license status any time under **Help, then License
and machine ID**.

## Download and install

From the **[Releases page](../../releases)**, download **CourseForge-PAAL-Setup-…-x64.exe** and run it.

Windows 10/11, 64-bit. It installs per user, so no administrator rights are needed, and it adds a Start menu
shortcut. At the SmartScreen prompt click **More info**, then **Run anyway**: the installer is unsigned. Run
the installer normally; the silent switch is not supported. Installing replaces any earlier CourseForge copy.

## One-time setup on each machine

The app drives **your own Claude account**, so it needs the **Claude CLI installed and signed in**. Install
the `claude` CLI, then in the app click **Connect Claude** and complete the *"Log in with your Claude
account"* step. No API key.

First time on a computer? Follow **[claude-setup.md](claude-setup.md)**, about 5 minutes. Python is bundled,
so there is nothing else to install.

---

© 2026 Emmanuel A. Merchán-Cruz. All rights reserved.

CourseForge PAAL is the exclusive property of Emmanuel A. Merchán-Cruz, sole author and owner, covering the
application, its source, and the prompts, templates, quality gates and design system it uses. It is not open
source, and no right to copy, redistribute, resell or create derivative works from it is granted.

Copyright in the application is separate from copyright in what you make with it: the lectures, decks,
solutions, keys and quizzes you generate belong to you and to your institution. Authoring runs through your
own Claude account, no course content reaches the author of this application, and the app has no telemetry.
