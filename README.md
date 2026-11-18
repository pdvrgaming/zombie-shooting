# DEAD ZONE: SURVIVAL APOCALYPSE 🧟‍♂️💥

> **Immersive 3D WebXR Survival Horror FPS** engineered for **Meta Quest 2 (Oculus Quest 2)**, with full cross-platform support for Desktop PC and Mobile Touchscreens.

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Play%20on%20GitHub%20Pages-brightgreen?style=for-the-badge&logo=github)](https://pdvrgaming.github.io/zombie-shooting/)
[![Meta Quest 2](https://img.shields.io/badge/Meta%20Quest%202-WebXR%206DOF%20Ready-blue?style=for-the-badge&logo=oculus)](https://pdvrgaming.github.io/zombie-shooting/)
[![Three.js](https://img.shields.io/badge/Three.js-r128-black?style=for-the-badge&logo=three.js)](https://threejs.org/)
[![Audio Engine](https://img.shields.io/badge/Audio-Spatial%203D%20Horror-orange?style=for-the-badge)](sounds/)

---

## 🌐 Live Website & Play Link

Play instantly in your browser or **Meta Quest Browser** with no installation required:
👉 **[https://pdvrgaming.github.io/zombie-shooting/](https://pdvrgaming.github.io/zombie-shooting/)**

---

## 🏷️ Discovery & Repository Settings

Copy and paste these directly into your GitHub Repository settings (**About** section at top-right of your repo):

- **Description:**
  > Immersive 3D WebXR Survival Horror FPS built with Three.js for Meta Quest 2 & Oculus Browser. Features 6DOF dual Touch controllers, spatial 3D audio, realistic ballistics, gore physics, interactive 3D spatial UI, and a 9-wave apocalypse campaign.
- **Website:**
  > `https://pdvrgaming.github.io/zombie-shooting/`
- **Topics / Tags for Discovery:**
  ```
  meta-quest-2, oculus-quest-2, webxr, threejs, vr-game, virtual-reality, zombie-shooter, survival-horror, fps, html5-game, webgl, spatial-audio, pwa, quest2-vr, browser-game
  ```

---

## 🎮 Overview

**Dead Zone: Zombie Apocalypse** is a fast-paced 3D survival game built with **Three.js** and **WebXR**. Survive 9 relentless waves across 3 hostile locations, detonate fuel barrels, collect tactical supply drops, and eliminate hordes of the undead and mutant beasts.

---

## 🌟 Key Features

### 1. 🔊 Realistic Acoustic Audio Engine (Catastic Zombie Horror Package)
Replaced synthetic tones with 44 high-fidelity audio samples from the **Zombie Horror Package**:
- **Bite & Attack:** Real gnashing bites (`Zombie_Attack_Bite`) and zombie attack roars.
- **Flesh Impacts & Blood:** Visceral flesh bullet hit sounds (`Impact_Flesh`, `Impact_Flesh_Gory_Light`) and dynamic liquid splashes (`Blood_Splash_A`).
- **Body Falls:** Heavy physical ground impact upon zombie defeat (`Foley_BodyFall`).
- **Spatial 3D Audio:** Integrated with Web Audio API `PannerNode` (HRTF distance model) so you hear exact zombie directions in 3D surround sound.
- **Atmospheric Footsteps & Foley:** Real crunching footsteps and movement audio.

### 2. ⏱️ Mission & Session Timer (Top-Left HUD)
- Positioned in the **top-left corner** of the HUD.
- **Unlimited Mode:** Displays total elapsed survival time (`MM:SS`).
- **Timed Session Mode:** Counts down remaining time. Under 30 seconds, it flashes bright red with an urgent warning alert.
- **VR Wrist HUD:** Displayed directly on your in-VR weapon HUD screen for real-time tracking inside the Quest 2 headset.

### 3. 🗺️ Continuous 9-Wave Campaign Progression
The game now flows seamlessly across all 3 sectors without requiring manual restarts:
1. **Location 1: Downtown City (Waves 1 – 3)**  
   - Urban ruins with crumbling skyscrapers and flickering streetlamps.  
   - *Boss:* **The Warden**
2. **Location 2: Dark Pine Forest (Waves 4 – 6)**  
   - Dense pine trees, wooden cabins, and foggy green moonlight.  
   - *Boss:* **Alpha Behemoth**
3. **Location 3: Bio-Lab Compound (Waves 7 – 9)**  
   - Industrial hazard corridors, glowing toxic silos, and crimson emergency sirens.  
   - *Boss:* **Omega Apex**
- **Seamless Transitions:** Defeating a sector's boss triggers a 4-second victory intermission with bonus ammunition and health replenishment before automatically deploying you to the next sector!

### 4. 📱 Automatic Device Detection at Startup
The startup UI automatically sniffs your platform and configures the interface:
- **🥽 Oculus / Meta Quest 2:** Promotes **ENTER VR (QUEST 2)** as the glowing primary action, switches to 6DOF Touch controller guides, and disables 2D cursor locks.
- **📱 Mobile Touchscreen:** Promotes **PLAY (MOBILE)**, enables the dual-analog virtual joystick and tactile fire/reload buttons.
- **🖥️ Desktop PC:** Promotes **PLAY (PC)**, enables pointer lock, mouse look, and keyboard layout.
- *Manual override buttons remain available in the menu for testing any mode.*

### 5. 🩸 Realistic Blood Shed & Decal Engine
- **Directional Velocity Splatter:** Blood bursts forward along the bullet exit vector with conical dispersion, variable droplet sizes, and gravity physics.
- **Persistent Ground Puddles (Decals):** Blood droplets falling to the ground (`y <= 0.02`) instantiate flat blood puddles that pool on the asphalt.
- **Headshot Decapitation Geysers:** 35+ blood mist particles, gore chunks, and bone fragments burst vertically on critical headshots.
- **Screen Damage Splatter:** Dynamic blood splashes pulse on the player's screen/visor when attacked.

### 6. ⌛ Main UI Session Time Limit Setter
Configure your playtime in the main menu before deployment:
- **Options:** `UNLIMITED`, `2 MIN`, `5 MIN`, `10 MIN`, `15 MIN`.
- **Evacuation Screen:** When time expires, a dedicated **SESSION IS OVER** screen summarizes your survival statistics (Final Score, Kills, Waves Conquered, Locations Cleared).

---

## 🕹️ Controls Guide

| Action | Desktop PC | Mobile Touch | Oculus / Meta Quest 2 |
| :--- | :--- | :--- | :--- |
| **Move** | `W` `A` `S` `D` / Arrows | Left Virtual Joystick | **Left Thumbstick** |
| **Aim / Look** | Mouse Movement | Right Half Screen Drag | **Head Tracking (6DOF)** |
| **Fire Weapon** | Left Mouse Click | Red `FIRE` Button | **Right Index Trigger** |
| **Reload** | `R` Key | `REL` Button | **Right Grip Button** |
| **Weapon Selection** | Choose in Main Menu UI | Choose in Main Menu UI | **Choose in Main Menu UI** |
| **Sprint** | Hold `Left Shift` | `RUN` Toggle Button | Push Left Stick Forward |
| **Pause Game** | `P` / `Escape` | `PAUSE` Top Button | **Left Menu / Grip Button** |
| **Turn** | Mouse Aim | Touch Drag | **Right Thumbstick (Snap Turn)** |

---

## 🥽 How to Run on Oculus / Meta Quest 2

### Method 1: Meta Quest Browser (Instant WebXR)
1. Host the project locally or on GitHub Pages:
   ```bash
   # Quick local server using Python
   python -m http.server 8000
   ```
2. Put on your **Meta Quest 2**.
3. Open the **Meta Quest Browser**.
4. Navigate to `http://<YOUR_PC_IP>:8000` or your GitHub Pages URL (`https://pdvrgaming.github.io/zombie-shooting`).
5. The game will automatically detect the Quest 2 headset. Tap **ENTER VR (QUEST 2)**.
6. Click **Allow** on the WebXR immersive permission prompt.
7. You are now inside the 3D apocalyptic world with full 6DOF Touch controller tracking!

### Method 2: Install as a Standalone Quest PWA
Because the project includes a `manifest.json` configured for WebXR:
1. In Meta Quest Browser, open the game URL.
2. Click the **three dots menu (...)** on the browser address bar.
3. Select **Install App** / **Add to Apps Library**.
4. The game will appear as an independent icon in your Quest App Library and launch in dedicated full-screen VR!

---

## 📂 Project Structure

```
Zombie Shooting/
├── index.html                           # Main game entry point (Enhanced WebXR & PC/Mobile)
├── dead_zone_zombie_apocalypse (3).html # Compatible secondary entry file
├── manifest.json                        # PWA & WebXR configuration for Meta Quest
├── .gitignore                           # Git ignore rules for OS and temporary files
├── README.md                            # Complete documentation and setup guide
└── sounds/                              # Catastic Zombie Horror Sound Pack
    ├── Bite/                            # Zombie attack bite clips (MP3)
    ├── Blood/                           # Liquid blood splatter and splash effects (MP3)
    ├── BodyFall/                        # Zombie body fall and impact foley (MP3)
    ├── Eat/                             # Zombie eating foley sounds (MP3)
    ├── Foley/                           # Clothes movement and crawling sounds (MP3)
    ├── Footsteps/                       # Zombie and survivor concrete footsteps (MP3)
    ├── Impact/                          # Flesh impact and gory bullet hit audio (MP3)
    └── VO/                              # Voice Over grunts, attacks, hurts, and idles
        ├── Zombie01/                    # Standard walker & runner vocals
        └── Zombie03/                    # Heavy & boss creature vocals
```

---

## 🛠️ Development & Git Setup

Repository: `https://github.com/pdvrgaming/zombie-shooting.git`

```bash
# Clone the repository
git clone https://github.com/pdvrgaming/zombie-shooting.git

# Launch a local test server
python -m http.server 8000
# or with Node.js
npx serve .
```

---

## 📜 Credits & License
- **Game Engine & Rendering:** Built with [Three.js r128](https://threejs.org/).
- **Audio Assets:** *Zombie Sound Pack - Free Version* by **Catastic** (All rights reserved by creator).
- **Developed for:** PC, Touch Devices, and Meta / Oculus Quest 2.
