# Mochi 🍡

Mochi is a personal thinking-partner and coach that lives **inside Claude**. You open
it, talk out loud about whatever's on your mind, and it sorts every thought, to-do,
meeting, and idea into a five-bucket priority board — then coaches you through actually
doing the important things.

## The pieces

| Piece | What it is | Where it lives |
| --- | --- | --- |
| **Mochi persona + logic** | The coach's voice, the 5-bucket sorting, the capture loop, the daily rituals | [`mochi-instructions.md`](./mochi-instructions.md) — paste into a Claude **Project → Custom Instructions** |
| **The Board** | A Google Sheet that is the durable memory of every task | [Mochi Board](https://docs.google.com/spreadsheets/d/1uRkMBwkhaIhxp-L7acsCFOodlQo09jiD0dNlJgrRH6k/edit) in your Drive |
| **9 AM recap** | A recurring in-chat message (no email) | See "The recurring recap" below |

## The five buckets

1. **Urgent & Important** — do now.
2. **Important, not Urgent** — plan it (this is where your future gets built).
3. **Urgent, not Important** — delegate or dispatch.
4. **Not Urgent, not Important** — brain dump, no pressure.
5. **Wild Idea Parking** — creative/random sparks.

If you don't say whether something is urgent or important, Mochi asks instead of guessing.

## Setup (one time)

1. **Create a Claude Project** called "Mochi".
2. Open `mochi-instructions.md`, copy the whole thing, and paste it into the Project's
   **Custom Instructions**.
3. Make sure the Project has your **Google Drive/Sheets** connection enabled so Mochi
   can read (and update) the Board.
4. Start talking. Brain-dump freely — Mochi captures and sorts it onto the Board.

## The recurring recap — how it actually works (the honest version)

You asked for the 9 AM recap to arrive as a **recurring message from Claude in the chat,
not an email.** Here's the real state of that, because I'd rather be straight than
oversell:

- **The content is fully built.** The exact recap format — yesterday's wins, today's
  open Urgent & Important, impact/countdown walk-throughs, one first step — is specified
  in the instructions. Say **"good morning"** or **"recap"** anytime and you get it
  immediately and reliably. Same for the **8:30 PM** nudge — say "evening" / "nudge".
- **A truly self-firing 9 AM message** (one that appears without you typing anything)
  depends on the surface:
  - In a **Claude web/desktop Project**, use Claude's built-in **Scheduled task**
    feature if available on your plan: schedule a daily 9:00 AM task with the prompt
    *"Run my Mochi morning recap from the Board."* That's the durable, no-typing path.
  - In a **Claude Code session** (like the one that built this), a `cron` job can fire
    the recap — but it only runs while that session is alive and expires after 7 days,
    so it's good for short stretches, not a forever-morning ritual.
- **What this is not:** it does not send email and does not touch Gmail — exactly as you
  asked.

## What Mochi cannot do (and the workaround)

- **Watch your phone / sound alarms for social-media time.** No cloud assistant can —
  that's an OS-level capability. Set **Android Digital Wellbeing** (or one-sec / Opal /
  Forest) for your 9 AM–12 PM and late-night windows to *detect and interrupt*. Mochi
  supplies the coaching script behind the boundary (see the instructions).
- **Silently monitor all your chats/projects/devices.** By design there's no
  cross-conversation surveillance — and you wouldn't want one agent wired into
  everything anyway. Mochi is scoped to the Board + what you tell it, and that's enough.

## Daily flow

- **Anytime:** open Mochi, talk, it captures + sorts onto the Board.
- **9:00 AM:** "good morning" → recap of yesterday's wins + today's must-dos + nudges.
- **8:30 PM:** "evening" → what's still open; lowest-lift option if you're tired.
- **Sunday:** "weekly review" → celebrate, re-sort, revisit parked ideas.
