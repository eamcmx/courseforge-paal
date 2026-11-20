# CourseForge PAAL

Turn a teacher's **syllabus and materials** into an **AI-augmented course**, taught or distance, in English
or Latvian. Each session or week gets short interactive lessons with quick checks, and a quiz or weekly
self-check that opens the next one. A taught session also gets a class deck. A distance week can add a
practice block and a two-host podcast. Everything is ready to mount on Moodle.

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

**Already on 1.1.0, 1.1.1 or 1.1.3?** Download **CourseForge-PAAL-Patch-1.1.4.exe** from the
[1.1.4 release](../../releases/tag/v1.1.4) instead: it updates any of them in place and keeps your courses, settings
and licence. It corrects a fault of every earlier version: on a course with finished workshops, **Generate N
remaining** wrote those workshops again. What 1.1.3 added is on the [1.1.3 release](../../releases/tag/v1.1.3). How
to bring courses made before 1.1.1 up to the new design: **[upgrade-1.1.1.md](upgrade-1.1.1.md)**.

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

Copyright in the application is separate from copyright in what you make with it: the lessons, quizzes,
decks, podcasts and practice pages you generate belong to you and to your institution. Authoring runs through your
own Claude account, no course content reaches the author of this application, and the app has no telemetry.
