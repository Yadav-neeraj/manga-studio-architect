# 🎨 Manga Studio Architect (Pro Max Ultra Edition)

> **Next-Generation Manga & Anime Creation Engine for AI Coding Agents**  
> *Reverse-Engineered from classic ink mastery, 3D cinematographic camera staging, and tactical battle physics.*

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Format: Antigravity / Claude Code / Cursor Skill](https://img.shields.io/badge/Agent%20Skill-Standard%20Format-green.svg)](#installation)
[![Version: 4.0.0](https://img.shields.io/badge/Version-4.0.0-orange.svg)](SKILL.md)

---

## ⚡ Overview

**Manga Studio Architect** is an elite AI Agent Skill designed to transform raw story concepts into **publishable Japanese Manga storyboards (Name / ネーム), Webtoons, dynamic anime cinematographic directing, and reproducible AI art prompts (Midjourney v6.1 / Niji 6, Flux.1, SDXL)**.

Unlike naive AI prompt templates that produce generic "talking-head" dialogue or forget established plot points after two chapters, **Manga Studio Architect** operates on:
1. **The 3D Virtual Cinematography Engine:** 14mm fisheye to 85mm optical telephoto compression with 3-layer spatial parallax.
2. **The Sakuga & Combat Physics Engine:** Real-world inertia, momentum conservation, Mach shockwaves, and Yutapon geometric debris.
3. **The Deductive Causality Engine:** Togashi-style tactical chess, information asymmetry (anti-omniscient leak), and zero-healing injury persistence.
4. **The Zero-Context-Loss Memory Dossier:** An externalized 4-tier persistent state ledger (`MANGA_STATE_LEDGER`) that maintains continuity across 100+ pages without context drift.

---

## 🏛️ System Architecture

```
[Raw User Prompt / Chapter Premise]
         │
         ▼
┌────────────────────────────────────────────────────────┐
│ Phase 0: Memory Ingestion & State Sync                │
│ - Reads active MANGA_STATE_LEDGER (Injuries, Gear, HP) │
│ - Enforces Cognitive Isolation (What characters know)  │
└────────────────────────────────────────────────────────┘
         │
         ▼
┌────────────────────────────────────────────────────────┐
│ Phase 1: Narrative & Ideological Conflict Engine       │
│ - Thesis vs Antithesis (Moral friction)                │
│ - Kishōtenketsu (起承転結) 4-Beat Pacing Rhythm         │
│ - Togashi Cost-Benefit Axiom (Equivalent Sacrifice)   │
└────────────────────────────────────────────────────────┘
         │
         ▼
┌────────────────────────────────────────────────────────┐
│ Phase 2: Character Consistency Matrix (Visual DNA)     │
│ - Silhouette, facial anchors, signature fashion tokens │
│ - Micro-physical behaviors & tells during dialogue     │
└────────────────────────────────────────────────────────┘
         │
         ▼
┌────────────────────────────────────────────────────────┐
│ Phase 3: The Sakuga Storyboard (Name / ネーム)         │
│ - Virtual Optics (14mm Wide vs 85mm Telephoto)         │
│ - 3-Layer Spatial Parallax (Foreground / Mid / Back)   │
│ - Combat Physics (Mach cones, Yutapon debris)          │
│ - Authentic Drawn-in Katakana SFX & "Ma" (Silence)     │
└────────────────────────────────────────────────────────┘
         │
         ▼
┌────────────────────────────────────────────────────────┐
│ Phase 4: Production-Grade AI Art Prompts               │
│ - 7-Component Mathematical Prompt Structure            │
│ - Negative Artifact Shields against AI defects         │
└────────────────────────────────────────────────────────┘
         │
         ▼
┌────────────────────────────────────────────────────────┐
│ Phase 5: State Delta Mutation & Memory Handoff         │
│ - Updates injuries, spent inventory, terrain fractures │
│ - Outputs fresh MANGA_STATE_LEDGER for next chapter    │
└────────────────────────────────────────────────────────┘
```

---

## 📁 Repository Structure

```tree
manga-studio-architect/
├── SKILL.md                              # Master Skill Instruction & Operating System
├── README.md                             # Repository Documentation
├── LICENSE                               # MIT License
├── references/
│   ├── anime-directors-bible.md          # Kubo, Togashi, Murata, Fujimoto, Miura directing DNA
│   ├── sakuga-and-physics.md             # 12 animation principles, kinetic recoil, Yutapon cubes
│   ├── cinematography-3d-camera.md       # 14mm-200mm optics, Dutch angles, 3D parallax layers
│   ├── dialogue-and-subtext.md           # Text vs Subtext vs Action, Japanese "Ma" silence
│   ├── logic-and-causality.md            # Anti-plot-hole laws, information asymmetry, injuries
│   ├── memory-dossier-protocol.md        # 4-tier persistent memory ledger (MANGA_STATE_LEDGER)
│   ├── anti-patterns-and-quality-gates.md# 7 deadly sins & 7 zero-defect quality gates
│   ├── panel-layouts.md                  # Traditional Gyaku-Z & mobile webtoon scroll pacing
│   ├── prompt-formulas-ultra.md          # 7-component diffusion prompt architecture
│   ├── prompt-formulas.md                # Style-specific prompt presets (Shonen, Seinen, Manhwa)
│   └── sfx-glossary.md                   # Authentic Japanese Katakana onomatopoeia dictionary
└── examples/
    └── titan-weave-sample.md             # End-to-end benchmark chapter script with prompts
```

---

## 🚀 Installation & Usage

### 1. In Google Antigravity / Gemini CLI
Clone or copy this folder directly into your global skills directory:
```bash
# Windows
Copy-Item -Path .\manga-studio-architect -Destination "$env:USERPROFILE\.gemini\config\skills\manga-studio-architect" -Recurse -Force

# Linux / macOS
cp -r manga-studio-architect ~/.gemini/config/skills/
```

### 2. In Project-Specific Workspaces (.agents / Claude Code / Cursor)
Copy into your project's `.agents/skills/` directory:
```bash
mkdir -p .agents/skills/
cp -r manga-studio-architect .agents/skills/
```

### 3. Usage Trigger
Simply ask your coding agent in natural language:
> *"Write a high-stakes shonen manga chapter where two martial artists duel across a collapsing bridge, with Togashi-style tactical logic and Midjourney prompts."*

The agent will automatically invoke the skill, generate character consistency bibles, sequence the panels, audit for zero defects, and append the updated `MANGA_STATE_LEDGER`.

---

## 🛡️ The 7 Zero-Defect Quality Gates

Every storyboard generated by this skill must pass 7 automated editorial checks:
1. **Optics & Camera Variety:** 100% variety in shot types and focal lengths (no talking heads).
2. **Action Physics Law:** Ground recoil, inertia, and secondary follow-through accounted for.
3. **Subtext & "Ma" Check:** Spoken text contrasts with physical micro-behavior or strategic truth.
4. **Eye-Flow & Kime-Doma:** Gyaku-Z hierarchy validated; climax positioned on page-turn/scroll drop.
5. **Authentic Katakana SFX:** Accurate onomatopoeia integrated with drawing direction (ドドドド, ゴゴゴゴ).
6. **AI Reproducibility Shield:** Visual DNA anchors and negative prompts locked in.
7. **Causality & Memory Integrity:** Zero healing contradictions; cognitive boundaries respected.

---

## 📜 License

Distributed under the MIT License. See [LICENSE](LICENSE) for details.
