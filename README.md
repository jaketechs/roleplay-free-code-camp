# FreeCodeCamp Basic Roleplay Game

This project is a basic roleplay game built while following the FreeCodeCamp curriculum. It demonstrates foundational JavaScript concepts such as arrays, objects, functions, and DOM manipulation.

## Features

- Navigate through different locations (e.g., town square, store, cave, fight scenes).
- Buy items and upgrade your character's inventory.
- Battle monsters with unique names and health stats.
- Manage player stats such as gold and health.
- Dynamic updates to the UI based on player actions.

## How to Play

1. **Start in the Town Square**:
   - Choose from available actions like visiting the store, entering the cave, or fighting a dragon.

2. **Visit the Store**:
   - Buy health to replenish your HP.
   - Purchase new weapons to increase your power.

3. **Enter the Cave**:
   - Encounter and battle different monsters.

4. **Fight Monsters**:
   - Attack, dodge, or run back to safety.
   - Defeat monsters to progress in the game.

## Project Structure

- **JavaScript**: Handles the game logic, including updating player stats, managing locations, and combat mechanics.
- **HTML**: Provides the structure of the game interface.
- **CSS**: Adds minimal styling to enhance the visual appearance.

## Code Highlights

### Locations Array

The game uses a `locations` array to manage different areas in the game:

```javascript
const locations = [
  {
    name: "town square",
    "button text": ["Go to store", "Go to cave", "Fight dragon"],
    "button functions": [goStore, goCave, fightDragon],
    text: "You are in the town square. You see a sign that says \"Store\"."
  },
  {
    name: "store",
    "button text": ["Buy 10 health (10 gold)", "Buy weapon (30 gold)", "Go to town square"],
    "button functions": [buyHealth, buyWeapon, goTown],
    text: "You enter the store."
  },
  {
    name: "cave",
    "button text": ["Fight slime", "Fight fanged beast", "Go to town square"],
    "button functions": [fightSlime, fightBeast, goTown],
    text: "You enter the cave. You see some monsters."
  },
  {
    name: "fight",
    "button text": ["Attack", "Dodge", "Run"],
    "button functions": [attack, dodge, goTown],
    text: "You are fighting a monster."
  }
];

