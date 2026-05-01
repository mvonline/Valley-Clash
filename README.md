# Valley Clash

A browser-based fan tribute fighting game: **stylized vector likenesses, original procedural art only**. Masters from the Valley of Peace and beyond. **Not affiliated with DreamWorks.**

## Quick start

Open **`index.html`** in a modern browser and pick a build:

| File | Description |
|------|-------------|
| [`kfp-valley-clash.html`](kfp-valley-clash.html) | **Canvas 2D** — single file, no extra dependencies. |
| [`kfp-valley-clash-pixi.html`](kfp-valley-clash-pixi.html) | **Pixi.js** — same gameplay; arena is drawn to an offscreen 2D canvas and composited via Pixi (GPU). Loads Pixi from an ESM CDN (needs network). |

If the page is opened as a local file (`file://`), some browsers restrict modules or audio; for Pixi builds, a tiny local server works best.

## Game modes

- **Arcade — 1P vs CPU** — You pick a master; the CPU gets a random rival and the match starts immediately.
- **Local versus — 2P** — Player 1 selects a warrior, then Player 2 selects a different one, then **Fight**.
- **How to play & combos** — In-game reference for controls and combo rules.

**Match rules:** First to **two round wins**. Blocking reduces damage. Each round opens with a **3-2-1** countdown, then **FIGHT!**

**Audio:** Procedural sound effects and looping background music (Web Audio). If you hear nothing, tap / click / press a key once (browser autoplay policies).

## Controls

| | Move | Jump | Block | Punch | Kick |
|---|------|------|-------|-------|------|
| **Player 1** | `A` / `D` | `W` | Hold `S` | `J` | `K` |
| **Player 2** | `←` / `→` | `↑` | Hold `↓` | `V` | `B` |

Player 2 may also use **numpad `4`** (punch) and **`5`** (kick), mapped the same as `V` / `B`.

## Combos

Every fighter has **two unique three-step chains**. On the **ground**, while **idle** (or leaving block into idle), press the sequence in order; the **final** step triggers a **signature special** (big damage and hitbox).

Internally, combos are defined with **punch = J** and **kick = K**. **Player 1** uses **`J` / `K`** on the keyboard. **Player 2** uses **`V` / `B`** (same roles: **V** = punch, **B** = kick). On **character select** in **2P mode**, after Player 1 has locked in, the combo list shows **`V` / `B`** for the player who is choosing.

The table below lists sequences in **Player 1 notation** (`J` / `K`). For Player 2, substitute **J → V** and **K → B**.

---

## Roster (26 fighters)

| Character | Title | Style (short) | Combo 1 | Combo 2 |
|-----------|-------|---------------|---------|---------|
| **Po** | Dragon Warrior | Grappler — messy power | Dumpling Rush — `J → J → K` | Skadoosh Palm — `K → J → J` |
| **Zhen** | Street Fox | Trickster — feints & speed | Alley Fake-out — `J → K → J` | Tail Trip — `K → K → J` |
| **Shifu** | Master | Technical — precise control | Pressure Point Barrage — `J → J → J` | Cane Cyclone — `K → J → K` |
| **Tigress** | Furious Five | Striker — long limbs | Talon Flurry — `J → K → K` | Thunder Sweep — `K → J → K` |
| **Monkey** | Furious Five | Aerial — unpredictable arcs | Drunken Branch — `J → K → J` | Banana Brawl EX — `J → J → J` |
| **Crane** | Furious Five | Zoner — spacing | Feather Fan — `K → J → J` | Crane Dive — `J → K → K` |
| **Viper** | Furious Five | Mixer — constriction | Ribbon Bind — `J → K → J` | Fang Spiral — `K → K → K` |
| **Mantis** | Furious Five | Rush — hyper speed | Praying Fury — `J → J → K` | Thousand Cuts — `J → K → J` |
| **Tai Lung** | Fallen Master | Pressure — brutal snow strikes | Iron Strike Chain — `J → K → J` | Leap of Legend — `K → J → J` |
| **The Chameleon** | Shifting Tyrant | Morph — trick hitboxes | Mirror Dash — `J → J → K` | Form Breaker — `K → K → J` |
| **Kai** | General of the Jade | Brute — chain reach | Jade Hook Grapple — `J → K → J` | Oblivion Sweep — `K → J → K` |
| **Oogway** | Valley Founder | Balancer — no wasted motion | Peach Blossom Palm — `J → J → K` | Stillness Fall — `K → K → K` |
| **Li Shan** | Panda Chief | Protector — throws & hugs | Father Bear Hug — `K → J → J` | Village Toss — `J → K → K` |
| **Mei Mei** | Ribbon Dancer | Flow — spin entries | Noodle Spiral — `J → K → J` | Ribbon Vault — `K → K → J` |
| **Thundering Rhino** | Master Council | Tank — forward momentum | Horn Line Drive — `J → J → J` | Council Crash — `K → J → K` |
| **Storming Ox** | Master Council | Wall — counter spikes | Iron Wall Bash — `K → J → J` | Stampede Turn — `J → K → J` |
| **Master Croc** | Bandit Turned Master | Snap — tail logic | Death Roll Chain — `K → K → J` | River Snap — `J → J → K` |
| **Master Chicken** | Bravest Master | Panic — lucky punishes | Fluster Flurry — `J → K → K` | Plucking Finale — `K → J → J` |
| **Lord Shen** | Cannon Throne | Blade wings — spacing | Throne Skewer — `J → K → J` | Cannon Waltz — `K → K → K` |
| **Wolf Boss** | Pack Alpha | Rushdown — pack pressure | Pack Rush — `J → J → K` | Alpha Trip — `K → J → K` |
| **Soothsayer** | Canyon Oracle | Trickster — reads your pattern | Horoscope Fake — `K → J → J` | Canyon Circle — `J → K → J` |
| **Mr. Ping** | Noodle Sage | Spacing — ladle range | Secret Ingredient — `J → J → J` | Ladle Arc — `K → K → J` |
| **Fung** | Croc Mercenary | Dirty — command grab bias | Laughing Grab — `J → K → K` | Mercenary Bite — `K → J → K` |
| **Master Porcupine** | Needle Palm | Chip — constant pokes | Needle Volley — `J → J → K` | Quill Cage — `K → K → K` |
| **Master Elephant** | Master Council | Giant — screen control | Trunk Cannon — `K → J → J` | Quake Stomp — `J → K → J` |
| **Jade Warrior** | Spirit Thrall | Ghost tempo — slip hits | Jade Blink — `J → K → K` | Thrall Rush — `K → J → K` |

Each row’s **Style** line in the game also has a slightly longer blurb on the select screen (hover the card).

### Roster note (art reuse)

Some later-film characters **reuse** another fighter’s procedural silhouette for visuals (`spriteAs`) while keeping **unique** stats and combos. Gameplay and combo tables above are **per character**; only the in-fight drawing may match another master’s shape.

---

## Tech snapshot

- Single-page **HTML + inline JavaScript**.
- **Canvas** build: one `<canvas>` for the arena.
- **Pixi** build boots WebGL via Pixi and blits the same logical frame.

Enjoy the Valley Clash.
