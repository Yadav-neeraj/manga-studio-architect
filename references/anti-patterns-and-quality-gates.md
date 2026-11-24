# Manga & Webtoon Industry Anti-Patterns & Zero-Defect Quality Gates

Derived from reverse-engineering the editorial evaluation standards of *Shueisha (Weekly Shonen Jump / Shonen Jump+)*, *Naver Webtoon*, *Clip Studio Paint EX*, and top diffusion model prompts.

---

## 🚫 The 7 Deadly Sins of Amateur & AI Manga Scripts

### 1. The "Talking Heads" Syndrome (Static Staging)
* **The Flaw:** Characters stand completely motionless, speaking paragraphs of dialogue like a radio drama or podcast.
* **The Professional Fix:** **Active Physical Subtext.** Characters MUST be engaged in physical action while speaking (inspecting a weapon, wrapping knuckles with tape, observing environment, shifting balance, lighting a cigarette, micro-expressions).

### 2. Reading Path & Balloon Flow Breakage
* **The Flaw:** Speech balloons placed arbitrarily across panels or horizontal placement in traditional manga, causing eye-track collisions.
* **The Professional Fix:**
  * **Traditional Manga (Gyaku-Z):** Balloons must strictly flow from **Top-Right to Bottom-Left**. The first speaker’s balloon is always higher and to the right.
  * **Webtoon (Vertical Scroll):** Balloons must flow strictly **Top to Bottom**. Never place critical dialogue side-by-side horizontally across the phone screen.

### 3. Camera Monotony (Chest-Up Shot Hell)
* **The Flaw:** Consecutive panels share the same medium shot distance and flat eye-level camera angle.
* **The Professional Fix:** **The Shot Contrast Rule.** No two consecutive panels may share the same camera distance or angle. Alternate between: Wide Establishing $\rightarrow$ Over-the-Shoulder $\rightarrow$ Extreme Close-Up (Eyes/Hands) $\rightarrow$ Tilted Dutch Angle $\rightarrow$ Worm's-Eye View.

### 4. The Unearned Exposition Dump
* **The Flaw:** Characters loudly explain their magic system, tragic backstory, or the villain's power in dialogue ("As you know, my flame burns at 1000 degrees...").
* **The Professional Fix:** **Show, Don't Tell.** Break exposition into:
  1. *Visual Clues* (cracked ground, sweat drops, steam rising from fingers).
  2. *Internal Monologue Captions* (terse, tactical deductions).
  3. *Opponent Reactions* (fear, calculating eye twitch).

### 5. The Page-Turn Blindspot (Kime-Doma Violation)
* **The Flaw:** Placing the biggest plot twist, monstrous transformation, or finisher strike in the middle of a right-hand page, where peripheral vision spoils it instantly.
* **The Professional Fix:**
  * **Traditional Manga:** Major twists and splash panels MUST be on the **Left-Hand Page (Kime-Doma / 決め駒)** so the revelation hits precisely at the physical page turn.
  * **Webtoon:** Major reveals MUST be preceded by a **Deep Gutter (400px–800px whitespace)** to create the "Scroll-Reveal suspense".

### 6. Visual Drift & AI Hallucination
* **The Flaw:** AI generates different clothes, hair styles, and faces in every panel.
* **The Professional Fix:** **Anchor Token Matrix (Visual DNA Lock).** Every prompt must enforce the character's exact token anchors: `[Name], [Age]yo [Gender], [Fixed Hair Silhouette], [Fixed Eye Color/Shape], [Fixed Signature Attire with exact color/texture]`, plus consistent negative prompt filters.

### 7. Weak / Generic SFX (Sound Effects)
* **The Flaw:** Using English comic book words like "BOOM" or "SLASH" that lack tactile Japanese manga weight.
* **The Professional Fix:** Authentic drawn-in **Japanese Katakana Onomatopoeia** (e.g., ゴゴゴゴ for menacing dread, ドドドド for rumbling ground, バン for sudden explosive impact, ズザザザ for gravel friction skids).

---

## ✅ The 6 Zero-Defect Quality Gates (Mandatory Checklist)

Before releasing any Manga / Webtoon storyboard, verify every gate:

| Gate | Check Question | Pass Condition |
| :--- | :--- | :--- |
| **Gate 1: Reading Path** | Does the dialogue order follow Gyaku-Z (Manga) or Top-Down (Webtoon)? | No eye-path zigzags or balloon overlaps. |
| **Gate 2: Camera Diversity** | Do any two adjacent panels share the same shot type or angle? | 100% variety in shot distance and perspective. |
| **Gate 3: Physical Staging** | Are characters physically acting or moving while speaking? | Zero static talking heads. Active verbs in every panel. |
| **Gate 4: Climactic Placement** | Is the climax placed on the page turn or after a deep scroll gutter? | Maximum element of surprise and impact. |
| **Gate 5: Authentic SFX** | Does every action panel include authentic Japanese Katakana SFX? | Katakana + Romaji + drawn-in visual direction included. |
| **Gate 6: AI Reproducibility** | Do all prompts contain full Visual DNA anchors and negative prompts? | Character consistency locked across panels. |
