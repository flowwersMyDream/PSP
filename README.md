# MCPSP — Minecraft PSP: Changelog

A portable port of **Minecraft Pocket Edition (v0.6.1)** for the PlayStation Portable — runs on every PSP model (including the 32 MB PSP-1000) and in PPSSPP.

---

## Latest Build — Fishing Update

The entire fishing feature, from Creative menu to the catch, is now finished and polished:

### 🎣 Fishing

- **Creative inventory** — the fishing rod now appears in the *Tools & Combat* tab (it was missing entirely before).
- **Proper rod icon** — the old 16×16 inventory icon was practically blank; it now has a real pixel-art fishing rod.
- **Custom player-made textures:**
  - `fishing_rod.png` — idle rod in hand (with float),
  - `fishing_rod_cast.png` — cast pose,
  - `fish.png` (raw cod) and `fish_cooked.png` (tropical fish) — what you actually catch.
- **Dynamic rod pose** — the rod switches to the *cast* texture while your bobber is out in the world and back to the *idle* pose the moment you reel in.
- **Real fishing gameplay:**
  - Splash sound and effect only play when the bobber lands in **water** — no more phantom splashes on dry land;
  - the bite timer only counts down while the bobber is in water;
  - fair, snappy bite times (2–12 seconds) instead of the old 3–30 s;
  - a clearer bite animation — the bobber sinks over 2 seconds with bubbles so you can't miss it;
  - **press `L` to cast**, **press `L` again to reel in and catch**.
- **New in-game instruction text** that tells you exactly how to fish.

### 🔧 Fixes

- **Grass texture restored** — the grass block edge now matches the original MCPE texture; the broken grass-on-dirt look is gone.
- Creative-tab placement of the fishing rod corrected so it shows up in the right category.

---

## Previous Updates

### 💎 Emerald Content

- **Emerald Ore in the world** — emerald ore now generates naturally while the world is created. Dig deep to find those shiny green gems.
- **Emerald Armor set** — a full set of emerald chestplate, helmet, leggings and boots. Protection you can feel, style you can show off. Craft it and be unstoppable.
- **Diamond Hopper** — a shiny funnel-block with its own little 9-slot storeroom inside. Vacuum up dropped items, keep them safe, and empty them whenever you want.

### ⛏️ 3×3 Pickaxe Mining

- Mining now digs a **3×3 area at once**. Faster tunnels, faster caves, faster fun.

### 🍎 Hunger, Skins & Inventory

- **Real hunger, just like Minecraft** — eat an apple or a warm cooked steak to refill your hunger bar; once you are well fed your health quietly heals on its own.
- **Player skins** — a whole little wardrobe to pick from. Step into the world looking exactly how you want.
- **A cozy new inventory** — a fresh, soft background hugs every item you carry, so sorting your treasures feels like a warm hug.

### 🌍 World & Modes

- **Flip between Survival and Creative** — switch any world between modes whenever you like. Play your way, always.
- **Full Bright** — turn it on and let the whole world glow like golden hour that never ends. No more scary dark corners.

### 🌐 Languages

- **English & Russian** — the whole game speaks your language; switch in Options.
- **PyskiEnglish (RU-Latin)** — Russian words written with Latin letters.
- **Nyashka mode** — a warm, fully translated cute language mode, finished with a little heart.
- Every screen, every button, every little note is translated.

### 💖 Extras

- **Credits screen** — made with love: a special thank-you card inside the game.
- **News & Updates screen** — exactly this menu in-game, written with care and a sprinkle of cuteness; open it any time from the main menu.
- A whole lot of care went into this port — every block, every pixel, every fix.

---

## Notes

- Keep `EBOOT.PBP` and the `data/` folder together.
- Worlds save into a `saves/` folder next to the EBOOT.
