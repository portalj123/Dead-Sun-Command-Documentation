# Dead Sun Command Documentation
Just a documentation for the commands in dead sun

Use SemiColon to open command menu.

## Command Signatures
- `[Args]` -- Used to represent a non specific argument in a command. This is generally replaced by the actual information meant to be passed in the command.
- `[UsingPlayer]` -- Used to Identify the player using the command. 

## Identifiers
- `Integer` Used to identify when a value is a whole number.
- `String` Used to identify when a value is a text.
- `Float` Used to identify when a value is a real number.

---

# Commands

**Important Info**
- Brackets are not used in command, they are included only to enhance readability
- Spaces should only be used when seperating the command from it's `[Args]`. Any other use case will likely invalidate the command

**Commands and their function**


```lua
Help
```
Prints a list of every command in the game.

---

```lua
GiveItem [ItemID : Integer]
```
Gives any item in the game to `[UsingPlayer]`.
**Usage Example:**
```lua
GiveItem 1
```
---

```lua
Teleport [X : Integer,Y : Integer,Z : Integer]
```
Teleports `[UsingPlayer]` to any XYZ coordinate.
**Usage Example:**
```lua
Teleport 256,500,129
```

---

```lua
SetTime [Time : Float]
```
Set's the global time in game.
**Usage Example:**
```lua
SetTime 17
```
---

```lua
GiveQuest [QuestID : String]
```
Gives any quest in the game to `[UsingPlayer]`.
**Usage Example:**
```lua
GiveItem 1
```
---

```lua
Kill [Player : String]
```
Kills any Player in the game.
**Usage Example:**
```lua
Kill JohnDoe
```

---

```lua
InstantHeal [Player : String]
```
Health any Player in the game to full health.
**Usage Example:**
```lua
InstantHeal portalj123
```

---

```lua
Kick [Player : String]
```
Kicks any Player in the game.
**Usage Example:**
```lua
Kick Kelletonskeleton16
```

---

```lua
Ban [Player : String]
```
Bans any Player in the game permanently, only use this against deserving players, and file a ban report afterwards. Failure to do so may result in the ban being appealed, and/or loss of admin.
**Usage Example:**
```lua
Ban fornitebattle676
```

---

```lua
Spawn [EntityID : String]
```
Spawn any entity in the game. (Entity will spawn exactly 12 stud in front of `[UsingPlayer]`, facing directly towards them.)
**Usage Example:**
```lua
Spawn Human
```


# Argument Information
Things like Arguments and Data you use in commands, like Item IDs and Quest IDs

## Items
The ItemID for each item in game

- `[1]`: Zombie Spawner
- `[2]`: Viper (Standard Revolver)
- `[3]`: AK 47
- `[4]`: Renetta (Standard Pistol)
- `[5]`: Mossberg (Shotgun)
- `[6]`: Pipe
- `[7]`: Crossbow
- `[8]`: Advanced Winter Rifle (Standard Sniper)
- `[9]`: Makeshift Machete

## Quests
The QuestID for each quest in game

- `ExampleQuest`: Example Quest
- `Intro`: Intro
- `SouthbridgeShelter`: Survivors Guilt

## Entities
The EntityID for each quest in game

- `Human`: Standard Human enemy
- `Passive`: Standard Passive Human, pretty much just a dummy with animations
- `Zombie`: Basic Zombie

## Common Teleports
Coordinates for common locations you can teleport to

- `1117,3,-775`: Survivor Base
- `-4096,3,0`: Testing Area
