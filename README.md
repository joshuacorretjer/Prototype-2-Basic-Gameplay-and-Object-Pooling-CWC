# Prototype 2 – Basic Gameplay

## Overview

A Unity 3D top-down arcade game developed as part of the **Create with Code Live – Spring 2020** course. The objective is to throw food projectiles at incoming animals before they run past the player.

The project focuses on implementing fundamental gameplay mechanics using C# and Unity, including player movement, projectile launching, random spawning, collision detection, and object instantiation. It was revisited toward the end of the course to introduce object pooling and improve performance.

## Features

- **Player Movement:** Implemented player controls with movement boundaries to keep the player within the playable area.
- **Projectile System:** Created a projectile system that allows the player to launch food at incoming animals.
- **Animal Spawning:** Implemented an animal spawning system that selects from an array of animal prefabs and spawns them at random intervals.
- **Collision Detection:** Implemented collision handling between projectiles and animals, destroying both objects upon impact.
- **Out-of-Bounds Detection:** Added functionality to remove projectiles and animals when they leave the playable area.
- **Debug Messages:** Used Unity's Debug Log to detect and report when animals successfully pass the player.
- **Object Pooling:** Optimized projectile management by reusing inactive objects instead of repeatedly destroying and instantiating them.

## What I Learned & Implemented

### Player Controls and Projectile Mechanics
- Used conditional statements (`if` statements) to establish movement boundaries and restrict player movement.
- Created projectile prefabs with movement scripts to control their forward movement.
- Used `Instantiate()` to spawn projectiles when the player launches food.
- Implemented a `DestroyOutOfBounds()` function to remove projectiles and animals that travel outside the playable area.

### Spawning System and Randomization
- Created an animal spawning manager to organize and control animal generation.
- Used arrays to store animal prefabs and randomly select which animal to spawn.
- Implemented `InvokeRepeating()` to execute spawning functions at randomized time intervals.
- Created separate custom functions for spawning logic to improve code organization and readability.

### Collision Detection and Camera Setup
- Configured the camera's projection settings to achieve a proper top-down perspective.
- Adjusted Box Colliders to better fit the dimensions of game objects.
- Implemented collision detection to destroy both the projectile and animal when they collide.
- Used `Debug.Log()` to display messages in the Unity Console when animals passed the player.

### Performance Optimization
- Learned and implemented object pooling for projectiles.
- Configured a pool of reusable projectile objects.
- Replaced repeated object destruction with object deactivation, allowing projectiles to be reused when needed.

## Technologies & Tools

- **Game Engine:** Unity
- **Programming Language:** C#
- **IDE:** Visual Studio
- **Concepts:** Player Movement, Projectile Systems, Prefabs, Instantiation, Arrays, Randomization, InvokeRepeating, Conditional Statements, Collision Detection, Box Colliders, Object Pooling

## Course

**Create with Code Live – Spring 2020**

A remote Unity course taught by professionals working at Unity, focused on learning game development and programming through hands-on projects.
