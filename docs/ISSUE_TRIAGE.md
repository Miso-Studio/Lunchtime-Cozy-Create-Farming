# Lunchtime Issues: How to Use the Ticket System

GitHub Issues are public tickets for things the Lunchtime team should track. They are not a private help desk, and opening an issue does not guarantee a fix or that a suggestion will be accepted.

## What should be an issue?

| Use GitHub Issues for | Use Discord or private contact for |
|---|---|
| Crashes and bugs in the modpack | “How do I craft/find/do this?” questions |
| Broken recipes, quests, items, textures, or audio | Quick troubleshooting and player-to-player help |
| Reproducible server, multiplayer, compatibility, or performance problems | Whitelist, account, payment, or other private server matters |
| Ideas for mods, quests, recipes, progression, or improvements | Personal information or sensitive reports |

Open the [Issues page](https://github.com/Miso-Studio/Lunchtime-Cozy-Create-Farming/issues), choose **New issue**, and select the Bug report or Feature request form. Search existing issues first so the same problem does not get reported several times.

## How to write a useful ticket

For a bug, include the exact Lunchtime version, Minecraft/Forge version, whether it happens on the client or server, what you expected, steps to reproduce it, and a relevant log or crash report when available. Remove private details before sharing logs. Do not upload mod JARs, full world saves, credentials, tokens, or private server information.

For a suggestion, explain the player benefit. For a mod suggestion, include its official project page and known compatibility or performance concerns.

## What the labels mean

The issue forms add a type label automatically:

- `bug` — something is broken or behaving unexpectedly.
- `enhancement` — a suggestion or improvement.
- `needs-triage` — the team has not reviewed the ticket yet.
- `needs-info` — more details are needed from the reporter.
- `confirmed` — the issue has been reproduced or otherwise verified.
- `in-progress` — someone is actively working on it.
- `blocked` — work is waiting on a dependency, upstream fix, or other blocker.
- `good first issue` — a relatively approachable task for a new contributor.

## One-time label setup

Open [Issues → Labels](https://github.com/Miso-Studio/Lunchtime-Cozy-Create-Farming/issues/labels), click **New label**, and create these labels if they do not already exist:

| Label | Description |
|---|---|
| `needs-triage` | New ticket waiting for its first review. The issue forms apply this automatically once the label exists. |
| `needs-info` | Waiting for the reporter to provide missing details. |
| `confirmed` | The problem has been reproduced or verified. |
| `in-progress` | Someone is actively working on it. |
| `blocked` | Work is waiting on an upstream fix, dependency, or other blocker. |

GitHub commonly provides `bug`, `enhancement`, and `good first issue` by default, but check the label page. If any are missing, create them too. GitHub issue forms silently skip labels that do not exist, so create `needs-triage` before relying on the automatic triage label.

## Maintainer workflow

1. **Triage:** check whether it is a duplicate, actionable, and in the right place.
2. **Ask for details:** if something important is missing, comment on the issue and apply `needs-info`.
3. **Verify and prioritize:** reproduce the bug when possible, apply `confirmed`, and decide whether it belongs in the current work.
4. **Track active work:** assign a person and apply `in-progress`; use `blocked` if it depends on something else.
5. **Close clearly:** explain when a fix is included in a release, or why a duplicate/proposal is being closed. Do not close a bug just because someone commented on it.

## Keep it lightweight

For now, two issue forms and a few labels are enough. You do not need a complex project board while the issue list is small. When you start juggling several active fixes, create a GitHub Project board with columns like **Inbox → Ready → In progress → Done**. Keep the issue itself as the discussion and history; use the board only to see work at a glance.
