# Recourse

[![Inkle Ink](https://img.shields.io/badge/Story_Engine-Ink_(Inkle)-purple.svg)](https://www.inklestudios.com/ink/)
[![JavaScript](https://img.shields.io/badge/Runtime-JavaScript_ES6-yellow.svg)]()
[![Platform](https://img.shields.io/badge/Platform-Web_Browser-orange.svg)]()
[![Course](https://img.shields.io/badge/Project-CSC_486-brightgreen.svg)]()
[![Team](https://img.shields.io/badge/Developed_By-The_Marines-blue.svg)]()

> A 19th-century maritime psychological narrative game where moral compromises, crew psychology, and the divine intervention of the ocean god Varuna dictate the survival of a storm-tossed vessel.

---

## Overview

**Recourse** is a branching interactive fiction and psychological drama created by **The Marines** for CSC 486. Powered by Inkle's [Ink](https://www.inklestudios.com/ink/) narrative scripting language and a responsive HTML5/JavaScript web interface, the game immerses players in high-stakes social negotiation aboard an ocean-going vessel.

Set during the era of the British East India Company, players step into the shoes of a colonial negotiator returning to England to reunite with family. When a monstrous tempest looms on the horizon, panic divides the crew. The ship's captain decrees that a democratic vote at nightfall will determine whether to push forward or turn back. That night, an ethereal vision of **Varuna**, the Hindu god of the ocean, reveals a chilling prophecy: turning back will cause the ship to sink, drowning everyone aboard.

To survive, you must navigate delicate crew politics and persuade at least three crew members to vote to stay the course—before night falls.

---

## Narrative & Characters

```
                           ┌───────────────────────────────┐
                           │   Prophetic Dream of Varuna   │
                           │  "Turning back seals doom!"   │
                           └───────────────┬───────────────┘
                                           │
                    ┌──────────────────────┴──────────────────────┐
                    ▼                                             ▼
        ┌───────────────────────┐                     ┌───────────────────────┐
        │   Persuade the Crew   │                     │    Maintain Morality  │
        │   (Need 3+ Votes)     │                     │ (Empathy vs Deception)│
        └───────────┬───────────┘                     └───────────┬───────────┘
                    │                                             │
                    └──────────────────────┬──────────────────────┘
                                           ▼
                           ┌───────────────────────────────┐
                           │     Nightfall Captain Vote    │
                           │   Victory, Doom, or Secrets   │
                           └───────────────────────────────┘
```

### The Protagonist
An East India Company negotiator caught between loyalty to homeland and service to the British crown. Weary and longing to see family in England, yet bound by conscience and a divine charge.

### The Crew
- **Arjun**: A fellow countryman aboard the ship, battling homesickness and existential doubt.
- **Andrew Lewis**: A cynical, seasick Scottish sailor in his late 30s who longs for the shores of Scotland and works only when commanded.
- **Raul**: A practical and reserved crewman who responds to calculated reasoning.
- **Robert**: A gruff, skeptical seafarer who honors captaincy orders but bristles at manipulation.
- **Mastan & Muhammad**: Stevedores whose mutual agreement can sway the balance of the vote.
- **Captain Hancock**: Master of the vessel, principled and determined to let democratic consensus decide the ship's fate.

---

## Key Gameplay Mechanics

- **High-Stakes Persuasion**: You only get **one chance** to convince each crew member. Misjudging their personality, history, or fears can permanently lose their vote.
- **Dynamic Morality System (`morality`)**: Starts at 100. Truthful, compassionate dialogue choices preserve your conscience, while manipulative, aggressive, or deceptive tactics deplete your morality score.
- **Vote Counter (`crewConvinced`)**: Tracks the number of committed allies. Securing at least 3 votes enables you to report to Captain Hancock and win the vote.
- **Multiple Narrative Branches & Secret Endings**: Different combinations of convinced sailors, morality thresholds, and dialogue discoveries unlock distinct narrative resolutions.
- **Atmospheric Audio Design**: Custom soundscapes with dynamic looping tracks for ship creaks, churning ocean waves, and tense psychological visions.
- **Player Quality-of-Life**: Built-in interactive controls to **Save** progress to localStorage, **Reload** from previous save points, **Restart** the story, and switch UI visual themes.

---

## Controls & User Interface

- **Choices**: Click any option button to advance the narrative and make critical dialogue decisions.
- **Top Navigation Bar**:
  - `restart`: Reset the story from the beginning.
  - `save`: Save story state and variables to browser memory.
  - `load`: Restore progress from the saved checkpoint.
  - `theme`: Toggle between light and atmospheric dark UI themes.

---

## How to Play

No installation or build tools required:

1. Clone or download the repository:
   ```bash
   git clone https://github.com/knandakumar25/Recourse.git
   ```
2. Open `index.html` in your favorite web browser:
   ```powershell
   Start-Process .\index.html
   ```

---

## Project Structure

```
Recourse/
├── index.html           # Main HTML5 game interface and audio containers
├── style.css            # Responsive layout and typography stylesheets
├── main.js              # Game loop, audio manager, Ink runner, and save/load system
├── ink.js               # Inkle Ink story compiler runtime (JavaScript port)
├── Recourse.js          # Compiled Ink story JSON data structure and story nodes
├── *.png / *.jpg        # Character portraits (andrew, arjun, raul, etc.) and locations
├── *.mp3 / *.wav / .flac# Environmental and ambient audio tracks
└── README.md            # Comprehensive project documentation
```

---

## Audio & Asset Credits

All audio tracks are utilized in accordance with Creative Commons licensing:

- **Ship Creaking-24b.wav** by *glitterglass* — [Freesound](https://freesound.org/s/420467/) (License: Creative Commons 0)
- **LAYERS 019 - ALCHEMIC DREAM DRONE-97.flac** by *Jovica* — [Freesound](https://freesound.org/s/107632/) (License: Creative Commons Attribution 4.0)
- **Lost In The Dream.mp3** by *SoundFlakes* — [Freesound](https://freesound.org/s/490511/) (License: Creative Commons Attribution 4.0)
- **Blade Runner style ambience loop.mp3** by *tsunchoo* — [Freesound](https://freesound.org/s/645101/) (License: Creative Commons 0)
- **on a wooden ship at sea 02.wav** by *LXX.70* — [Freesound](https://freesound.org/s/91072/) (License: Creative Commons Attribution 4.0)
- **Horror Atmosphere 6_The Abyss Stares Back_Loop** by *Ulrich_Wehner* — [Freesound](https://freesound.org/s/736879/) (License: Creative Commons Attribution 4.0)
- **creaking-tension-shipwood-owi.mp3** by *wolfowi* — [Freesound](https://freesound.org/s/588310/) (License: Creative Commons 0)
