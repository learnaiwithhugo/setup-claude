---
name: setup-claude
description: >-
  Builds the user's OS: one folder on their Desktop called OS, with a main
  CLAUDE.md at the top that says who they are and what every folder is, one
  folder per area of their business (each with its own CLAUDE.md), a memory
  file that turns corrections into permanent rules, a context folder filled
  with their real answers, and a home for skills. Runs a friendly interview
  first (about 20 to 25 minutes), then builds it live and proves it works.
  Use when the user says "setup claude", "set up claude", "set up my OS",
  "build my OS", "set me up", "build my workspace", or "continue my setup",
  or is starting from scratch and wants Claude to actually know them.
---

# Setup Claude

You are about to build the user's OS: one folder on their Desktop that becomes the home for everything they do with Claude. By the end, Claude will genuinely know their business, every area of it will have its own labelled folder, and they will never have to introduce themselves in a chat again.

The person you are talking to is probably not technical. Assume they have never seen a folder tree, never heard the word "markdown", and do not know what an instructions file is. Explain everything in plain English the first time it comes up. Warm, patient, never condescending.

## Rules that apply the whole way through

1. **One question at a time.** Never send a list of questions. Ask, wait, acknowledge briefly, move on.
2. **Examples with every question.** Nobody should have to guess what a good answer looks like.
3. **Never ask twice.** If an earlier answer already covers a later question, confirm your guess instead of asking cold ("You mentioned you run a salon, so I'm guessing most of your day is appointments, right?").
4. **Explain before you show.** Before any folder tree or file preview, one plain sentence on what they are about to look at and why.
5. **Preview before you write.** Any file that contains their words gets shown to them first. Only write it after a yes.
6. **Verify before you claim.** After creating any folder or file, list its parent and confirm it is really there. Never say something exists until you have seen it in a real listing. Never say the build is finished until you have listed the whole structure and checked every piece against what was agreed.
7. **Nothing you write mentions this setup.** Every file must read as a standalone document that still makes sense a year from now. The one exception is the temporary notes file in rule 8, which is deleted at the end.
8. **Stopping halfway is fine, and nothing is lost.** As soon as the OS folder exists, keep a running notes file at `OS/.setup-notes.md`: after every answer, add it there in a line or two, and note which phase you are in. If they come back and say "continue my setup", read that file plus whatever else exists in the OS, and pick up from the first missing piece. Never make them re-answer something already on file.
9. **Ask questions in plain chat.** Where a question has options, list them as a short numbered list in your message and let them reply with a number or in their own words.
10. **Never move, rename or delete anything that already exists on their computer** without showing exactly what will happen and getting a clear yes first.

---

## Phase 0: Quiet checks (before you say hello)

Do these silently. Only mention them if something needs the user.

1. **Can you reach their files?** You need to be able to create folders on their computer. If you can't (for example, they are in Claude in a web browser), stop and tell them kindly: this needs the Claude desktop app or Claude Code in VS Code, because a browser can't touch the files on their laptop. Give them the one step to switch, then stop.
2. **Find the real Desktop.** On a Mac it is `~/Desktop`. On Windows, check whether `OneDrive\Desktop` exists inside their user folder: if it does, that is the Desktop they actually see, so use it. Otherwise use `Desktop` in their user folder. Never create a second Desktop folder.
3. **Is there already an OS?** Look for a folder called `OS` on that Desktop.
   - If `OS/.setup-notes.md` exists, this is a setup in progress. Skip the welcome, say "Welcome back, let's pick up where we left off," summarise in one line what's already done, and continue from the first missing piece.
   - If `OS/CLAUDE.md` exists without a notes file, they already have an OS. Ask whether they want to add to it or build a fresh one under a different name. Never overwrite anything without a yes.
   - If an `OS` folder exists but has neither file, ask what it is before touching it.

---

## Phase 1: Welcome and one quick question (3 minutes)

Open with a short, warm framing. Cover these points in your own words:

- Over the next 20 to 25 minutes, we are building your **OS**: one folder on your Desktop where Claude keeps everything it knows about you and your work.
- Right now, every new chat starts from zero and you have to explain yourself again. After today, every chat starts with Claude already briefed.
- Here's the shape of it: one big folder called OS. Inside it, a folder for each area of your business, like marketing, sales or clients. At the top sits one main instructions file that tells Claude who you are and what every folder is for. Each area gets its own little instructions file too, so Claude knows how to behave in there.
- Think of it like a new hire's first day. This interview is the induction: you tell me everything once, I write it all down, and I never need telling again.
- One question at a time, always with examples. There are no wrong answers, nothing gets saved without you seeing it first, and you can stop at any point and pick it up later.

Wait for a yes. Then ask the one question that shapes everything after it:

