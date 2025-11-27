# 🚢 Battle_Simulator · C Naval Warfare Sim

On-chain vibes in an off-chain world.

This is an **Advanced Naval Battle Simulator** I built in **Year 1 / Sem 1 – Programming Methodology** using pure **C** (no AI, no VS Code magic, no Git knowledge at the time). I only knew GitHub existed, so I uploaded the finished project later as proof-of-work.

The sim models a WW2-style battlefield where a **battleship (B)** fights multiple **escort ships (E)** on a 2D grid. Ships have different guns, angle ranges, shell speeds and impact power. All attacks use **real physics** – projectile motion, time-of-flight, range equations and damage accumulation. :contentReference[oaicite:0]{index=0}

---

## ✨ Core Features

- 🎯 Grid-based naval battlefield (square canvas)
- 🚢 Single battleship vs many escort ships
- 🔫 Projectile motion with physics:
  - launch angle  
  - initial velocity  
  - range & hit calculations  
- 💥 Hit / miss & impact power per ship type
- 📊 Damage % accumulation on the battleship
- 🔁 Multiple simulation modes:
  - static battlefield  
  - battleship moving through waypoints  
  - gun jam with restricted angles  
- 🧾 All runs logged to text files (initial state, hits, results)

---

## 🧠 IRL Engineering Under the Hood

- Classical mechanics + A/L level physics  
- Projectile equations (range, time, vertical motion)  
- Power-based damage model for repeated hits  
- Strategy-style decisions on which ships to target first

Built to level up:
- arrays & 2D grids  
- functions and modular C design  
- control structures & loops  
- file handling & simulation logic  

---

## 🛠 Stack

- **Language:** C  
- **Paradigm:** Procedural  
- **Compile:** `gcc ... -lm`  
- **Tools:** VS Code / terminal

---

## 🚀 Run It

```bash
gcc main.c physics.c ships.c battlefield.c io.c -o battle_sim -lm
./battle_sim
