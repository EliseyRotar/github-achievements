<div align="center">

# 🏆 GitHub Achievements Unlocker

**The only toolkit you need to earn every GitHub achievement badge — automatically.**

[![Stars](https://img.shields.io/github/stars/EliseyRotar/github-achievements?style=for-the-badge&color=yellow&logo=github)](https://github.com/EliseyRotar/github-achievements/stargazers)
[![Forks](https://img.shields.io/github/forks/EliseyRotar/github-achievements?style=for-the-badge&color=blue&logo=github)](https://github.com/EliseyRotar/github-achievements/network/members)
[![Issues](https://img.shields.io/github/issues/EliseyRotar/github-achievements?style=for-the-badge&color=red&logo=github)](https://github.com/EliseyRotar/github-achievements/issues)
[![License](https://img.shields.io/github/license/EliseyRotar/github-achievements?style=for-the-badge)](LICENSE)

*Scripts · GitHub Actions · Step-by-step guides · Works in under an hour*

[**Quick Start**](#-quick-start) · [**All Achievements**](#-achievements) · [**Scripts**](#-scripts) · [**FAQ**](#-faq)

</div>

---

## 🚀 What is this?

GitHub has **9 achievement badges** you can earn on your profile. Most people don't know how to get them — or think they require months of open-source contributions.

This repo gives you:
- ✅ **Shell scripts** that automate Quickdraw, Pull Shark, and Pair Extraordinaire
- ✅ **GitHub Actions workflows** that auto-merge PRs for YOLO
- ✅ **Clear step-by-step guides** for every badge
- ✅ **A ready-made discussion board** to practice Galaxy Brain

> All badges can be earned **in your own repos** — no external contributions required for most of them.

---

## ⚡ Quick Start

```bash
# 1. Clone this repo
git clone https://github.com/EliseyRotar/github-achievements.git
cd github-achievements

# 2. Get a GitHub token: Settings → Developer settings → Personal access tokens → repo scope

# 3. Run whichever script you need:
./scripts/get-quickdraw.sh   YOUR_USERNAME  YOUR_REPO  YOUR_TOKEN
./scripts/get-pull-shark.sh  YOUR_USERNAME  YOUR_REPO  YOUR_TOKEN  16
./scripts/get-pair-extraordinaire.sh  YOUR_USERNAME  YOUR_REPO  YOUR_TOKEN  48  "Friend" "friend@email.com"
```

Badges appear on your profile within **24 hours**.

---

## 🏅 Achievements

### ⚡ Quickdraw
> Close an issue or pull request within 5 minutes of opening it.

**Tiers:** None — one-time badge

**Automate it:**
```bash
./scripts/get-quickdraw.sh USERNAME REPO TOKEN
```
**Manual:** Open any issue → immediately click Close issue. Done in 10 seconds.

---

### 🦈 Pull Shark
> Have your pull requests merged.

| Tier | PRs Needed |
|------|-----------|
| 🥉 Base | 2 |
| 🥈 Bronze | 16 |
| 🥇 Silver | 128 |
| 🏆 Gold | 1024 |

**Automate it:**
```bash
# Earn bronze (16 PRs) in one command:
./scripts/get-pull-shark.sh USERNAME REPO TOKEN 16
```

The script creates branches, opens PRs, and merges them automatically. Run it multiple times to stack tiers.

---

### 🧠 Galaxy Brain
> Have your discussion reply marked as the accepted answer.

| Tier | Answers Needed |
|------|---------------|
| 🥉 Base | 2 |
| 🥈 Bronze | 8 |
| 🥇 Silver | 16 |
| 🏆 Gold | 32 |

**How to earn it:**
1. Enable Discussions in your repo settings
2. Ask a question in the Q&A category
3. Reply with the answer
4. Mark it as "Answered"

> Check the [Discussions tab](../../discussions) in this repo — it's already set up with Q&A enabled!

---

### ⭐ Starstruck
> Have one of your repositories starred.

| Tier | Stars Needed |
|------|-------------|
| 🥉 Base | 16 |
| 🥈 Bronze | 128 |
| 🥇 Silver | 512 |
| 🏆 Gold | 4096 |

**How to earn it:** Star this repo ⭐ and share it with friends! Every star counts toward the achievement.

---

### 👥 Pair Extraordinaire
> Co-author commits that get merged in a pull request.

| Tier | Co-authored PRs |
|------|----------------|
| 🥉 Base | 1 |
| 🥈 Bronze | 10 |
| 🥇 Silver | 24 |
| 🏆 Gold | 48 |

**Automate it:**
```bash
# Earn gold (48 PRs) in one command:
./scripts/get-pair-extraordinaire.sh USERNAME REPO TOKEN 48 "Co-Author" "coauthor@email.com"
```

The script adds `Co-authored-by:` trailers to commits, which GitHub detects automatically.

---

### 🎯 YOLO
> Merge a pull request without a code review.

**Tiers:** None — one-time badge

**Two ways to get it:**
1. Open any PR → merge it before requesting a review
2. Add the `yolo` label to any PR → the included GitHub Actions workflow merges it automatically

---

### 💖 Public Sponsor
> Sponsor a GitHub user or organization via GitHub Sponsors.

**Tiers:** None — one-time badge

**How to earn it:** Go to any [GitHub Sponsors page](https://github.com/sponsors) and sponsor someone for $1/month. Cancel any time after the badge appears.

---

### 🧊 Arctic Code Vault Contributor *(Retired)*
Awarded to developers whose code was stored in GitHub's 2020 Arctic Code Vault. No longer earnable.

### 🚁 Mars 2020 Helicopter Contributor *(Retired)*
Awarded to developers whose code flew on NASA's Perseverance rover. No longer earnable.

---

## 📁 Scripts

| Script | What it does |
|--------|-------------|
| `scripts/get-quickdraw.sh` | Opens and instantly closes an issue via API |
| `scripts/get-pull-shark.sh` | Creates N branches, opens PRs, and merges them all |
| `scripts/get-pair-extraordinaire.sh` | Same but with `Co-authored-by:` commit trailers |

All scripts require a [Personal Access Token](https://github.com/settings/tokens) with `repo` scope.

### GitHub Actions Workflows

| Workflow | Trigger | What it does |
|----------|---------|-------------|
| `.github/workflows/yolo.yml` | PR labeled `yolo` | Merges the PR immediately without review |
| `.github/workflows/pull-shark-auto.yml` | PR labeled `auto-merge` | Auto-merges any labeled PR |

---

## 📋 Checklist

Copy this into your own notes and tick off as you go:

```
[ ] Quickdraw
[ ] YOLO
[ ] Pull Shark      — base (2) / bronze (16) / silver (128) / gold (1024)
[ ] Pair Extraordinaire — base (1) / bronze (10) / silver (24) / gold (48)
[ ] Galaxy Brain    — base (2) / bronze (8) / silver (16) / gold (32)
[ ] Starstruck      — base (16) / bronze (128) / silver (512) / gold (4096)
[ ] Public Sponsor
```

---

## ❓ FAQ

**How long until badges appear?**
Up to 24 hours. Check your profile in an incognito window to rule out caching.

**Do private repos count?**
Yes — but only if you enable *Show private contributions* in your GitHub profile settings.

**Can I earn Pull Shark by merging my own PRs?**
Yes. You don't need another person to merge them — you can open and merge your own PRs.

**Pull Shark not showing after merging PRs?**
Make sure your commits use a **GitHub-verified email**. Check with `git log -1 --format='%ae'` — it should match your GitHub noreply address (`ID+username@users.noreply.github.com`) or a verified email in [email settings](https://github.com/settings/emails). Commits with a local hostname email (e.g. `user@192.168.x.x`) may not count toward achievements.

**Will GitHub detect this as spam?**
These are all legitimate GitHub features used as intended. GitHub's own docs describe all these actions as the way to earn achievements.

**Why aren't Arctic Code Vault / Mars 2020 earnable?**
They were tied to one-time events (2020 archive snapshot and NASA mission). GitHub retired them permanently.

---

## 🤝 Contributing

Found a new achievement or a better method? PRs welcome!

If this helped you, please **⭐ star the repo** — it also helps others find it and contributes to the Starstruck achievement demonstration!

---

## 📚 References

- [Schweinepriester/github-profile-achievements](https://github.com/Schweinepriester/github-profile-achievements) — community-maintained achievement list
- [drknzz/GitHub-Achievements](https://github.com/drknzz/GitHub-Achievements) — badge gallery with images
- [GitHub Community Discussion #176080](https://github.com/orgs/community/discussions/176080) — official community thread
- [githubachievements.com](https://githubachievements.com/) — achievement guide

---

<div align="center">

**If this repo helped you, smash that ⭐ star button — it means a lot and helps others find this!**

Made with ❤️ for the GitHub community

</div>
