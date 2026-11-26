# Umbra Duel — Shadows of the Broken Seal

A single-file 2D side-view silhouette martial-arts and weapon fighting game built with **HTML5 Canvas** and **vanilla JavaScript** (zero external libraries, images, or audio files).

## How to Play

1. **Direct Browser Launch:** Open `index.html` directly in any desktop or mobile browser.
2. **Local Server:** Serve the project folder with any static server (e.g., `http://localhost:8080`) and open it in your browser.

---

## Features

- **Procedural Silhouette Rig & Animations:** Forward-kinematics skeleton (`head`, `torso`, `upper/lower arms`, `thighs/calves`, `obi` sash, shadow cape, headgear, and glowing spirit eyes) with smooth keyframe interpolation across idle, walk, jump, crouch, dodge-roll, attacks, block, parry, hit-react, knockdown, get-up, victory, and KO.
- **4 Painted 3-Layer Parallax Arenas:**
  - *Dusk Temple*
  - *Bamboo Forest*
  - *Misty Ruins*
  - *Night Harbour* (including a *Blood Eclipse* boss variant)
- **Combat System:**
  - Limb-level hurtboxes and hitboxes with startup, active, and recovery frames, hitstop, screen shake, directional sparks, ribbon weapon trails, floating damage numbers, and slow-motion final KOs.
  - **4 Weapons** (*Nightfall Katana*, *Twin Viper Fangs* dual daggers, *Whispering Iron Staff*, *Titan Executioner Axe*), each with distinct reach, speed, damage, and **2 unique Rage Specials**.
  - **Defense & Mobility:** Standard block, **Perfect Parry** (tap block right before impact to stun the attacker and gain Rage), and invincible **Dodge-Roll**.
  - **Best-of-3 Rounds** with a 60-second timer and round/KO banners.
- **Game Modes & Progression:**
  - **Campaign:** 8-fight story progression with rising AI difficulty and final boss **Lord Malakor**.
  - **Quick Duel:** Pick your arena, AI difficulty, and opponent weapon.
  - **Shadow Armory:** Spend coins earned from fights to unlock and upgrade weapons & armor (up to Lv 5) and customize your spirit accent glow.
  - **Local Save:** Auto-saves progress in `localStorage` with an automatic in-memory fallback.
- **Procedural Web Audio:** Synthesized whooshes, blade/body impacts, metallic parries, gongs, UI clicks, and an Eastern ambient drone with mute and volume controls.

---

## Controls

### Desktop (Keyboard)
| Action | Keys |
| :--- | :--- |
| Move Left / Right | `A` / `D` (or `Left` / `Right` Arrow) |
| Jump / Crouch | `W` / `S` (or `Up` / `Down` Arrow) |
| Dodge-Roll (Invincible) | Double-tap `A` or `D`, or press `Shift` |
| 3-Hit Punch / Kick | `J` / `K` |
| 3-Hit Light Weapon Slash | `L` |
| Heavy Weapon Cleave | `Back + L`, hold `L`, or `H` |
| Crouch / Air Attacks | `S` + `J`/`K`/`L` or Jump + `J`/`K`/`L` |
| Throw Spirit Kunai | `O`, `J + K`, or `Back + J` |
| Block / Perfect Parry | Hold `I` (tap `I` just before impact to Parry) |
| Weapon Rage Specials (50%+ Rage) | `U` (Special I) / `S + U` or `Back + U` (Special II) |
| Pause | `Esc` or `P` |

### Mobile (Touch)
- Virtual analog joystick on the left + Roll button, with ergonomic action buttons on the right (auto-detected on touch devices or toggled in **Settings**).

---

## Balance & Customization

All gameplay, physics, economy, and AI difficulty constants are grouped at the top of the script in `CONFIG`, `WEAPONS`, `ARMORS`, and `CAMPAIGN_FIGHTERS` inside `index.html`.
