# MCPSP — Minecraft PSP FORK BY SASHKA: Changelog

DOWNLOAD GAME https://workupload.com/file/sgg8j3rSvDt ( game file size 75 mb, Yowza, that’s a big file. Try again with a file smaller than 25MB)

A portable port of **Minecraft Pocket Edition (v0.6.1)** for the PlayStation Portable — runs on every PSP model (including the 32 MB PSP-1000) and in PPSSPP.

---

## Latest Build — Fishing Update + Fixes

The entire fishing feature, from Creative menu to the catch, is now finished and polished — together with the fixes we bumped into along the way:

### 🟩 Grass Fix

- **Починка травы** — restored the original grass block edge straight from the upstream terrain atlas (removed the broken "grass-on-dirt" look). The grass block now matches MCPE exactly, and the hidden **Epic Lucky Block** texture stayed perfectly intact.

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

### 🔧 Other Fixes

- Creative-tab placement of the fishing rod corrected so it shows up in the right category.

---

## Previous Updates

### 💎 Emerald Content

- **Emerald Ore in the world** — emerald ore now generates naturally while the world is created. Dig deep to find those shiny green gems.
- **Emerald tool set** — a full set of emerald tools: sword, pickaxe, shovel, axe and hoe — tougher and shinier than diamond.
- **Emerald Armor set** — a full set of emerald chestplate, helmet, leggings and boots. Protection you can feel, style you can show off. Craft it and be unstoppable.
- **Diamond Hopper** — a shiny funnel-shaped block with its own 9-slot storeroom inside. Drop items next to it and it vacuum-sucks them up automatically, keeps them safe, and lets you take them back out any time through its own inventory screen. Craft it, place it, and it will catch everything that falls your way.

### 🌈 Rainbow Content

- **Rainbow Ore in the world** — a brand new rainbow ore generates while the world is created and drops **Rainbow Crystals**.
- **Rainbow tools & armor** — a whole rainbow set: sword, pickaxe, shovel, axe, hoe, and a full armor outfit. Crafted from Rainbow Crystals.
- **Block of Rainbow** — store your crystals in style.

### 🎲 Lucky Blocks

- **Lucky Block** — break it and get a surprise: a random piece of loot (diamonds, emerald gems, rainbow gems, tools, food and more) — and sometimes a mob pops out to say hi!
- **Epic Lucky Block** — the big brother: spits out 2–4 rewards at once. Epic loot like emerald armor, diamond swords, cakes, gold and diamond blocks — or a whole group of mobs. High risk, high reward.

### ⛏️ 3×3 Pickaxe Mining

- Mining now digs a **3×3 area at once**. Faster tunnels, faster caves, faster fun.

### 🧟 Mobs & Spawning

- **Natural mob spawning** — animals (sheep, pigs, chickens, cows) and monsters (zombies, skeletons, spiders, creepers) spawn around the world, day and night — with weights, spawn clusters and sensible caps just like the real game.
- **Monster Spawner** — a cage block that grinds out monsters while you're nearby; it generates inside the world's dungeons and can also be grabbed from the Creative menu.
- **Generated dungeons** — the world generator hides underground rooms with a Mob Spawner in the middle and chests with loot. Go find them!

### 🍎 Hunger, Skins & Inventory

- **Real hunger, just like Minecraft** — eat an apple or a warm cooked steak to refill your hunger bar; once you are well fed your health quietly heals on its own.
- **Player skins** — a whole little wardrobe to pick from. Step into the world looking exactly how you want.
- **A cozy new inventory** — a fresh, soft background hugs every item you carry, so sorting your treasures feels like a warm hug.

### 🌍 World, Weather & Modes

- **Flip between Survival and Creative anytime** — open the Worlds list, press **Square** on any world and pick Survival or Creative with the Left/Right + Cross pills. No re-creating worlds, no progress loss — flip your very own way.
- **Real weather** — the world cycles through clear skies, **rain** and **storms** with their own lengths; storms trigger **lightning strikes** that strike near you with a bright flash and a boom, and can set the ground on fire. Weather is a per-world option in the world generator.
- **Snowy climates** — cold biomes build up **snow layers**, just like the real game.
- **Full Bright** — turn it on and let the whole world glow like golden hour that never ends. No more scary dark corners.
- **Sleep in a bed** — click a bed at night and sleep until dawn; it becomes your new respawn point too.

### 🌐 Languages

- **English & Russian** — the whole game speaks your language; switch in Options.
- **PyskiEnglish (RU-Latin)** — Russian words written with Latin letters.
- **Nyashka mode** — a warm, fully translated cute language mode, finished with a little heart.
- Every screen, every button, every little note is translated.

### 💖 Extras

- **Credits button** — a dedicated *Credits* entry in **Options → Game** (reached right from the Game category) opens a full auto-scrolling credits screen, dedicated to the people who made the port.
- **News & Updates screen** — the in-game change log; open it any time from the main menu to see what's new.
- **Hidden easter egg** — something secret is waiting for those who hold the right buttons in-game. Find it!
- A whole lot of care went into this port — every block, every pixel, every fix.

### ⚡ Optimization

- **Fits on a 32 MB PSP-1000** — the whole world stays in RAM thanks to a compact storage: block IDs, block data and lighting are packed per-chunk instead of per-block. A ~20 MB world takes about 4 MB, which is what makes the full map playable on the little PSPs.
- **Streaming renderer** — only the mesh columns near the camera are drawn; the world around you builds lazily as you explore instead of all at once.
- **Dual-threaded world generation** — terrain is generated on a separate worker thread, so the menu stays responsive while a world builds or saves.
- **Mipmapping + texture atlas** — distance shimmering is handled with mip levels that generate automatically, and the fast GE-as-VRAM path keeps texture switches cheap.
- **Fast memory routines** — VFPU-accelerated memcpy is used where it counts, keeping frame times steady.
- **Quality/performance knobs** — view distance, clouds, leaves, particles, smooth lighting, mipmapping and dithering are all adjustable in Options, with sensible auto-neutered defaults on low-memory PSPs.

---

## Notes

- Keep `EBOOT.PBP` and the `data/` folder together.
- Worlds save into a `saves/` folder next to the EBOOT.
