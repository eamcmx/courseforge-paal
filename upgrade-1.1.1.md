# CourseForge PAAL 1.1.1: install the patch and upgrade older courses

CourseForge PAAL 1.1.1 comes as a small patch for 1.1.0, and it can bring courses made by earlier versions up to the
new design without making them again. These instructions are for the course designers and lecturers who use
CourseForge.

## What 1.1.1 changes

- **A live picture in every lesson.** Beside its task, each lesson has a chart or diagram of its idea that the student
  moves with a slider or a switch. Every part also has at least one task that simulates the topic.
- **A video script for every topic.** Once a topic is generated, CourseForge writes the script of one explainer video
  for it. Nothing is voiced until a person approves the script.
- **A faster fact review.** One reviewer reads all the lessons of a part, and one second check tests all the findings,
  instead of two runs for each lesson.
- **Older courses can be upgraded.** A unit made with 1.0 or 1.1.0 gets its live pictures in place. A course made
  before 1.0 can be brought into the new design as a new course.

## Install the patch

The patch, `CourseForge-PAAL-Patch-1.1.1.exe`, is under half a megabyte. It updates CourseForge PAAL 1.1.0 in place,
and your courses, settings and licence stay as they are.

1. **Check that 1.1.0 is installed.** In Windows Settings, Apps, Installed apps, the list shows **CourseForge PAAL
   1.1.0**. On a computer without CourseForge, install 1.1.0 first from its
   [release page](https://github.com/eamcmx/courseforge-paal/releases/tag/v1.1.0), then the patch.
2. **Close CourseForge PAAL.** The patch does not run while it is open.
3. **Download the patch** from the [1.1.1 release](https://github.com/eamcmx/courseforge-paal/releases/tag/v1.1.1)
   and run it. At the SmartScreen prompt click **More info**, then **Run anyway**: the patch is not signed.
4. **Click Yes when Windows asks for permission.** It asks when CourseForge was installed for all users of the
   computer.
5. **Wait for "CourseForge PAAL is now 1.1.1"**, then press Close. Installed apps now shows **CourseForge PAAL 1.1.1**.
6. **Open CourseForge.** Your courses and your licence are where they were.

The patch replaces 8 files of the installation: the app itself and 7 engine files. It keeps the 8 files it replaced
in the folder `resources\backup-1.1.0` of the installation, which is `C:\Program Files\CourseForge PAAL` for an
installation for all users.

| The patch says | What to do |
| --- | --- |
| CourseForge PAAL is not installed on this computer | Install 1.1.0 first, then run the patch again |
| This patch updates CourseForge PAAL 1.1.0. The version installed here is ... | That computer has another version: use the full installer of the current release |
| Close CourseForge PAAL first, then run this patch again | Close CourseForge, then run it again |

## Which path for which course

What to do depends on the CourseForge version that made the course. The course board offers the right step by itself.

| Made with | What the course has | What to do |
| --- | --- | --- |
| 1.1.1 | Short lessons with live pictures | Nothing |
| 1.1.0 | Short lessons, pictures from the materials, varied tasks, no live pictures | **Upgrade** the units in place, then **Write the video scripts** |
| 1.0.0 | Short lessons, no pictures from the materials, half of the tasks "tag each item", no live pictures | **Upgrade** the units in place. For the pictures from the materials and the varied tasks of 1.1, generate a unit again |
| Before 1.0 | A long lecture, a teacher deck, worked solutions and a key per session | **Bring into the new design**: a new course beside the old one |
| Any version, a workshop topic | A tutorial around a Lab | Nothing: workshops keep their own design |

## Courses made with 1.0 or 1.1.0: upgrade the units in place

An upgrade adds a live picture to each lesson of a finished unit and keeps every other part of the lesson. It does no
web search and writes no new lessons, so it takes about a sixth of a full run.

1. Open the course board. The bar above the topics says how many units were made before 1.1.1.
2. Press **Upgrade all** in the bar, or **Upgrade to 1.1.1** on one unit's row. The units are upgraded one at a time;
   each row shows its progress, and Stop ends the run.
3. Wait for each row to say "upgraded to 1.1.1: a live picture in each of the N lessons".
4. Open a few lessons with the unit's Open button and move their live pictures.
5. Export and put the units back in Moodle, as "Put the upgraded units back in Moodle" describes.

What an upgrade changes:

- **Added:** one live picture per lesson, drawn from the facts and numbers the lesson already gives.
- **Fixed:** what today's lesson check refuses, with the smallest change, for example a source named "doc 01, page 4"
  becomes its title and page.
- **Kept:** every sentence, figure, quick check, video, task, end check and link; the unit's check (quiz) and its
  podcast.

CourseForge checks the result before it replaces the unit: the lesson check, the pages assembled, every live picture
moved in a browser, and each lesson still at least 85% its own text. It keeps the earlier version in the unit's folder
as `out.before-1.1.1`.

An upgrade does not add what 1.1 changed in the writing itself: pictures taken from the materials, facts added from
the web, varied tasks, and a simulation in every part. A 1.0 unit that needs those is generated again.

## Narrated videos for courses already generated

A topic generated with 1.1.1 gets its explainer script on its own. A course generated earlier gets its scripts from
one button, without generating anything again.

1. Open the course board. The bar above the topics says how many generated topics have no video yet.
2. Press **Write the video scripts**. CourseForge writes one explainer script (3 to 5 minutes) for each such topic,
   one topic at a time, from its lessons as they are. A topic that already has a video keeps it.
3. **Read each script** in its topic's row (Read the script). To change one, write what to change and press Write it
   again.
4. In the same bar, type who approves the scripts and press **Approve all and make the videos**. The videos are made
   one after another. Approve only scripts you have read.
5. Export the course again. The export puts each video, its captions and a poster beside the units, and MOUNTING.md
   says how to show them in Moodle.

The voice is Gemini 2.5 Pro when Settings use Gemini and hold a Gemini key; otherwise CourseForge uses its built-in
voices.

## Put the upgraded units back in Moodle

An upgrade changes only the lesson pages of a unit, so in Moodle only each unit's File resource is replaced. Its check
(the quiz) stays as it is.

1. On the course board, press **Export & MOUNTING.md**.
2. Open MOUNTING.md. Every unit that changed since the last export is marked **Changed since the last export**.
3. In Moodle, for each marked unit: open its File resource's settings, delete its files, drag in the new `.zip` from
   the `export` folder, choose **Unzip**, and set `index.html` as the main file again. Save.
4. Do not import a check that did not change: that adds a second copy of its questions.
5. Add the new videos, if any, as MOUNTING.md describes under Narrated videos.
6. Open one upgraded lesson as a student would and move its live picture.

The same steps apply to a course in the Course Studio format.

## Courses made before 1.0: bring them into the new design

A course made before 1.0 has a long lecture, a teacher deck, worked solutions and a key per session. That design
cannot be changed into short lessons in place, so CourseForge makes a new course beside it and leaves the old one as
it is.

1. Open the old course. The bar above its sessions says it was made before CourseForge 1.0. Press **Bring into the
   new design**.
2. CourseForge makes a new course named "<old name> (1.1 design)", with the same syllabus and settings, and opens it.
   It holds a copy of each old session's materials and the text of its lecture, waiting for the new units.
3. Check the course settings, then **propose the plan** and approve it, as for any new course.
4. Press **Attach the earlier materials** in the bar. Each new unit takes the materials of the session at the same
   place in the old course, and that session's lecture as one more source. A unit that already has materials keeps
   them.
5. Look over each unit's materials and change any that do not fit its topic.
6. Press **Generate all**. The course is written in the new design from these sources, unit by unit, with its checks
   and live pictures.
7. Export it and mount it in Moodle as a new course. Keep the old Moodle course until the new one has been checked.

This path generates every unit, so it takes a whole run per unit.

## Time

Measured on one test unit (4 lessons, one part of a distance week), with Claude Opus 5.5 at extra high effort:

| What | 1.1.1 | 1.1.0 |
| --- | --- | --- |
| Generating a unit (web search, writing, fact review, repair, check) | 83 min | 142 min |
| Of which the fact review | 23 min | 86 min |
| Upgrading a unit in place | 13 min | (no upgrade in 1.1.0) |

Estimates, not measured: a course of 6 lesson parts takes about 8 hours to generate with 1.1.1, and about
1 hour 20 minutes to upgrade in place. Workshops and video scripts come on top of both.

## If something goes wrong

An upgrade that does not pass leaves the unit exactly as it was, and its row says why.

| The row says | What it means | What to do |
| --- | --- | --- |
| The upgrade changed the text of lesson N | The agent rewrote more than the live picture | Press Upgrade again; if it repeats, generate the unit again |
| The upgrade did not pass the lesson check | A live picture or another part of a lesson broke a rule | Press Upgrade again; the row names the lesson and the rule |
| The live picture does not change when its controls are used | A picture's slider or switch moves nothing | Press Upgrade again |
| ... is open in another program | A file of the unit is open, for example in a browser | Close it, then press Upgrade again |

**To go back to the unit before its upgrade:** the earlier version is kept in the unit's folder as `out.before-1.1.1`
(the board's Open folder button, then `sessions/session-NN`). Close CourseForge, rename `out` to `out.upgraded`,
rename `out.before-1.1.1` to `out`, and open CourseForge again.

**To go back to 1.1.0 after the patch:** run the full CourseForge PAAL 1.1.0 installer again. The courses are not
touched by it. The 8 files the patch replaced are also kept in `resources\backup-1.1.0` of the installation.
