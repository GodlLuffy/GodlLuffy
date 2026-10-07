# ⚡ GodlLuffy — Futuristic Developer Profile // Setup & Layout Guide

This repository contains your custom, production-grade GitHub Profile README inspired by **Udit Gupta's (`Ug0510`) Redline v4 design language**, customized for **Anup Gundelwar (`@GodlLuffy`)**.

---

## 📁 Project Structure

```bash
Profile/
├── README.md               # Master GitHub Profile markdown
├── LAYOUT_GUIDE.md         # This customization & deployment manual
└── assets/                 # Bespoke high-octane animated SVG banners
    ├── hero.svg            # Cyber HUD Header with role carousel & avatar scanner
    ├── about-life.svg      # Philosophy cards + 3-slide animated feature showcase
    ├── stack.svg           # Orbital constellation graph + categorized tech cards
    ├── id-dashboard.svg    # 3D swinging lanyard ID badge + GitHub metrics dashboard
    └── connect.svg         # High-contrast interactive connection cards
```

---

## 🚀 How to Publish to Your GitHub Profile

Since GitHub renders the special repository with the same name as your username (`GodlLuffy/GodlLuffy`) on your public profile:

1. **Open your repository:** [github.com/GodlLuffy/GodlLuffy](https://github.com/GodlLuffy/GodlLuffy)
2. **Push or upload these files:**
   - Commit the `assets/` folder (with all 5 SVGs: `hero.svg`, `about-life.svg`, `stack.svg`, `id-dashboard.svg`, `connect.svg`).
   - Commit `README.md` into the root of the repository.
3. **Using Git CLI (Recommended):**
   ```bash
   # In this directory:
   git init
   git remote add origin https://github.com/GodlLuffy/GodlLuffy.git
   git branch -M main
   git add README.md assets/
   git commit -m "feat: futuristic cyber-obsidian developer profile v4"
   git push -u origin main --force
   ```
4. View your profile at **`https://github.com/GodlLuffy`** — your dark-mode cyber developer dashboard will immediately come alive!

---

## 🎨 Theme & Color Palette Matrix

| Token | Hex Code | Usage |
| :--- | :--- | :--- |
| **Obsidian Dark** | `#050811` / `#070c1a` | Deep canvas & background base |
| **Glass Card Fill** | `#091322` / `#0b172a` | Sleek developer cards & badges |
| **Card Border** | `#1d3b63` / `#247bff` | Low-friction structural outlines |
| **Electric Blue** | `#247bff` / `#3d93ff` | Primary tech accents & highlights |
| **Neon Cyan** | `#00f0ff` | Terminal prompts, status indicators & glows |
| **Cyber Crimson** | `#ff3366` | Slogan badges, alerts, active states |
| **Slate Text** | `#88a5cc` / `#9db6d8` | Secondary copy & technical monospace |
| **Crisp White** | `#f0f5ff` | Primary titles & high-contrast headings |

---

## 🛠️ Customization Guide

### 1. Updating Your Avatar Photo
In `assets/hero.svg` and `assets/id-dashboard.svg`, look for:
```xml
<image href="https://avatars.githubusercontent.com/u/198222047?v=4" ... />
```
- Replace the URL with your preferred image URL, or add a local file like `./assets/avatar.png` and reference `href="./assets/avatar.png"`.

### 2. Customizing Roles in the Hero Carousel
In `assets/hero.svg`, lines `135-165`:
You will find 4 distinct animated `<g>` groups. Edit the text inside:
```xml
<text x="56" y="438" ...>⚡ Creative Frontend & 3D Developer</text>
<text x="56" y="438" ...>🚀 Full-Stack Web & App Architect</text>
<text x="56" y="438" ...>📱 Cross-Platform Mobile Engineer (Flutter)</text>
<text x="56" y="438" ...>✨ UI/UX & 60FPS Micro-Animations Crafter</text>
```

### 3. Modifying Your Tech Stack
In `assets/stack.svg`:
- **Orbital Satellites:** Modify lines `80-140` to change the center satellites (JS, TS, React, Flutter, 3D, Node).
- **Tech Cards:** Modify the categorized cards in sections `01 // CORE LANGUAGES`, `02 // FRONTEND & 3D`, and `03 // BACKEND & MOBILE`.

### 4. Updating GitHub Live Stats Parameters
In `README.md`, you can tweak the query parameters for your live SVG cards:
```markdown
https://github-readme-stats.vercel.app/api?username=GodlLuffy&show_icons=true&theme=tokyonight&bg_color=070b16&title_color=247bff&text_color=adbed8&icon_color=00f0ff&border_color=193057
```
- `bg_color`: Custom card background (`070b16`)
- `title_color`: Header title color (`247bff`)
- `icon_color`: Icon glow color (`00f0ff`)
- `border_color`: Card border stroke (`193057`)

### 5. Busting GitHub's Image Cache
GitHub uses a caching proxy (`camo.githubusercontent.com`). If you ever update any SVG in `assets/` and GitHub still displays the old version, simply append `?v=2` to the image tag in `README.md`:
```markdown
<img src="./assets/hero.svg?v=2" width="100%" />
```

---

<sub>Engineered with precision for GodlLuffy. Ready for deployment.</sub>
