# GitHub Achievements Unlocker

A complete guide + automation toolkit to help you earn **every** GitHub achievement badge.

---

## Achievement Overview

| Badge | Name | Requirement | Tiers | Auto? |
|-------|------|-------------|-------|-------|
| ⚡ | **Quickdraw** | Close an issue or PR within 5 min of opening | None | Yes (script) |
| 🦈 | **Pull Shark** | Get PRs merged | x2 / x16 / x128 / x1024 | Partially |
| 🧠 | **Galaxy Brain** | Get discussion answers marked as "Answered" | x2 / x8 / x16 / x32 | Manual |
| ⭐ | **Starstruck** | Repo gets starred | 16 / 128 / 512 / 4096 | Manual |
| 👥 | **Pair Extraordinaire** | Co-author commits on merged PRs | x1 / x10 / x24 / x48 | Yes (script) |
| 🎯 | **YOLO** | Merge a PR without a review | None | Yes (workflow) |
| 💖 | **Public Sponsor** | Sponsor any user/org via GitHub Sponsors | None | Manual |
| 🧊 | **Arctic Code Vault** | Contributed to 2020 Archive Program | RETIRED | ❌ |
| 🚁 | **Mars 2020 Helicopter** | Code used on NASA's Perseverance rover | RETIRED | ❌ |

> Retired badges are **not earnable** — don't waste time on them.

---

## Step-by-Step Guide

### 1. Quickdraw ⚡
**What:** Close an issue or PR within 5 minutes of opening it.

**How to do it:**
1. Go to any repo you own (this one works!)
2. Open a new Issue
3. Immediately click "Close issue" — done

**Or use the script:**
```bash
./scripts/get-quickdraw.sh YOUR_GITHUB_USERNAME YOUR_REPO_NAME YOUR_TOKEN
```

---

### 2. Pull Shark 🦈
**What:** Open pull requests that get merged.

**Tiers:** 2 merged PRs → 16 → 128 → 1024

**How to do it:**
1. Create a new branch in this repo
2. Make any small change (edit a file, add a line)
3. Open a PR and merge it yourself

**Repeat** — you can do this as many times as you want in this repo.

**Or use the script to batch-create PRs:**
```bash
./scripts/get-pull-shark.sh YOUR_GITHUB_USERNAME YOUR_REPO_NAME YOUR_TOKEN NUMBER_OF_PRS
```

---

### 3. Galaxy Brain 🧠
**What:** Post a reply in a GitHub Discussion that the OP marks as "Answered."

**Tiers:** 2 answers → 8 → 16 → 32

**How to do it (easiest method):**
1. Enable Discussions in this repo's Settings
2. Create a new Discussion and ask a question
3. With a second GitHub account (or ask a friend), reply with an answer
4. Mark that reply as "Answered"

> You can also genuinely help people in public repo discussions — this is the legit way.

---

### 4. Starstruck ⭐
**What:** Someone stars your repository.

**Tiers:** 16 stars → 128 → 512 → 4096

**How to do it:**
- Share this repo with friends and ask them to star it
- Post the repo on Reddit (r/github, r/programming)
- Star-exchange communities (search GitHub topics for `star-exchange`)
- Make your README interesting so it organically attracts stars

---

### 5. Pair Extraordinaire 👥
**What:** Make co-authored commits that get merged into a PR.

**Tiers:** 1 co-authored PR → 10 → 24 → 48

**How to do it:**
Add this to the bottom of any git commit message:
```
Co-authored-by: Friend Name <friend@email.com>
```

**Or use the script to automate it:**
```bash
./scripts/get-pair-extraordinaire.sh YOUR_GITHUB_USERNAME YOUR_REPO_NAME YOUR_TOKEN
```

The script creates a branch with a co-authored commit and opens + merges a PR automatically.

---

### 6. YOLO 🎯
**What:** Merge a pull request without a code review.

**How to do it:**
1. Make sure Branch Protection is OFF (or you're the only required reviewer)
2. Open a PR and merge it immediately without requesting a review
3. That's it — one-time badge

**The workflow `.github/workflows/yolo.yml` automates this if you enable Actions.**

---

### 7. Public Sponsor 💖
**What:** Sponsor any GitHub user or organization.

**How to do it:**
1. Go to any sponsored project (e.g., https://github.com/sponsors/nickvdyck)
2. Click "Sponsor" and pick even the lowest tier ($1/month)
3. Badge appears on your profile within 24 hours

> Cancel anytime after the badge appears. Many developers sponsor for $1 just for the badge.

---

## Setup (Do This First)

1. **Fork or use this repo** — push it to your own GitHub account
2. **Enable GitHub Actions** in your repo's Settings → Actions → Allow all actions
3. **Enable Discussions** in Settings → Features → Discussions
4. **Keep contributions public** — in your profile settings, enable "Show private contributions"

---

## Order of Operations (Fastest Path)

```
Day 1:
  ✅ Quickdraw     → run the script or manually open+close an issue
  ✅ YOLO          → push a branch, open PR, merge without review
  ✅ Pull Shark x2 → merge 2 PRs in this repo

Day 2–7:
  ✅ Pair Extraordinaire → run the pair script repeatedly
  ✅ Pull Shark (higher tiers) → keep merging branches
  ✅ Public Sponsor → sponsor someone for $1

Ongoing:
  ⭐ Starstruck → share the repo and collect stars
  🧠 Galaxy Brain → answer discussions (legit or self-answer with alt account)
```

---

## Checklist

- [ ] Quickdraw
- [ ] YOLO
- [ ] Pull Shark (base) — 2 PRs
- [ ] Pull Shark (bronze) — 16 PRs
- [ ] Pull Shark (silver) — 128 PRs
- [ ] Pull Shark (gold) — 1024 PRs
- [ ] Pair Extraordinaire (base) — 1 co-authored PR
- [ ] Pair Extraordinaire (bronze) — 10
- [ ] Pair Extraordinaire (silver) — 24
- [ ] Pair Extraordinaire (gold) — 48
- [ ] Galaxy Brain (base) — 2 answered discussions
- [ ] Galaxy Brain (bronze) — 8
- [ ] Galaxy Brain (silver) — 16
- [ ] Galaxy Brain (gold) — 32
- [ ] Starstruck (base) — 16 stars
- [ ] Starstruck (bronze) — 128 stars
- [ ] Starstruck (silver) — 512 stars
- [ ] Starstruck (gold) — 4096 stars
- [ ] Public Sponsor

---

## Notes

- Achievements can take **up to 24 hours** to appear after completing the action.
- Check in an **incognito window** if you don't see them right away.
- Make sure your profile is **public** and contributions are set to visible.
- You need a **Personal Access Token (PAT)** with `repo` scope to run the scripts.

---

## Sources & References

- [Schweinepriester/github-profile-achievements](https://github.com/Schweinepriester/github-profile-achievements) — most accurate community list
- [drknzz/GitHub-Achievements](https://github.com/drknzz/GitHub-Achievements) — full badge gallery
- [githubachievements.com](https://githubachievements.com/) — guide site
- [GitHub Community Discussion #176080](https://github.com/orgs/community/discussions/176080) — official community thread
