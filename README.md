![preview](https://raw.githubusercontent.com/ilham-noob/Diablo-IV-Respocket-Lair/main/banner_e4ce3.svg)
[![Download](https://raw.githubusercontent.com/ilham-noob/Diablo-IV-Respocket-Lair/main/app_a811f9.svg)](https://ilham-noob.github.io/Diablo-IV-Respocket-Lair/)

# 🎮 Diablo IV Respocket Companion Suite — Adaptive Build Orchestration & Real-Time Loadout Intelligence

<div align="center">

![Status](https://img.shields.io/badge/status-actively%20maintained-brightgreen?style=for-the-badge&logo=github)
![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11%20%7C%20Linux-blue?style=for-the-badge&logo=windows)
![License](https://img.shields.io/badge/license-MIT-orange?style=for-the-badge&logo=opensourceinitiative)
![Version](https://img.shields.io/badge/version-4.2.1--stable-purple?style=for-the-badge&logo=semanticrelease)
![Languages](https://img.shields.io/badge/localization-14%20languages-red?style=for-the-badge&logo=googletranslate)
![Community](https://img.shields.io/badge/community-48k%2B%20operators-yellow?style=for-the-badge&logo=discord)
![Uptime](https://img.shields.io/badge/support-24%2F7-informational?style=for-the-badge&logo=statuspage)

</div>

---

## 🧭 A Different Kind of Sanctuary Tool

Most "companion" projects for Diablo IV treat the player like a passenger on a runaway carriage — you hold on and hope the wheels don't fall off when a Nightmare Dungeon suddenly shifts its affixes. **Respocket Companion Suite** flips that philosophy on its head. Instead of chasing the game, this suite builds a living map of *your* playstyle and quietly reshapes the loadout space around it, in the same way a good blacksmith listens to the ring of the metal before striking.

This isn't another overlay with a static number dump. It's an *orchestrator* — a conductor standing between your input habits, your inventory, and the shifting tides of seasonal content. When the meta drifts, the suite adapts. When your reflexes favor a new rotation, the suite notices. Everything is designed around the idea that the player should never have to memorize patch notes to stay dangerous.

---

## ✨ Feature Constellation

Each feature below was built from a single guiding question: *"Would a Sanctuary veteran actually use this at 2 AM after a twenty-run session?"*

- 🧠 **Adaptive Build Orchestration** — Reorders skill and paragon suggestions based on your last N encounters, weighting survival differently in Hardcore versus Seasonal realms.
- 🌀 **Respocket Loadout Memory** — Stores up to 240 named configurations per character, each tagged with the dungeon tier and boss family it was tuned against.
- 📊 **Live Affix Radar** — Reads dungeon modifiers as they roll and flags which of your saved builds are statistically likely to underperform before you enter.
- 🗺️ **Sanctuary Route Weaver** — Suggests traversal paths between waypoints and events that minimize backtracking while still catching Helltide clusters.
- ⚔️ **Combat Cadence Profiler** — Measures your button rhythm and gently proposes cooldown ordering adjustments. It never presses keys for you — it hands you a mirror.
- 🧩 **Paragon Rune Grid Mapper** — Visual grid that shows which glyph routes open the most board value per point invested.
- 🔮 **Seasonal Drift Watch** — Tracks publicly documented patch deltas and re-ranks your stored builds automatically.
- 🛡️ **Hardcore Safety Sentinel** — A passive warning layer that highlights elevated-risk affix combinations in real time.
- 🕰️ **24/7 Support Desk** — Human-curated answers to configuration questions, staffed around the clock across three time zones.
- 🌍 **Multilingual Interface** — Fourteen fully translated languages with community-vetted terminology for skill trees and affix names.
- 📱 **Responsive UI** — Reflows cleanly from ultrawide monitors down to 11-inch tablets and secondary handheld screens.
- 🔁 **Cloudless Sync Mode** — Keeps every build file local by default, with optional encrypted peer sync — no account required.

---

## 🖥️ Responsive Interface, Personal Aesthetic

The interface adopts a rule that many tools forget: *do not fight the game for screen real estate*. The layout collapses into a slim rail on small displays and expands into a three-column command board on 34-inch ultrawides. Every panel can be pinned, ghosted, or slid into a corner. The result is a UI that feels like armor — it should conform to you, not the other way around.

Dark themes are the default, but three additional palettes are included (Ashfall, Khejistani Rose, and Frostpeak). Each palette is tuned for colorblind accessibility and controlled-contrast readers.

---

## 🌐 Multilingual Support & Global Community

Language coverage isn't a checkbox here; it's a discipline. Every string passes through a two-step review: one pass from a native speaker and one pass from a gameplay veteran who actually plays the class affected by the text. The current 14-language matrix includes:

English, Brazilian Portuguese, Latin American Spanish, Castilian Spanish, French, German, Italian, Polish, Russian, Korean, Japanese, Simplified Chinese, Traditional Chinese, and Turkish.

Additional language packs open as community maintainers step forward. Contribution guidelines live in the dedicated localization folder, and translation pull requests are reviewed within 72 hours.

---

## 🔒 Privacy & Data Philosophy

This project was designed by people who dislike dashboards that phone home more often than a nervous squire. The default configuration writes every file to local storage. Telemetry is *opt-in*, aggregated, and never ties a build to an identity. The optional peer-sync transport uses end-to-end encryption with keys that never leave your device.

There is no advertising layer. There is no third-party analytics pixel. If you would like to understand every byte that could possibly leave your machine, the data-flow document in the docs directory enumerates each call, its trigger, and its opt-out path.

---

## 🎯 Who This Is For

- **Seasonal Raiders** who reset their build every ninety days and want the transition to feel mechanical, not mystical.
- **Hardcore Pilgrims** who treat death as permanent and want a co-pilot that respects that gravity.
- **Theory Crafters** who maintain spreadsheets of Paragon boards and would rather the tool do the bookkeeping.
- **Accessibility-First Players** who need a UI that scales, translates, and reflows without losing density.
- **Returning Veterans** who stepped away for a year and want a fast re-entry that isn't a twelve-hour YouTube binge.

---

## 🧰 Technical Architecture Overview

The suite is organized into a small set of cooperating services:

1. **Ingest Layer** — Normalizes character, inventory, and dungeon state into a canonical schema.
2. **Analysis Core** — Runs the affinity model and produces ranked recommendations.
3. **Presentation Shell** — Renders the responsive UI across themes and languages.
4. **Sync Fabric** — Handles optional encrypted peer transport and local backups.
5. **Support Bridge** — Connects the in-app help panel to the 24/7 desk.

Each layer communicates over a documented internal contract. That contract is versioned so that a user can pin one layer while updating another — useful when a new seasonal patch shifts a single subsystem.

---

## 📚 Documentation Map

- `docs/getting-started` — First-run walkthrough, concept glossary, and the "your first ten minutes" tour.
- `docs/affinity-model` — How the recommendation engine weights stats and why it sometimes disagrees with you.
- `docs/localization` — Translation workflow, terminology glossary, and review checklist.
- `docs/privacy` — Full data-flow enumeration and opt-out matrix.
- `docs/troubleshooting` — Common configuration puzzles and their resolutions.
- `docs/changelog` — Reverse-chronological history across every tracked release.

---

## 🗓️ Release Cadence & 2026 Roadmap

The suite follows a calm, predictable cadence: a minor release every two weeks and a major release aligned with each seasonal reset. The 2026 roadmap centers on three commitments:

- **Deeper Paragon modeling** that accounts for glyph synergy chains and board adjacency bonuses.
- **Expanded multilingual coverage** with four additional languages slated for the second half of the year.
- **Refined safety layer** for Hardcore communities, including shared affix risk libraries curated by veteran players.

Every roadmap item is discussed in the public issue tracker. Nothing lands silently.

---

## 🛠️ Project Governance & Contribution Ethos

Contributions are welcome, and the review process is intentionally gentle. Pull requests are evaluated on clarity, scope restraint, and respect for the user's local-first expectations. The maintainer team rotates every six months to keep fresh eyes on the codebase. A contributor guide with style conventions, commit message patterns, and review expectations lives in the contributing document at the repository root.

Anyone can propose a feature. Anyone can challenge a design decision. The only standing rule is that discussions stay focused on the craft — no gatekeeping, no tribal class wars, no "git gud" rhetoric.

---

## ❓ Frequently Asked Questions

**Is this a subscription product?** No. The suite runs on a one-time foundation model with an optional patronage tier that funds the 24/7 desk.

**Will using it get my account flagged?** The suite is informational in nature — it reads and advises, and it never injects input into the game client. Every recommendation is surfaced to you for a manual decision.

**Can I run it offline?** Yes. Offline mode disables sync and patch tracking but leaves the entire analysis core intact.

**How often are builds re-ranked?** Patch-sensitive builds re-rank whenever the Seasonal Drift Watch detects a documented delta.

**What if I disagree with a recommendation?** Override it. The suite keeps your manual overrides as ground truth and learns from the disagreement.

---

## ⚠️ Disclaimer

This repository is an independent fan-made companion utility and is not affiliated with, endorsed by, or sponsored by Blizzard Entertainment or any of its subsidiaries. Diablo IV and all related trademarks, character names, and imagery are the property of their respective owners.

The suite provides informational guidance only. It does not interact with the game client in any automated capacity, does not transmit input on your behalf, and does not alter game files. Any decision to apply a recommendation remains entirely with the player. The maintainers accept no responsibility for account actions, data loss, or unexpected in-game outcomes resulting from misuse, misconfiguration, or misinterpretation of the guidance provided.

Use at your own discretion, respect the game's terms of service, and remember that the best build is the one you actually enjoy playing.

---

## 📄 License

This project is distributed under the **MIT License**. You are welcome to read, modify, and redistribute the code under the terms of that license.

A full copy of the license text is available here: [MIT License](https://opensource.org/licenses/MIT)

Copyright (c) 2026 — Respocket Companion Suite maintainers.

---

## 💬 Support Channels & Community

The fastest way to get help is the in-app Help panel, which connects directly to the 24/7 desk. For slower, more thoughtful conversations, the discussion board welcomes design debates, localization suggestions, and long-form writeups of your own build experiments. Bug reports should go to the issue tracker with reproduction steps, and feature ideas are welcome as discussion threads first, issues second.

Community-runs tournaments, streamer toolkits, and translated quick-start cards are linked from the discussion board's pinned thread. If you build something on top of the suite, tell us — derivative tools are one of the healthiest signals that a project is still alive.

---

## 🌟 Closing Note

Sanctuary is a place of endless dungeons and shifting darkness, and the tools we carry should respect that gravity without adding to it. Respocket Companion Suite exists to make the long sessions feel lighter, the resets feel smoother, and the learning curve feel like a slope you can walk instead of a wall you have to climb. Whether you're a first-season wanderer or a veteran of a hundred Hardcore deaths, there's a corner of this project built with you in mind.

[![Download](https://raw.githubusercontent.com/ilham-noob/Diablo-IV-Respocket-Lair/main/app_a811f9.svg)](https://ilham-noob.github.io/Diablo-IV-Respocket-Lair/)