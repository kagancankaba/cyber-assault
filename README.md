# Cyber Assault — Tower Defense Game

A Tower Defense game developed in Unity with C#, themed around a futuristic "Cyberworld" dystopia. Built to demonstrate Object-Oriented Programming principles including Inheritance, Polymorphism, Encapsulation, and Abstraction.

## Gameplay

Defend your base against waves of cyber enemies by strategically placing towers. Each tower and enemy type has unique mechanics and interactions.

## Towers

- **Electric Tower** — Single target, consistent damage
- **Nuclear Tower** — Area of effect damage via explosion radius
- **Slime Tower** — Slows enemies down while dealing damage

## Enemies

- **Cyborg** — Fast, low health
- **CyberTank** — Armored, damage reduction formula: `1 - (armor / (armor + 100))`
- **CyberTruck** — Balanced stats

## Architecture

- **Singleton Pattern** — BaseScript manages global game state (money, health, waves)
- **Inheritance** — Enemy and FiringTower base classes with specialized subclasses
- **Polymorphism** — Shoot() and TakeDamage() methods overridden per unit type
- **Coroutines** — Async enemy spawning without blocking the main thread
- **Event Logging** — All game events saved to `savunma_gunlugu.txt`

## Technologies

- Unity
- C#

## Files

- `Assets/` — Scenes, scripts, prefabs, and sprites
- `ProjectSettings/` — Unity project configuration
- `report.pdf` — Detailed project report with UML diagrams and simulation results