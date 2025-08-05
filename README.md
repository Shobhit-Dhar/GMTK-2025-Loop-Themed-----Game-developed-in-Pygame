# That Time I Got Summoned by a Mage to Use My Intellect and Break Free from the Dungeon (TTIGSBAMTGOOTD)

## Overview

This is a 2D platformer game built with Pygame. The player controls a character who has been summoned into a mysterious, dark, and foggy dungeon by a mage. The goal is to navigate through a series of interconnected levels, acquire new abilities, and ultimately find a way to escape. The game features a minimalist, silhouette art style reminiscent of the game *Limbo*, with a focus on atmosphere and exploration.

## Story

You are an ordinary person who has been unwillingly summoned into a dark dungeon by a mysterious mage. The mage, also trapped, needs your intellect to help them both escape. You must traverse the treacherous levels, unlocking new powers along the way, to find the final exit and return to your world. Will you trust the mage? Will you find your way out?

## Features

*   **Atmospheric Silhouette Art Style:** A grayscale color palette and silhouette-based graphics create a moody and mysterious atmosphere.
*   **Progressive Abilities:** Start with basic movement and unlock abilities like jumping, double jumping, and a fireball attack as you progress through the levels.
*   **Level-Based Progression:** Navigate through multiple interconnected rooms, each with its own unique layout and challenges.
*   **Interactive NPCs:** Encounter a mysterious robed figure who provides cryptic dialogue and hints.
*   **Dynamic Lighting and Effects:** Features include fog particles, dust particles from movement, and glowing effects for key items and abilities.
*   **Engaging Audio:** Includes sound effects for actions like jumping and walking, and background music that changes with the game state.
*   **Physics-Based Platforming:** Smooth and responsive player controls with gravity and momentum.
*   **Interactive Environments:** Breakable boxes can hide keys or other secrets.

## How to Play

### Controls

*   **Move Left:** `A` or `Left Arrow`
*   **Move Right:** `D` or `Right Arrow`
*   **Jump / Double Jump:** `Spacebar`, `W`, or `Up Arrow`
*   **Drop Down from Platform:** `S` or `Down Arrow`
*   **Interact with NPC:** `E`
*   **Fireball (Once Unlocked):** `F` or `Left Shift` (Aim with the mouse)

### Gameplay

1.  **Navigate the Dungeon:** Move your character through each level, avoiding falls and overcoming platforming challenges.
2.  **Talk to the Mage:** Press 'E' when near the robed figure to get hints and story dialogue.
3.  **Unlock Abilities:** Certain levels will grant you new powers that are essential for progressing.
4.  **Find the Exit:** Your ultimate goal is to find and unlock the final door to escape the dungeon.

## Requirements

*   Python 3.x
*   Pygame library

## Installation & Running the Game

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

2.  **Install Pygame:**
    ```bash
    pip install pygame
    ```

3.  **Create a `sounds` folder:**
    Create a folder named `sounds` in the root directory of the project.

4.  **Add Sound Files:**
    Place the following sound files into the `sounds` folder. You can use your own `.wav` and `.mp3` files, but they must be named correctly.
    *   `jump.wav`
    *   `walk.wav`
    *   `fireball.wav`
    *   `menu_theme.mp3`
    *   `game_theme.mp3`
    *   `ending_theme.mp3`

5.  **Run the game:**
    ```bash
    python game.py
    ```
    *(Assuming the provided code is saved as `game.py`)*

## Code Structure

*   **`Game` class:** The main class that manages the game loop, states (menu, playing, etc.), and events.
*   **`Player` class:** Handles all player logic, including movement, animation, abilities, and collisions.
*   **`Level` class:** Loads and manages the data for each level, including platforms, doors, and NPCs.
*   **`Door`, `BreakableBox`, `NPC` classes:** Define the interactive objects within the game.
*   **`Fireball`, `DustParticle`, `FogParticle` classes:** Manage visual effects and projectiles.
*   **`Menu`, `EndingScreen` classes:** Handle the main menu and the end-game credit sequence.
*   **Constants and Game States:** Global variables for screen dimensions, colors, and game states are defined at the top of the file.
