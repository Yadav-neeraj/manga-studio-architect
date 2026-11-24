# The Long-Form Memory Dossier Protocol (Zero-Context-Loss Architecture)

When writing large manga epics (spanning multiple chapters, volumes, or hundreds of pages), conventional AI models suffer from **Context Window Degradation**. Over time, models forget earlier wounds, confuse inventories, leak hidden secrets prematurely, and contradict established world physics.

This protocol implements an **Externalized Persistent State Ledger** (analogous to a software save-state or game engine memory bus) that guarantees 100% continuity across infinite narrative horizons.

---

## 1. The 4-Tier Memory Hierarchy

Every long-form manga project managed by this skill maintains a 4-tier structured memory matrix:

```
┌────────────────────────────────────────────────────────┐
│ TIER 1: IMMUTABLE WORLD CANON (The Physics Ledger)     │
│ - Fundamental rules of magic, technology, and biology  │
│ - Power scaling ceiling, forbidden anomalies, geography│
├────────────────────────────────────────────────────────┤
│ TIER 2: DYNAMIC ENTITY STATE MATRIX (Character Ledger) │
│ - Real-time HP, active wounds, scars, stamina reserve  │
│ - Exact inventory (held weapons, spent ammunition)     │
│ - Psychological state, cognitive trauma, hidden motives│
├────────────────────────────────────────────────────────┤
│ TIER 3: CHRONOLOGICAL BEAT ARCHIVE (The History Log)   │
│ - Condensed historical event log (Chapter/Page summary)│
│ - Timestamp / Day-cycle tracking (e.g., Day 1, 03:15 AM)│
│ - Altered environments (cratered valley, burnt forest) │
├────────────────────────────────────────────────────────┤
│ TIER 4: NARRATIVE THREAD & CHEKHOV'S GUN REGISTRY      │
│ - Open plot hooks, unresolved mysteries, debts owed    │
│ - Planted clues, pending ticking clocks, prophecies   │
└────────────────────────────────────────────────────────┘
```

---

## 2. The Standard Memory Ledger Schema (`MANGA_STATE_LEDGER`)

To prevent memory loss, this structured state block must be generated, maintained, and synchronized between turns:

```json
{
  "project_meta": {
    "title": "TITAN WEAVE",
    "current_chapter": 1,
    "current_page": 3,
    "in_universe_timestamp": "Day 1, 03:00 AM (Night)"
  },
  "world_physics_state": {
    "magic_laws": "Kinetic Vector Redirection; Acoustic Resonance Shatter",
    "cost_law": "Vector threads cause severe muscular tension; Sonic resonance requires exact pitch match"
  },
  "characters": {
    "Kaelen": {
      "status": "Alive, Combat-Active",
      "health_and_injuries": [
        "Light gravel abrasion on knees from Page 1 skid",
        "Muscular tension in right hand from absorbing 40-ton blow"
      ],
      "stamina_percent": 88,
      "inventory": ["5 Metallic Ring Bands (Right Hand)", "Torn combat poncho"],
      "information_boundary": "Unaware of Lord Malakor's Void Domain or identity"
    },
    "Vesper": {
      "status": "Alive, Combat-Active",
      "health_and_injuries": ["Zero physical damage", "Stamina optimal"],
      "stamina_percent": 95,
      "inventory": ["Dual Tuning-Fork Rapier", "Extracted Calamity Core (held in left pouch)"],
      "information_boundary": "Recognizes the silence as a high-tier domain technique"
    }
  },
  "environment_state": {
    "location": "Sector 7 Canyon",
    "terrain_modifications": [
      "20-foot crater where Obsidian Beast exploded",
      "Spiderweb bedrock fractures under Kaelen's back heel"
    ],
    "atmosphere": "Artificial silence (Shin), air pressure zero"
  },
  "chekhov_guns_and_threads": [
    {
      "id": "CG-01",
      "item_or_mystery": "Extracted Calamity Core in Vesper's pouch",
      "status": "Dormant (Target of interest)",
      "target_payoff": "Rent payment / Source of Malakor's ambush"
    },
    {
      "id": "CG-02",
      "item_or_mystery": "Lord Malakor's half-porcelain mask origin",
      "status": "Introduced (Unresolved mystery)"
    }
  ]
}
```

---

## 3. The Continuous Two-Phase Memory Loop

### Phase A: Pre-Scene Memory Ingestion (Read Before Writing)
Before authoring any new page or chapter:
1. Parse the current `MANGA_STATE_LEDGER`.
2. Check all active characters' injuries, stamina, and current inventory.
3. Validate Information Asymmetry: Ensure no character speaks or acts on knowledge they have not directly witnessed or learned.

### Phase B: Post-Scene State Mutation & Handoff (Write After Finishing)
Immediately after delivering a storyboard:
1. Compute the **State Delta** (What injuries were sustained? What items were used or dropped? How did the terrain change?).
2. Update the `MANGA_STATE_LEDGER` and present it at the end of the chapter delivery.
3. This updated block serves as the immutable ground-truth anchor for the subsequent scene.