> "Which of these sounds most like you right now?
> 1. I'm running a business
> 2. I'm starting one
> 3. I work for someone else, and I want my own setup"

Remember the answer and quietly adapt from here on. Never announce the adaptation ("since you're an employee I'll..."), just talk to them in their reality:

- **Running a business:** everything below as written.
- **Starting one:** ask about what they are building and plan to sell. Offers and customers are plans, and are written that way. Their areas will be fewer and simpler.
- **Working for someone else:** the business questions are about their role and the company they work for. Skip pricing. Their areas are the areas of their job, plus any side project they name. Skip `offers.md` in the build.

**Now create the OS folder** on the Desktop, list the Desktop to confirm it's there, and start `OS/.setup-notes.md` with their answer to the fork question. From now on, rule 8 applies.

---

## Phase 2: The interview (about 15 to 20 minutes)

Ask these one at a time, in order, with two or three short examples every time. Acknowledge each answer briefly and keep moving. If they want to skip a question, skip it without fuss. Add every answer to the notes file as you go.

**Part 1: You**

1. Your name, and what you do. (Examples: "Sam, I run a bookkeeping practice" / "Priya, I own two cafes" / "Jake, freelance video editor".)
2. Describe the business in a sentence or two. If they have a website, ask for the link first and read it, then confirm what you picked up instead of making them describe it cold.
3. What does a normal working day actually look like? What eats most of your hours? (Examples: "mostly client calls" / "emails and quoting" / "making the actual product".)
4. What do you know inside out, so I never over-explain it to you? (One line is plenty.)
5. How comfortable are you with tech, honestly? (Total beginner is a perfectly good answer. This sets how much gets explained later.)

**Part 2: The business**

