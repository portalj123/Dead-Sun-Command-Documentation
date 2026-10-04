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
GiveItem [ItemID : String]
```
Gives any item in the game to `[UsingPlayer]`.
**Usage Example:**
```lua
GiveItem Viper
```
---
```lua
GiveAmmo [AmmoType : String],[Amount : Integer]
```
Gives ammo of any type to `[UsingPlayer]`.
**Usage Example:**
```lua
GiveAmmo Assault,64
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
Kicks any Player in the game. `This will be disabled during the public playtest`
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
Spawn any entity in the game. (Entity will spawn exactly 12 studs in front of `[UsingPlayer]`, facing directly towards them.)
**Usage Example:**
```lua
Spawn Human
```

---

```lua
SetWeather [WeatherID : String]
```
Changes the global weather to `WeatherID`.
**Usage Example:**
```lua
SetWeather Rain
```

---

```lua
GiveCash [CashAmount : Number]
```
Gives `[CashAmount]` to  `[UsingPlayer]`.
**Usage Example:**
```lua
GiveCash 12500
```

# Argument Information
Things like Arguments and Data you use in commands, like Item IDs and Quest IDs

## Items
The ItemID for each item in game
Ranged
- `[Viper]`: Viper (Standard Revolver)
- `[AK47]`: AK 47
- `[Renetta]`: Renetta (Standard Pistol)
- `[Mossberg]`: Mossberg (Shotgun)
- `[Crossbow]`: Crossbow `Currenly Disabled`
- `[AWP]`: Advanced Winter Rifle (Standard Sniper) `Currenly Disabled`
Melee
- `[Pipe]`: Pipe
- `[MakeshitBlade]`: Makeshift Machete
Throwable
- `[Molotov]`: Molotov Cocktail (Throwable)
- `[Bottle]`: Glass Bottle (Throwable)
- `[Brick]`: Brick (Throwable)

## Quests
The QuestID for each quest in game

- `ExampleQuest`: Example Quest
- `ExampleQuest2`: Example Quest
- `EliminateGroupTest`: Quest created for testing out enemy group spawning and killing
- `EliminateGroupTest2`: Quest created for testing out enemy group spawning and killing with stealth
- `CampaignQuest2 - 8`: All currently created storyquests. DO NOT USE, the map is not available in testing, and they will not function properly.

## Entities
The EntityID for each quest in game

- `Human`: Standard Human enemy
- `Passive`: Standard Passive Human, pretty much just a dummy with animations
- `Zombie`: Basic Zombie
- `Viral`: Faster, More intelligent zombie

## Weather Types
The WeatherID for each weather type in game

- `Clear`: Clear, Sunny, Warm
- `Rain`: Heavy Rain, Cold
- `Cloudy`: Lukewarm
- `Snow`: Heavy Snow, Cold
