---
title: SWE-Team
emoji: 🤝
colorFrom: red
colorTo: yellow
sdk: gradio
sdk_version: 5.50.0
app_file: app.py
hf_oauth: true
pinned: false
short_description: Track GitHub team management statistics for SWE assistants
---

# SWE Assistant Team Management Leaderboard

SWE-Team ranks software engineering assistants by their real-world GitHub membership event activity.

No benchmarks. No sandboxes. Just real membership events tracked from public repositories.

## Why This Exists

Most AI coding assistant benchmarks use synthetic tasks and simulated environments. This leaderboard measures real-world activity: how many membership events is the assistant generating? How active is it across different projects? Is the assistant's usage growing?

If an assistant is consistently generating membership events across different projects, that tells you something no benchmark can.

## What We Track

Key metrics from the last 180 days:

**Leaderboard Table**
- **Assistant**: Display name of the assistant
- **Website**: Link to the assistant's homepage or documentation
- **Total Membership Events**: Number of team membership changes (e.g., adding or removing members) performed by the assistant

**Monthly Trends**
- Membership event volume over time (bar charts)
- Activity patterns across months

We focus on 180 days to highlight current capabilities and active assistants.

## How It Works

**Data Collection**
We mine GitHub activity from [GHArchive](https://www.gharchive.org/), tracking:
- Membership events by the assistant (`MemberEvent` data)

**Regular Updates**
Leaderboard refreshes weekly (Tuesday at 00:00 UTC).

**Community Submissions**
Anyone can submit an assistant. We store metadata in `SWE-Arena/bot_metadata` and results in `SWE-Arena/leaderboard_data`. All submissions are validated via GitHub API.

## What's Next

Planned improvements:
- Repository-based analysis (which repos are assistants managing)
- Extended metrics (membership event types, member roles, access levels)
- Organization and team breakdown
- Member management patterns (invitations, removals, role changes)

## Questions or Issues?

[Open an issue](https://github.com/SWE-Arena/SWE-Team/issues) for bugs, feature requests, or data concerns.
