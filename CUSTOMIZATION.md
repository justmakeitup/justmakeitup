# CUSTOMIZATION GUIDE — NEON//IDENTITY SYSTEM

This guide explains how to customize, update, and maintain your **NEON//IDENTITY** GitHub profile.

---

## 1. Fast Track: Publishing to Your GitHub Profile

To make this README visible on your public GitHub profile (`https://github.com/justmakeitup`):

1. **Verify your special profile repository:**
   - Go to [github.com/new](https://github.com/new).
   - Create a repository with your exact username: `justmakeitup`.
   - Set visibility to **Public** and check **Add a README file** (or push this existing directory).
2. **Push the repository files:**
   ```bash
   git init
   git add .
   git commit -m "feat: launch NEON//IDENTITY cyberpunk GitHub profile"
   git branch -M main
   git remote add origin https://github.com/justmakeitup/justmakeitup.git
   git push -u origin main --force
   ```
3. **Check the Live Profile:**
   - Visit `https://github.com/justmakeitup`.
   - Ensure the portrait, all 5 SVGs, and markdown tables render cleanly.

> **Tip on Image Caching:** GitHub uses a proxy service (Camo) to cache images. If you update any SVG or PNG file, increment the version query string in `README.md` (e.g. change `./assets/hero.svg?v=1` to `./assets/hero.svg?v=2`) to force GitHub's cache to refresh immediately.

---

## 2. Modifying Personal Information & Bio

### Editing the Hero Introduction
In `README.md`, locate the table under `### ◈ OPERATOR PROFILE & IDENTITY`:
- Update the headline:
  ```markdown
  <h3>Building thoughtful digital experiences. Exploring technology through practical projects.</h3>
  ```
- Adjust the paragraphs describing your workflow, experience, or tools.

### Editing the Animated Role Ticker in `assets/hero.svg`
Open `assets/hero.svg` in any text editor and find the cycling terminal lines:
```xml
<!-- Slide 1 -->
<g class="anim-c1">
  <text x="28" y="4" fill="#F3F7FA">FOCUS // Building thoughtful digital experiences &amp; clean web apps</text>
</g>
```
You can edit the text inside each slide (`anim-c1` to `anim-c4`) to highlight new roles or interests.

---

## 3. Updating the Project Showcase

Project cards are structured using standard GitHub Markdown tables in `README.md` under `### ◈ FEATURED PRACTICAL PROJECTS`.

To add or update a project, edit the table row:
```markdown
<tr>
  <td>
    <strong>Project Name</strong><br />
    <sub>Subtitle / Category</sub>
  </td>
  <td>
    Clear, factual explanation of architecture, purpose, and key technical achievements.
  </td>
  <td>
    <code>React</code> <code>TypeScript</code><br /><br />
    <a href="https://github.com/justmakeitup/your-repo"><strong>View Repository ↗</strong></a>
  </td>
</tr>
```

---

## 4. Customizing the Technology Stack

1. **In `README.md`:** Update the ASCII table under `### ◈ VERIFIED TECHNICAL MATRIX`.
2. **In `assets/stack.svg`:**
   - Find the `<g transform="translate(420, 60)">` block.
   - Edit the `<text>` nodes inside the chips to add or swap technologies.
   - To keep SVG file sizes small and rendering reliable across all browsers, text chips are used instead of external image dependencies.

---

## 5. Adjusting the Color Palette

All SVG files use consistent hexadecimal color tokens. You can find-and-replace colors across the `.svg` files if you want to alter the aesthetic:

| Role | Color Name | Current Hex | Suggested Alternatives |
| :--- | :--- | :--- | :--- |
| **Canvas** | Obsidian Black | `#080B10` | `#0A0E17`, `#05070A` |
| **Panels** | Deep Graphite | `#111720` | `#131B26`, `#161F2E` |
| **Borders** | Muted Slate | `#18212B` | `#1E293B`, `#263345` |
| **Primary Accent** | Neon Cyan | `#00E5FF` | `#00F0FF`, `#38BDF8` |
| **Secondary Accent**| Electric Teal | `#00FFC6` | `#10FF80`, `#00E676` |
| **Subtle Accent** | Ultraviolet | `#8B5CF6` | `#A855F7`, `#6366F1` |
| **Status Accent** | Magenta Accent | `#FF3CAC` | `#F43F5E`, `#EC4899` |
| **Primary Text** | Ice White | `#F3F7FA` | `#FFFFFF`, `#F8FAFC` |
| **Secondary Text**| Muted Blue-Grey| `#9AA8B7` | `#8B949E`, `#94A3B8` |

---

## 6. Portrait Guidelines

The project enforces a strict **Single Portrait Rule**:
- File: `assets/id.png`
- Format: PNG with alpha or dark neutral background (`#000000`).
- Framing: Head and shoulders cropped approximately to the collarbone or shirt collar.
- Resolution: Square, 800×800 to 1024×1024 px.
- If you ever replace `assets/id.png`, simply save your new image with the exact same filename.
- **Rule:** Never introduce a second character illustration, anime avatar, or secondary face in any other section.
