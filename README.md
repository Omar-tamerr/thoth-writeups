# 𓂀 THOTH Writeup Library

> Official writeup library for [THOTH CTF AI Mentor](https://github.com/omar-tamerr/thoth)

**By Omar Tamer · EG · [omar-tamerr.github.io](https://omar-tamerr.github.io)**

---

## What is this?

This repo powers the `thoth library` command inside THOTH.

Every writeup here is a **progressive hint engine** — not a blog post.
Each stage has 3 hint levels that unlock one at a time:

```
nudge      → gentle direction, no spoilers
clue       → names the tool or vulnerability class
near_solve → specific enough to act on, stops before the flag
```

Users get hints from your writeup without ever seeing the full solution.

---

## Usage (inside THOTH)

```bash
thoth library                          # browse all writeups
thoth library --load wgel              # load by name (fuzzy)
thoth library --url https://tryhackme.com/room/wgelctf  # load by URL
thoth library --update                 # fetch latest
```

---

## Current Library

| # | Room | Platform | Difficulty | Tags | Author |
|---|------|----------|------------|------|--------|
| 1 | [Wgel CTF](writeups/THM-Wgel.json) | TryHackMe | Easy | web, ssh, privesc, wget | [Omar Tamer](https://omar-tamerr.github.io) |

*New writeups added regularly. Watch the repo for updates.*

---

## Want to Collaborate?

If you write CTF writeups and want yours in the THOTH library — I would love to work together.

> ⚠️ **Only writeups with explicit permission from the author are accepted.**
> No writeup is ever added without direct agreement from the creator.

### What you get

- Your name on every hint THOTH delivers from your writeup
- Your writeup URL linked in the library for every user
- Credit in this README and the THOTH tool
- Exposure to the full THOTH user base

### How it works

1. Open an issue titled `[Collaboration] Room Name`
2. Link your existing writeup (blog, Medium, GitHub Pages — anywhere)
3. We agree on terms
4. I convert it to THOTH format — or you can do it yourself using the template below
5. PR merged, you're in the library

### Writeup JSON format

```json
{
  "slug":       "THM-RoomName",
  "room":       "Room Name",
  "platform":   "TryHackMe",
  "difficulty": "Easy",
  "author":     "Your Name",
  "author_url": "https://your-site.com",
  "tags":       ["web", "privesc"],
  "description": "One line description of the attack chain",
  "full_writeup_url": "https://link-to-your-writeup.com",
  "key_facts": [
    "port 80 Apache",
    "username found in source",
    "SSH key exposed"
  ],
  "stages": {
    "recon": {
      "nudge":     "Gentle question that points the right direction — no specifics",
      "clue":      "Name the tool or vulnerability class — not the exact command",
      "near_solve": "Specific enough to act on — stop just before the flag/shell"
    },
    "enumeration": {
      "nudge":     "...",
      "clue":      "...",
      "near_solve": "..."
    },
    "foothold": {
      "nudge":     "...",
      "clue":      "...",
      "near_solve": "..."
    },
    "privesc": {
      "nudge":     "...",
      "clue":      "...",
      "near_solve": "..."
    }
  }
}
```

---

## Links

- THOTH Tool: [github.com/omar-tamerr/thoth](https://github.com/omar-tamerr/thoth)
- My Writeups: [omar-tamerr.github.io](https://omar-tamerr.github.io)
- Open a collaboration issue here

---

*𓂀 THOTH CTF AI Mentor — Learn. Solve. Grow.*
