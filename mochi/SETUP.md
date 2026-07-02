# Setting up Mochi in Claude — click by click

Goal: a Claude **Project** you open and talk to, backed by your **Mochi Board** sheet,
with a **9:00 AM** recap that fires on its own. ~10 minutes, one time.

## Step 1 — Create the Project
1. Go to **claude.ai** and sign in as **rlxy3209@gmail.com**.
2. In the left sidebar, click **Projects** → **+ New project** (or **Create project**).
3. Name it **Mochi**. Give it a description like *"My daily task-triage coach."*
4. Click **Create**.

## Step 2 — Give Mochi its brain (custom instructions)
1. Inside the Mochi project, find **Instructions** (sometimes labeled *"Set custom
   instructions"* or a ✏️ pencil near the project name).
2. Open the file **`mochi/mochi-instructions.md`** from this repo, copy **everything** in it.
3. Paste it into the Instructions box and **Save**.
   - Shortcut: the raw file is at
     `https://github.com/rlxy3209-dev/job-crm/blob/main/mochi/mochi-instructions.md`

## Step 3 — Connect your Google Sheet (the Board)
1. Still in Claude, open **Settings → Connectors** (or **Feature preview**) and make sure
   **Google Drive** is connected for rlxy3209@gmail.com. (You've already connected it once.)
2. That lets Mochi read — and update — your **Mochi Board**:
   https://docs.google.com/spreadsheets/d/1uRkMBwkhaIhxp-L7acsCFOodlQo09jiD0dNlJgrRH6k/edit

## Step 4 — Take it for a spin
Open the Mochi project and just talk. Try:
> "Brain dump: I need to submit my I-20, I should text my recruiter back, and random idea —
> I want to start a newsletter someday."

Mochi should sort those into the buckets, ask about anything unclear, and update the Board.
Then try **"good morning"** to see the recap, and **"evening"** for the night nudge.

## Step 5 — Make the 9 AM recap fire on its own
If your plan has **Scheduled tasks** (look for a clock/⏰ icon or "Schedule" in the project
or the message box):
1. Create a scheduled task in the Mochi project.
2. Time: **daily, 9:00 AM**.
3. Prompt: **"Run my Mochi morning recap from the Board."**
4. Save. Optionally add a second one at **8:30 PM**: *"Run my Mochi evening nudge."*

If you don't see Scheduled tasks, no problem — just type **"good morning"** each day and
you get the identical recap.

## Optional — phone focus (the 30-min scroll interruption)
Claude can't watch your screen, so your phone does the watching and Mochi does the talking:
1. Android: **Settings → Digital Wellbeing & parental controls → App timers**. Set limits on
   your social apps (e.g. 30 min), covering the 9 AM–12 PM and late-night windows. Or install
   **Opal**, **one-sec**, or **Forest** for firmer interruptions.
2. When it interrupts you, open Mochi and say *"I got pulled into scrolling"* — Mochi gives you
   the boundary pep-talk and the smallest next step.

---
That's it. Mochi is now something you open and speak to, every day.
