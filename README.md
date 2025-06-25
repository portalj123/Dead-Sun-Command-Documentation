# Dead Sun Command Documentation
Just a documentation for the commands in dead sun

## Command Signatures
- `[Args]` -- Used to represent a non specific argument in a command. This is generally replaced by the actual information meant to be passed in the command.
- `[UsingPlayer]` -- Used to Identify the player using the command. 

## Identifiers
- `Integer` Used to identify when a value is a whole number.
- `String` Used to identify when a value is a text.

---

# Commands

**Important Info**
- Brackets are not used in command, they are included only to enhance readability
- Spaces should only be used when seperating the command from it's `[Args]`. Any other use case will likely invalidate the command

**Commands and their function**

```
GiveItem [ItemID : Integer]
```
Gives any item in the game to `[UsingPlayer]`

```
Teleport [X : Integer,Y : Integer,Z : Integer]
```
Teleports `[UsingPlayer]` to any XYZ coordinate

```
GiveQuest [QuestID : String]
```
Gives any quest in the game to `[UsingPlayer]`

---

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

## Quests
The QuestID for each quest in game

- `ExampleQuest`: Example Quest
- `Intro`: Intro
- `SouthbridgeShelter`: Survivors Guilt
