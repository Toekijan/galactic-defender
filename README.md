# 🚀 GALACTIC DEFENDER (Galaga-Inspired Pixel-Art Shmup)

A retro arcade shoot-'em-up mini-game reminiscent of classic **Galaga (1981)**, built with vanilla HTML5 Canvas and the Web Audio API.

---

## 🕹️ How to Play

Open `index.html` directly in any modern web browser (Chrome, Edge, Firefox, Safari).

### Controls
| Input | Action |
|---|---|
| <kbd>←</kbd> <kbd>→</kbd> or <kbd>A</kbd> <kbd>D</kbd> | Move Fighter Left / Right |
| <kbd>Space</kbd> or <kbd>Z</kbd> / <kbd>K</kbd> | Fire Dual Lasers |
| <kbd>S</kbd> | Toggle Game Speed (`SLOW`, `NORMAL`, `FAST`) |
| <kbd>P</kbd> | Pause / Resume Game |
| <kbd>M</kbd> | Mute / Unmute 8-Bit Audio |
| <kbd>C</kbd> | Toggle CRT Scanline Shader Effect |
| **Touch / Mouse** | On-screen Virtual Arcade Pad (`LEFT`, `RIGHT`, `FIRE`) & Header Buttons (`SPD`, `CRT`, `SND`, `PAD`) |

---

## 👾 Features & Mechanics

1. **Formation Flight & Dive-Bombing Runs**:
   - Enemies fly into screen in coordinated squads using smooth **Cubic Bézier Curves**.
   - The alien fleet "breathes" and sways horizontally while in formation.
   - Attack waves break formation to dive-bomb towards the player's coordinates while aiming lasers downward.
   - Off-screen diving enemies re-enter from the top and dock back into the fleet.

2. **Alien Fleet**:
   - **Boss Galaga (Green / Blue)**: Takes 2 hits to eliminate! Turns damaged blue on first strike. Awards 150 pts in formation or 400 pts during a dive. Often accompanied by escort butterflies.
   - **Butterfly (Red)**: Fluttering escorts. Awards 80 pts in formation or 160 pts diving.
   - **Bumblebee (Yellow)**: Nimble vanguard scouts. Awards 50 pts in formation or 100 pts diving.

3. **Dual Fighter Power-Up**:
   - Defeating a diving Boss Galaga has a chance to drop a **Power Core**.
   - Collecting it docks an adjacent twin starship, enabling **4 simultaneous laser cannons** and doubled firing width!
   - Taking a hit while in Dual mode sacrifices the twin ship and leaves your core fighter alive.

4. **Authentic 8-Bit Synthesizer (Web Audio API)**:
   - Zero external audio files or dependencies.
   - Procedural sounds: laser zaps, enemy dive warbles, metallic hits, explosions, stage fanfare, and game-over themes.

5. **Arcade Presentation**:
   - 3-Layer parallax starfield with hyper-speed warp transitions.
   - Pixel particle explosions & floating point popups.
   - CRT scanline & curved bezel shader overlay (toggleable).
   - High score persistence via `localStorage`.
   - End-of-game Galaga combat report (Shots Fired, Hits, and Hit Ratio %).
