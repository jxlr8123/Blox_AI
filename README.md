# Blox Fruits Lite

Small 3D island game: explore, talk to NPCs, fight bandits and pirates, level up, and sail between islands.

---

## Play the game (Windows)

Your friend only needs this folder and **[Node.js](https://nodejs.org/)** installed (grab the **LTS** version if unsure).

1. Open **PowerShell** or **Command Prompt**.
2. Go to the game folder, for example:
   ```bash
   cd C:\Users\Whatever\Downloads\Blox_Fruits
   ```
3. Install dependencies (first time only, needs internet):
   ```bash
   npm install
   ```
4. Start the game:
   ```bash
   npm start
   ```

A window should open. If it says `electron is not recognized` or errors about missing modules, run `npm install` again in the same folder.

---

## Controls

| Input | What it does |
|--------|----------------|
| **W A S D** | Move on foot. **W/S** forward/back, **A/D** turn. Same keys steer the **boat** (plus **A/D** strafe sideways in the boat). |
| **Space** | Jump (on land). |
| **Mouse wheel** | Zoom camera in/out. |
| **E** | Talk / interact: **guide**, **shop**, **boat seller**, **boat**, gray island NPCs. Also **closes** most popups. |
| **1** | Hotbar: if you own **both** fruits, press **1** to **switch** between Rubber and Flame; with only one fruit it stays equipped. |
| **Left click** | Normal attack for the fruit you have equipped (Rubber stretch punch or Flame fire punch). |
| **Z** | Heavy attack (longer range, cooldown) — Rubber heavy stretch or Flame searing strike. |

On-screen hints appear when you are near something you can use (shop, guide, boat, etc.).

---

## What to do in the game

1. **Green island** — Talk to the **guide**. At the **market**, buy **Rubber** or **Flame** fruit — **each costs $5000** (you start with **$5000**, so you can afford **one** fruit unless you earn more). Press **1** to switch fruits when you own both. Defeat **3 bandits** once, then talk to the **guide** for **300 XP** (bandit mission is **one-time only**).
2. Get a **boat** from the **boat seller** at the west dock (boat is **free**). Walk to the boat and press **E** to board; sail to the **gray island**.
3. **Gray island** — Talk to the NPC in the **center** and pick a trial (**captain** or **six pirates**). Finish it, then talk to that NPC again for **1200 XP** and a fresh run.

Missions and level/XP are shown in the HUD (money top-left, level bar, health).

---

## Optional: build a portable `.exe`

If you have the project set up with `npm install` and `electron-builder`:

```bash
npm run dist
```

Check the `release` folder for the generated Windows build (see `package.json` for details).

---

## Troubleshooting

| Problem | Try this |
|---------|-----------|
| `npm` command not found | Install Node.js and restart the terminal. |
| Black screen / instant close | Run `npm install` in the game folder, then `npm start` again. |
| Game is slow | Close other heavy apps; lower isn’t built in, but zooming out a bit can help a little. |

Enjoy.