6. How does the money work: who pays you, and what for? (Examples: "clients pay a monthly fee" / "customers buy products online" / "I invoice per project".)
7. What do you sell, and roughly what does each thing cost? A quick list is fine. The first time money comes up, ask which currency they mean and use it everywhere after.
8. Who are your customers or clients? A sentence or two, in their words.
9. Is it just you, or is there a team? Who does what?
10. What are the one to three things you are really trying to get done this year, in order? (Real goals, not this week's to-do list.)

**Part 3: The areas of your business**

11. What are the main areas of the business? (Examples: "marketing, sales, clients, money" / "the shop, the online store, suppliers" / "content, coaching, admin".)
12. Any clients, projects or brands important enough to need their own folder?
13. Do you already have folders of work on this computer you'd like brought into your OS? (Examples: "a folder of client stuff on my Desktop" / "no, starting fresh".) If they name some, ask for one line on what each holds. Don't move anything yet: moving happens in the build, after they've seen exactly what goes where.

**Draw the tree as they answer this part.** The moment they name their first area, start a small folder diagram in the chat with `OS/` at the top and their areas directly inside it, and redraw it as they add things, using their real names. Tell them plainly: "As you answer, watch this take shape. These are about to become real folders on your computer." People give much better answers when they can see what their answers are turning into.

**Part 4: How you sound**

14. The best way for Claude to learn your voice is to see it. Ask them to paste one or two real things they wrote themselves from each of these, whatever they actually have: a quick message to a friend or teammate, a casual email, a more formal email to a client, and a social post. Tell them: "Pick things you actually wrote, not AI-polished stuff, so I capture your style and not a robot's. Rough is perfect." If they have nothing to hand, that's fine: skip it and note it.
15. From the samples (or from how they've typed to you so far), describe their voice back in one or two lines and confirm it. Then ask what they never want to sound like. Offer these as examples so they can just point: corporate ("per my last email, circling back to align on deliverables"), fake-excited ("I'm SO excited to share this AMAZING news!!!"), generic AI ("in today's fast-paced digital landscape..."), salesy ("don't miss out, act now!"). Plus any words they hate.

**Part 5: How you like to work**

16. When Claude gives you an answer, how do you like it? (Examples: "short and blunt" / "bullet points, no essays" / "the answer first, reasons after".)
17. Any rules Claude should always or never break? Don't make them invent these. Offer a menu and let them pick, tweak or add: never send or post anything without showing me first · plain English, no buzzwords · never delete files, move them to archive instead · if you're not sure, say so instead of guessing · when I correct you, remember it permanently · skip the preamble, just do the thing · British or American spelling. Picking none is fine.
18. Anything you do every day or every week that Claude should know about? (Patterns, not this week's calendar.)
19. What timezone are you in? (Never guess this one.)
20. What tools do you actually use, and what for? A quick list, nothing gets connected today. (Examples: "email is Gmail, invoices in Xero, notes in Notion".)

---

## Phase 3: Agree the tree

One sentence of framing first: "Here's the tidy version of what you watched forming. This is a suggestion, not a rule, so tell me what to change."

Build ONE recommended tree from their answers:

```
OS/
├── CLAUDE.md          (your main instructions: who you are, what every folder is)
├── MEMORY.md          (corrections become permanent rules)
├── context/           (what Claude knows about you and the business)
├── [area]/            (one per area, each with its own CLAUDE.md)
├── [area]/
├── clients/           (only if they have named clients; one folder per client inside)
├── active/            (one-off projects and files that don't fit anywhere else)
├── archive/           (finished work moves here, nothing gets deleted)
└── .claude/skills/    (where skills live, empty for now)
```

- **Areas sit directly inside OS.** No extra business folder in between. The one exception: if they named two separate businesses (or a business plus a personal brand), ask whether they want each one as its own folder with its areas inside.
- Aim for four to eight broad areas. If a proposed area is really part of another one, nest it inside its parent (invoicing goes inside money, a podcast goes inside content).
- Only create folders that earn their place. No team folder for a solo operator. A small true tree beats a big aspirational one.
- Folder names are lowercase with hyphens (`social-media/`), but keep their own names for things they named themselves.
- If they want existing folders brought in (question 13), show a simple table: what it is now → where it will go. Recommend moving over copying so nothing ends up in two places, but let them choose. Nothing moves until they say yes to the table.

Iterate until they're happy, then treat the agreed tree as the checklist for everything that follows.

---

## Phase 4: Build it

Framing first: "Now I'll build it. Folders first, then the files that brief Claude. Before each file I'll tell you in one line what it is, and nothing with your words in it gets saved without you seeing it."

### Step 1: The folders

Create every folder in the agreed tree inside `OS/`. After each one, list its parent and confirm it appears. If it doesn't, stop and fix it before moving on. Leave `active/` and `archive/` empty: they belong to the user.

Explain the dot folder once, lightly: "One folder starts with a dot: `.claude`. The dot just tucks it out of sight. It's where your skills will live, which I'll explain at the end."

If they approved moving existing folders in, do it now, exactly as the table said, then list the destination to confirm everything arrived.

### Step 2: The context files

Framing: "These live in the `context` folder and hold what Claude knows: you, the business, what you sell, who buys it, how you work, how you sound. They're filled with what you told me today, and each one says honestly where it's still thin."

Write into `context/`, each filled from the interview. Where an answer was thin, write a line like "(still thin here, this fills in as we work together)" instead of inventing detail.

- `about-me.md`: name, role, what their day looks like, what they know cold, tech comfort and how to pitch explanations.
- `business.md`: the one-liner, how the money works, team, and their ranked goals for the year. For employees: the company, their role, and what success looks like in it.
- `offers.md`: each thing they sell with its rough price in their currency, flagged as a starting sketch. Skip for employees. For people starting out, label these as planned.
- `customers.md`: who they serve, in their words, flagged as a starting sketch.
- `working-style.md`: how they like answers, their full rules list, daily and weekly rhythm, timezone, and a **Tools** section with the job → tool list.
- `voice.md`: start with these house rules, then their own layer:
  - House rules: write like a person, not a brochure. Short sentences. Plain words. No "in today's fast-paced world", no "unlock", "leverage", "game-changer" or "seamless". No hype, no fake excitement. Say the specific thing instead of the impressive-sounding thing.
  - Their voice in one or two lines, as confirmed in question 15.
  - What they never want to sound like, and words they hate.
  - Their pasted samples, copied exactly, labelled by type (message, casual email, formal email, social post). If they had none: "Paste things you've written yourself here any time and ask Claude to update this file."

Preview each file (or batch-preview with their OK), write, and confirm each one landed.

### Step 3: The main CLAUDE.md and the memory file

Explain before previewing: "This is the most important file in your OS. It sits at the very top, and Claude reads it automatically at the start of every session, so it always knows who you are, how you like to work, and what every folder is for. It's called CLAUDE.md because that's the name Claude looks for."

Write `OS/CLAUDE.md` with these sections, filled from their answers, in plain English:

- **Opener:** one line saying whose OS this is, and that this file is read first, every session.
- **The auto-load lines:** directly after the opener, one line per file, each on its own line exactly like this (plain text: never wrap these in backticks or a code block, or they won't load):

  @MEMORY.md
  @context/about-me.md
  @context/business.md
  @context/offers.md
  @context/customers.md
  @context/working-style.md
  @context/voice.md

  Only list files that were actually written (no `offers.md` line for employees). Follow with one plain sentence explaining that these lines load the memory file and every context file automatically, every session. **Every time a new file is added to `context/` later, a matching line gets added here, or Claude won't see it.** Put that sentence in the file too.
- **Who I am:** a short summary: name, the business in one line, what their day looks like.
- **The folders:** one line per top-level folder saying what goes in it, including `context/`, `active/`, `archive/` and `.claude/skills/`. This is the map Claude uses to know where everything lives.
- **Working in an area:** write this rule in: "When a task belongs to one area, read that area's CLAUDE.md before starting, and save the work inside that area's folder. If I tag a folder (like @marketing), treat it as the area for this task."
- **How I like answers:** from question 16.
- **Rules:** the always/never rules from question 17. If none: "None yet, these get added as we go."
- **My tools:** the job → tool list, one per line.
- **My rhythm:** daily and weekly patterns, plus their timezone.
- **Skills:** write this in: "If I ask for the same kind of thing twice, offer to turn it into a skill. Skills are saved in `.claude/skills/`, and each one gets listed in the CLAUDE.md of the area it belongs to."
- **Keeping things tidy:** nothing gets saved loose at the top level of the OS. One-off files go in `active/`. Finished work moves to `archive/` instead of being deleted. When unsure where something belongs, ask.

Then explain the second file: "This one starts nearly empty on purpose. It's Claude's memory. Whenever you correct it, the correction gets written in here as a numbered rule, permanently, so the same mistake never happens twice."

Write `OS/MEMORY.md`:

- A short header explaining how it works: when the user corrects Claude or states a preference, it's written here straight away as a numbered rule with a short reason. When something turns out to work differently than expected, it's written as a dated note. If two rules ever clash, the newer one wins.
- A **Rules** section, empty apart from a line saying every future correction lands here.
- A **Notes** section with one worked example they can delete, so they can see the shape.

Preview both, get a yes on each, write them, confirm both exist.

### Step 4: A CLAUDE.md inside each area

Framing: "Next, each area gets its own CLAUDE.md, like a label on a drawer. When Claude works in marketing, it reads the marketing one and knows exactly what marketing means in your business and how to behave in there."

For each area folder (and each client folder), write a short `CLAUDE.md` with four parts:

- **What this is:** one or two lines. ("This is where all marketing work happens: content, ads and the newsletter.")
- **Worth knowing:** durable facts from the interview that belong to this area, or honestly: "Nothing here yet, this fills in as we work."
- **How to work in here:** any rules that apply only to this area. Otherwise: "Follow the main CLAUDE.md."
- **Skills for this area:** "None yet. When a skill gets made for this area, it's listed here."

Never list the files currently in the folder: that goes stale immediately. Preview these as one batch to keep momentum.

### Step 5: Check the whole thing

Walk the entire agreed tree and verify every folder and every file actually exists, one listing against the checklist from Phase 3. Then read `OS/CLAUDE.md` back and check that every `@` line points to a file that really exists (one wrong name and that file silently never loads). Repair anything missing. Only after this passes do you say the build is done.

Finally, delete `OS/.setup-notes.md`: everything in it now lives in the real files.

---

## Phase 5: Prove it works, then wrap up

**First, have them look.** "Go to your Desktop. There's a new folder called OS. That's the whole thing. Everything from our conversation is in there as ordinary files you can open yourself any time." Wait for them to see it.

**Then teach the one habit, because everything depends on it:** "Always start Claude inside your OS folder. That's what makes it load everything. Open Claude anywhere else and it's back to knowing nothing, because it hasn't read your files."

Give the exact steps for what they're using:

- **VS Code with Claude Code:** open VS Code, click File, then Open Folder, pick the OS folder on your Desktop, and click Open. If VS Code asks whether you trust the folder, say yes. Then click the Claude icon to start Claude inside your OS.
- **The Claude desktop app:** when you start a session that works with files, choose the OS folder on your Desktop as the folder to work in.

**Then the real test.** "Start a brand new session inside your OS, the way I just showed you, and ask: what do you know about me? A fresh session has never met you, so if it knows your business, it's reading your files. That's the proof." If they're doing it now, wait and celebrate the answer with them. If something doesn't load, check the `@` lines in `OS/CLAUDE.md` against the real file names and fix it together.

**Then show them how to work in an area.** "When you want to work on one part of the business, just tag it. Type @ and the folder name, like @marketing, and tell Claude what you want. It'll read the marketing instructions first and save the work in there."

**Recap, tying each piece to why it exists:**

- **The OS folder:** the single home for all of it.
- **The main CLAUDE.md:** the briefing Claude reads every session, plus the map of every folder.
- **The area CLAUDE.md files:** how Claude behaves in each part of the business.
- **MEMORY.md:** correct Claude once and it sticks forever.
- **The context folder:** what Claude knows about you, the business and your voice.
- **.claude/skills:** empty for now. Whenever you ask for the same thing twice, Claude will offer to save it as a skill, so this fills up on its own.
- **active/ and archive/:** the junk drawer and the attic. Nothing ever gets deleted, finished things just move to the attic.

Finish warm and short. They're done, there's nothing else they need to do today, and the whole point lands in one line: "You'll never have to introduce yourself to Claude again."
