# mos-smma-skills

Social media marketing skills for Claude Code: platform-ready posts in your voice, from a topic or repurposed from something long you already made.

Built by [The Vibe Marketing Lab](https://www.skool.com/the-vibe-marketing-lab) for the MarketingOS engine (`pipx install marketing-os`).

## What's in here

| # | Skill | What it does | Time |
|---|-------|--------------|------|
| 1 | `/mos-linkedin-post` | LinkedIn posts from a topic, or a batch repurposed from one long-form piece (a transcript, a wiki page, a past post) | ~2-3 min |
| 2 | `/mos-x-post` | X/Twitter posts and threads from a topic, or long-form repurposed into tweets | ~2-3 min |

More platforms land here as they're built. One folder per skill, each with its own `SKILL.md`.

## Prerequisites

1. **Claude Code** with a Claude Pro or Max subscription.
2. **Your voice on file** in the project you run from: `reference/core/voice.md` and `reference/core/audience.md`. The posts are only as much "you" as those files are.

## Install

Skills live in `~/.claude/skills/`. This repo keeps them under version control and links them into place, so a `git pull` is all an update takes.

```bash
git clone https://github.com/the-vibe-marketing-lab/mos-smma-skills.git ~/Desktop/mos-smma-skills
cd ~/Desktop/mos-smma-skills
bash setup.sh
```

`setup.sh` links every skill folder in this repo into `~/.claude/skills/` (a symlink on macOS and Linux, a directory junction on Windows via Git Bash). Restart any open Claude Code session, then type `/mos-linkedin-post` to confirm it loads.

**Updating:** `cd ~/Desktop/mos-smma-skills && git pull`. The links point at the clone, so that's it. Updates are announced in the Skool community.

**Other packs:** this is one of the `mos-*-skills` packs that accompany the [MarketingOS engine](https://github.com/the-vibe-marketing-lab/marketing-os). The full list is in the [marketing-os-skills](https://github.com/the-vibe-marketing-lab/marketing-os-skills) README.

## How to use

- **From a topic:** `/mos-linkedin-post` then "a post on why most gym owners over-discount in January". You get options in your voice, hook first.
- **From long-form:** point either skill at a file. A YouTube transcript from [mos-yt-skills](https://github.com/the-vibe-marketing-lab/mos-yt-skills) or a wiki page from your knowledge library turns into a week of posts in one run.
- **Threads:** `/mos-x-post` and ask for a thread. It structures the hook, the body tweets and the close.

## Tips

- Repurpose from your best long-form, not your newest. The material that already worked has the proof in it.
- Post the draft that sounds most like you, not the one that sounds most like LinkedIn.
