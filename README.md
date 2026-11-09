# Samurai vs Zombies: Sacred Chronicles

A comprehensive, feature-complete 2D horizontal lane-defense game inspired by *Samurai vs Zombies Defense*, built with **single-file HTML5 Canvas, modern CSS, and modular vanilla JavaScript (zero external dependencies)**.

Featuring rich procedural vector-rendered graphics, high-contrast silhouettes, a branching overworld campaign map, unique unit combat abilities, a consumable battle belt pouch, and a persistent upgrade economy.

---

## 🎮 How to Play

Open [`index.html`](file:///C:/Users/nicho/.gemini/antigravity/scratch/samurai-vs-zombies/index.html) directly in any modern web browser, or launch it from PowerShell:
```powershell
Start-Process "C:\Users\nicho\.gemini\antigravity\scratch\samurai-vs-zombies\index.html"
```

### Controls
* **Hero Locomotion & Kiting:**
  * `A` / `Left Arrow` (or on-screen `◀ RETREAT` button): Move left toward the Sacred Village Gate. Holding Left while facing oncoming enemies performs a **tactical retreat** (firing backward at a 20% movement speed penalty).
  * `D` / `Right Arrow` (or on-screen `ADVANCE ▶` button): Advance right toward the Cursed Demon Portal.
  * **Double-Tap `A` or `D` (or press `SPACE`):** Trigger **Flash Step (Dodge Roll)** with invulnerability frames once unlocked in the Dojo.
* **Smart Proximity Combat System:**
  * **Close Quarters (≤ 110px):** Automatic Katana 3-hit combo chain with escalating damage and screen-shake finisher.
  * **Ranged Zone (110px – 480px):** Automatic Yumi longbow stance, calculating parabolic ballistic trajectory with gravity drop.
* **Allied Troop Deployment (Leadership Spirit):**
  * `[1]` **Peasant Militia (15 Spirit):** *Panic Pitchfork* (20% chance on hit to inflict fear, causing zombies to flee backward for 1.5s).
  * `[2]` **Yari Spearman (35 Spirit):** *Spear Wall Formation* (When 3+ spearmen cluster together, they lock shields, gaining +40% armor and knocking back foes).
  * `[3]` **Imperial Bowman (50 Spirit):** *Flaming Volley* (Every 4th shot shoots a flaming arrow that creates a ground fire patch dealing DoT for 3s).
  * `[4]` **Armored Daimyo Guard (80 Spirit):** *Iron Cleave & Taunt* (Massive 1.4x silhouette; greatsword cleaves up to 4 foes while roaring to force nearby enemies to attack him).
  * `[5]` **Shrine Maiden / Miko (95 Spirit):** *Purifying Radiance* (Emits a continuous golden aura healing all allies within 160px for 5% max HP every 2s and cleansing debuffs).
* **Consumable Battle Belt Pouch:**
  * `[Z]` or `[6]` **Sacred Sake Gourd:** Instantly heals 60% max HP and grants 3s knockback immunity.
  * `[X]` or `[7]` **Onigiri Bento:** Instantly refills +50 points of Leadership Spirit.
  * `[C]` or `[8]` **Kagutsuchi Fire Bomb:** Throws a bomb exploding into a blazing wall of fire on the ground (6s duration).
  * `[V]` or `[9]` **Kami Time Talisman:** Freezes all undead units in ice crystals for 4.5 seconds.
* **Hero Active Skills:**
  * `[Q]` **Katana Dash (12s CD):** 300px invulnerable dash cleaving all enemies in path for 300% damage.
  * `[W]` **Arrow Hail (18s CD):** Volley of 20 fiery arrows plunging from the sky over a 400px zone.
  * `[E]` **War Cry (25s CD):** Grants +50% movement speed and +40% attack damage to all active allies for 8s.
* **System Controls:**
  * `[M]` Toggle synthesized Taiko/Shamisen background rhythm.
  * `[P]` Pause / Resume.

---

## 🗺️ Overworld Campaign Node Map
Between battle encounters, explore an interactive parchment map with branching routes:
* **Main Battle Gate:** Mandatory defensive stage defending against horde pushes.
* **Sacred Bamboo Grove (Challenge Node):** High-difficulty wave of swift Ninja & Ghouls awarding **2x Demon Soul Gems**.
* **Traveling Tea Merchant (Shop Node):** Stock up on battle consumables (Sake, Bento, Fire Bombs, Time Talismans).
* **Hidden Shrine (Blessing Node):** Choose 1 of 4 permanent run blessings (Wind Stride, Divine Edge, Spirit Font, Iron Vitality).
* **Boss Nodes:**
  * *The Ashen Citadel:* Encounter the **Red Oni Warlord** mini-boss wielding a spiked Kanabo.
  * *Rift of the Corrupted Kyubi:* The **Nine-Tailed Fox Demon Boss** floating in air and casting spectral hellfire orbs!

---

## 👹 Monster Horde Archetypes
1. **Rotting Ashigaru (Zombie Peasant):** Swamp-green skin, violet loincloth, glowing yellow eyes, melee bites.
2. **Cursed Shadow Ninja:** Pitch-black silhouette, glowing cyan eyes, erratic smoke puff evasion, dual purple kunai.
3. **Blight Spitter:** Bloated purple corpse carrying a rotting ballista that launches dripping green acid pools onto the ground.
4. **Armored Skeletal Samurai:** Exposed stark-white ribcage over rusted armor, parries attacks, drags a chipped nodachi blade.
5. **Red Oni Warlord (Mini-Boss):** Muscular crimson demon twice the height of the hero; slams his spiked Kanabo for a 180px AOE shockwave.
6. **Corrupted Kyubi (Final Campaign Boss):** Nine-tailed spectral fox demon radiating purple spiritual flames, floating mid-air, casting homing hellfire orbs.

---

## ⛩️ Persistent Dojo & Blacksmith
Spend accumulated Gold Coins and Demon Soul Gems:
* **Samurai:** Katana Honing, Compound Bow Crafting, Master O-Yoroi Plate, Flash Step (Dodge Roll).
* **Village & Spirit:** Command Horn (increases max Leadership capacity to 250 and boosts passive regen), Sacred Village Gate (fortifies Gate HP and adds automated rooftop archers).
* **Allied Units:** Level up Peasant Militia, Yari Spearmen, Imperial Bowmen, Daimyo Guards, and Shrine Maidens to Tier 5.
* **Belt Pouch Restocks:** Purchase Sake Gourds, Bento Boxes, Fire Bombs, and Time Talismans.

---

## 🔊 Dynamic Web Audio API Sound
* 100% procedurally synthesized in real time:
  * Crisp sword slashes and resonant parry clinks.
  * High-tension bow twangs and arrow hit thuds.
  * Low-frequency bass rumble for Kanabo slams and Fire Bomb explosions.
  * Shimmering Kagura bell chimes and ice freeze effects.
  * Rhythmic procedural Taiko drum cadence and Shamisen arpeggios in the Japanese Hirajōshi pentatonic scale.
