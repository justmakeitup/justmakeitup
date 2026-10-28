# NEON//IDENTITY SYSTEM — MASTER BUILD PROMPT

## Role & Mission
Act as a senior GitHub profile designer, cyberpunk art director, SVG motion designer, frontend developer, and personal-brand strategist.

Design and generate a complete, distinctive, professional cyberpunk GitHub profile README and self-contained SVG asset suite for **Ranit Das** (`justmakeitup`).

---

## Core Visual Identity
- **Design Philosophy:** Professional first, cyberpunk second. Technically credible, recruiter-friendly, sophisticated, and dark-mode native.
- **Palette:**
  - Obsidian Black: `#080B10`
  - Deep Graphite: `#111720`
  - Muted Panel Grey: `#18212B`
  - Neon Cyan Accent: `#00E5FF` (Primary)
  - Electric Teal Accent: `#00FFC6` (Primary)
  - Ultraviolet: `#8B5CF6` (Subtle)
  - Controlled Magenta: `#FF3CAC` (Subtle)
  - Ice White Text: `#F3F7FA`
  - Muted Secondary Text: `#9AA8B7`
- **Visual Elements:** Fine technical grids, thin cyan borders, coordinate markings, subtle gradient glows, clean monospace metadata, and restrained SVG animations.

---

## Critical Identity & Portrait Constraints
1. **Exactly ONE authentic portrait:** `assets/id.png` (authentic head-and-shoulders portrait of Ranit Das cropped to the collar, professional shirt/jacket with subtle cyber rim lighting).
2. **Zero duplicate faces or character illustrations:** No anime, no avatars, no pointing character (`right_pointing.png` eliminated), no secondary portraits across any section or inside any SVGs.
3. **Factual Integrity:** Represent all skills, projects, and technologies with 100% honesty. Explicitly document AI-assisted development workflows (Antigravity, ChatGPT). No fabricated metrics, awards, or fake star counts.

---

## Deliverable Architecture
```text
.
├── README.md              # Complete GitHub-flavored Markdown document
├── assets/
│   ├── id.png             # The single authentic collar-level portrait
│   ├── hero.svg           # Cyberpunk identity header with cycling role ticker
│   ├── about-life.svg     # Architecture & methodology + 3-slide exploration carousel
│   ├── stack.svg          # Triple orbital hub + grouped verified stack chips
│   ├── id-dashboard.svg   # Suspended lanyard ID with microchip schematic & barcode
│   └── connect.svg        # Central station network uplink to communication channels
├── preview/
│   └── index.html         # Local preview testbed with desktop/mobile view toggles
├── PROMPT.md              # Master generation prompt & design specs
├── CUSTOMIZATION.md       # Detailed guide for customizing content, assets, and styling
├── README-QA.md           # Validation checklist and test verification results
└── ranit-github-profile.zip # Complete upload-ready archive
```

---

## SVG Engineering Guidelines
- 100% self-contained valid XML.
- Namespaced IDs per file (`hero-*`, `abt-*`, `stk-*`, `dash-*`, `conn-*`) to prevent collision.
- SMIL + CSS animations only (zero JavaScript, zero `foreignObject`).
- Fallback base state at 0s for viewers with animation disabled.
- Respect `@media (prefers-reduced-motion: reduce)`.
