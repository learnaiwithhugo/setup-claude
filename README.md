# Setup Claude

A Claude skill that builds your OS: one folder on your Desktop that holds everything Claude needs to know about you and your business.

Claude interviews you first (one question at a time, always with examples), then builds the whole thing live and checks every piece is really there.

## What it builds

```
OS/
├── CLAUDE.md          your main instructions: who you are, what every folder is
├── MEMORY.md          correct Claude once and it becomes a permanent rule
├── context/           everything about you: the business, what you sell, your customers, how you work, how you sound
├── marketing/         one folder per area of your business,
├── sales/             each with its own CLAUDE.md
├── clients/           (only if you have clients, one folder each inside)
├── active/            one-off projects and files that don't fit anywhere else
├── archive/           finished work moves here, nothing gets deleted
└── .claude/skills/    where your skills live, empty to start
```

The areas are yours. They come from your answers, so a cafe owner and a bookkeeper end up with different folders.

- **CLAUDE.md** is a note Claude reads at the start of every session. It loads all your context and holds a map of every folder, so Claude already knows who you are.
- **Each area's CLAUDE.md** says what that folder is for and how you like to work in there. Tag the folder (like @marketing) and Claude reads it before starting.
- **MEMORY.md** starts nearly empty. Every time you correct Claude, the correction is saved here so it doesn't happen twice.

## How long it takes

About 20 to 25 minutes, mostly the interview. You can stop halfway and say "continue my setup" later. Nothing you've answered is lost.

## What you need

Claude Code (in VS Code or the terminal) or the Claude desktop app. It won't work in Claude in a web browser, because a browser can't create folders on your computer.

## Install

The easy way: open Claude Code and paste this:

```
Install this skill globally for me: https://github.com/learnaiwithhugo/setup-claude
```

Or do it by hand:

1. Click the green **Code** button above, then **Download ZIP**, and unzip it.
2. Move the `setup-claude` folder (the one containing `SKILL.md`) into your skills folder:
   - Mac: `~/.claude/skills/`
   - Windows: `%USERPROFILE%\.claude\skills\`
3. Restart Claude Code.

## Run it

Type:

```
setup claude
```

Answer honestly. Real answers in, real setup out. When it finishes, start a fresh session inside your OS folder and ask Claude "what do you know about me?" If it knows your business, it's working.

## One habit

Always start Claude inside your OS folder. That's what loads everything. Open Claude anywhere else and it's back to knowing nothing.

---

Made by [Hugo Manning](https://www.instagram.com/hugomxnning/) · [learnaiwithhugo.com](https://learnaiwithhugo.com)
