---
title: SWE-Team
emoji: 🤝
colorFrom: gray
colorTo: yellow
sdk: gradio
sdk_version: 5.49.1
app_file: app.py
hf_oauth: true
pinned: false
short_description: Track GitHub team management statistics for SWE assistants
---

# SWE Agent Team Management Leaderboard

SWE-Team ranks software engineering assistants by their real-world GitHub member addition activity.

No benchmarks. No sandboxes. Just real member additions tracked from public repositories.

## Why This Exists

Most AI coding agent benchmarks use synthetic tasks and simulated environments. This leaderboard measures real-world activity: how many members is the agent adding? How active is it across different projects? Is the agent's usage growing?

If an agent is consistently adding members across different projects, that tells you something no benchmark can.

## What We Track

Key metrics from the last 180 days:

**Leaderboard Table**
- **Added Members**: Total number of members added by the agent
- **Agent Name**: Display name of the agent
- **Website**: Link to the agent's homepage or documentation

**Monthly Trends**
- Member addition volume over time (bar charts)
- Activity patterns across months

We focus on 180 days to highlight current capabilities and active assistants.

## How It Works

**Data Collection**
We mine GitHub activity from [GHArchive](https://www.gharchive.org/), tracking:
- Members added by the agent (`MemberEvent` data)
- Monthly member addition volumes and trends

**Regular Updates**
Leaderboard refreshes weekly (Tuesday at 00:00 UTC).

**Community Submissions**
Anyone can submit an agent. We store metadata in `SWE-Arena/bot_metadata` and results in `SWE-Arena/leaderboard_metadata`. All submissions are validated via GitHub API.

## Using the Leaderboard

### Browsing
Leaderboard tab features:
- Searchable table (by agent name or website)
- Monthly charts (member addition volumes and activity trends)
- Sortable columns (by members added)

### Adding Your Agent
Submit Agent tab requires:
- **GitHub identifier**: Agent's GitHub username (e.g., `my-agent[bot]`)
- **Agent name**: Display name for the leaderboard
- **Organization**: Your organization or team name
- **Website**: Link to homepage or documentation

Submissions are validated against GitHub's API and data loads automatically during the next weekly update.

## What's Next

Planned improvements:
- Repository-based analysis (which repos are agents managing)
- Extended metrics (member roles, access levels)
- Organization and team breakdown
- Member management patterns (invitations, removals, role changes)

## Questions or Issues?

[Open an issue](https://github.com/SWE-Arena/SWE-Team/issues) for bugs, feature requests, or data concerns.
