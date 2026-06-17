# Tile-Based Movement (Xogot Tutorial)

This project demonstrates how to build **simple tile-based player movement**
entirely in **Xogot** — the iPad and iPhone port of the Godot game engine.

The tutorial shows how to create a player that moves one tile at a time, snaps
cleanly to a grid, and uses directional raycasts to prevent movement into
blocked spaces. This technique is useful for **puzzle games, dungeon crawlers,
roguelikes, RPGs, and grid-based gameplay systems**, all built directly on iPad.

---

## Features

* Simple **CharacterBody2D** player scene
* Player art using **Sprite2D**
* Tile-sized **CollisionShape2D** setup
* Four-direction movement using Godot input actions
* **RayCast2D** detectors for checking blocked tiles
* Exported **tile size** and **movement speed** variables
* Automatic player position snapping to the tile grid
* Smooth movement from one tile to the next
* Designed to work smoothly on **iPad and iPhone** with Xogot
* Compatible with **Godot 4.x**

---

## Video Tutorial

Watch the full video walkthrough by **Jhello** on the Xogot YouTube channel:

[Tile-Based Movement in Xogot - Godot on iPad](https://youtu.be/73Hu8MeBhz0)

---

## How to Use

1. Download or clone this repository:

```bash
git clone https://github.com/xogot-projects/Xogot-Tile-Based-Movement.git
```

2. Open the project in **Xogot** on iPad or iPhone.

3. Open the main scene and run the project.

4. Move the player using your configured input controls.

The player will move one tile at a time and use raycasts to avoid moving into
blocked spaces.

---

## What You'll Learn

This sample project covers the core pieces needed for grid-based movement in
Godot:

* Creating a reusable player scene
* Aligning a player to a tile grid
* Using exported variables for tile size and movement speed
* Referencing child nodes with `@onready`
* Moving smoothly with `move_toward()`
* Using `RayCast2D` nodes to detect blocked directions
* Handling directional input with Godot's built-in input actions

---

## Project Structure

The project includes a small 2D scene with a tile-based world and a player scene
configured for grid movement.

The player scene contains:

* `CharacterBody2D` root node
* `Sprite2D` for the player artwork
* `CollisionShape2D` for tile-sized collision
* A `Detectors` node containing four `RayCast2D` nodes:

  * Up
  * Down
  * Left
  * Right

The player script handles snapping, input detection, raycast checks, and smooth
movement from one tile to the next.

---

## Requirements

* Xogot for iPad or iPhone
* Godot 4.x compatible project files

---

## About Xogot

**Xogot** brings the Godot editor to iPad and iPhone, making it possible to
build, edit, and test Godot projects directly on iOS devices.

Learn more at: https://xogot.com

---

## Join the Community

Join the Xogot Discord to ask questions, share projects, and connect with other
Godot creators using Xogot:

https://discord.gg/TDEcyfHZAh
