# Strong_hold_game_project
Object Oriented Programming 
2nd Smester Project 
# Multiplayer Kingdom Simulation Game

A C++ terminal-based simulation game where two players manage their kingdoms by building structures, trading, training soldiers, and engaging in diplomacy or warfare. The game supports turn-based multiplayer mechanics and offers strategic gameplay with map movement, alliances, and resource management.

## 🎯 Project Overview

This project simulates a medieval-themed kingdom management game for two players. Each player can:
- Build and manage infrastructure (farms, houses, barracks, workshops)
- Produce and trade resources (food, wood, gold)
- Train military units and engage in battles
- Use diplomacy tools like alliances and betrayal
- Save/load game progress and view historical logs of trades and battles

The game promotes critical decision-making with strategic trade-offs between peaceful growth and aggressive expansion.

## 🧰 Technologies Used

- **Language:** C++
- **Development Tools:** GCC, g++, Terminal/Command Prompt
- **File Handling:** Save/load functionality via `.txt` files
- **Randomization:** `rand()` function for game unpredictability
- **Multiplayer Support:** Implemented via turn-based shared state
- **Logging Systems:** Persistent logs for market trades, battles, and treaties

## 🗂 Project Structure
├── game.h # Kingdom class declaration
├── game.cpp # Kingdom class definition (build, trade, train, etc.)
├── multiplayer.h # Multiplayer engine header
├── multiplayer.cpp # Multiplayer engine implementation
├── main.cpp # Game loop and turn manager
├── score.txt # Event log (auto-generated)
├── chat.txt # Player communication log (auto-generated)
├── treaty.txt # Alliance and diplomacy log (auto-generated)
├── battle_log.txt # Battle history log (auto-generated)
├── market.txt # Trade records (auto-generated)
├── <player>_save.txt # Save file for each player (auto-generated)

## ✅ Features Implemented

### Kingdom Management
- **Resources:** Gold, food, wood
- **Buildings:** Barracks, farms, houses, woodcutters, workshops, mines
- **Population Growth:** Increases with number of houses
- **Weapon Crafting:** Bows, swords, maces via workshops

### Military Training
- **Units:** Archers, swordsmen, macemen
- **Requirement:** Weapons + gold + barracks

### Trade System
- Trade food and wood legally or illegally (risk/reward system)
- All trade logs saved to `market.txt`

### Diplomacy and Warfare (Multiplayer)
- Send messages to other players
- Form or break alliances
- Attack enemy kingdoms (considering alliance betrayal penalties)
- View alliances and map positions

### Map Movement
- Each kingdom has coordinates on a 5x5 map
- Players can move on the map

### Logging
- Battle logs (`battle_log.txt`)
- Diplomatic actions (`treaty.txt`)
- Trade actions (`market.txt`)
- Chat messages (`chat.txt`)

## 💾 How to Run the Game

### 1. Compile the Game
```bash
g++ main.cpp game.cpp multiplayer.cpp -o kingdom_game
2. Run the Game
./kingdom_game
3. Play!
Two players (e.g., Saba and Fasiha) take turns.

Input number options based on the in-game menu.

Save/load games using options 10 and 11.

👥 Project Division & Contributions
Module	Contributor(s)	Description
game.h/cpp	Developer 1	Implemented all core gameplay mechanics like building, trading, resource generation, and training.
multiplayer.h/cpp	Developer 2	Designed multiplayer interaction engine (alliances, chat, attack, map movement).
main.cpp	Both	Integrated game loop and user interaction, turn switching, and UI handling.

📚 What We Learned
Hands-on file handling using ifstream/ofstream

Managing game state using object-oriented programming

Multiplayer logic via turn-based engine

Real-time logging and interaction with the file system

Strategic game design decisions including diplomacy, risk-reward systems, and simulation elements

🎮 Enjoy playing and managing your kingdom!



