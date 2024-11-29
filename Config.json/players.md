---
position: 10
title: Players
authors: MCrow
published: true
description: Players settings allow you to adjust the health, food, water, and virus levels of players, as well as the damage and regeneration rates of these levels.
---

Players settings allow you to adjust the health, food, water, and virus levels of players, as well as the damage and regeneration rates of these levels. You can also adjust the experience, detection radius, and other player settings.

Based on [Official Unturned Wiki](https://unturned.wiki.gg/wiki/Gameplay_config#Players) and our experience.

```json
"Players": {
  "Health_Default": 100,
  "Health_Regen_Min_Food": 90,
  "Health_Regen_Min_Water": 90,
  "Health_Regen_Ticks": 60,
  "Food_Default": 100,
  "Food_Use_Ticks": 350,
  "Food_Damage_Ticks": 15,
  "Water_Default": 100,
  "Water_Use_Ticks": 320,
  "Water_Damage_Ticks": 20,
  "Virus_Default": 100,
  "Virus_Infect": 50,
  "Virus_Use_Ticks": 125,
  "Virus_Damage_Ticks": 25,
  "Leg_Regen_Ticks": 750,
  "Bleed_Damage_Ticks": 10,
  "Bleed_Regen_Ticks": 750,
  "Armor_Multiplier": 1.0,
  "Experience_Multiplier": 1.5,
  "Detect_Radius_Multiplier": 0.5,
  "Ray_Aggressor_Distance": 8.0,
  "Lose_Skills_PvP": 1.0,
  "Lose_Skills_PvE": 1.0,
  "Lose_Skill_Levels_PvP": 0,
  "Lose_Skill_Levels_PvE": 0,
  "Lose_Experience_PvP": 0.5,
  "Lose_Experience_PvE": 0.5,
  "Lose_Items_PvP": 1.0,
  "Lose_Items_PvE": 1.0,
  "Lose_Clothes_PvP": true,
  "Lose_Clothes_PvE": true,
  "Lose_Weapons_PvP": true,
  "Lose_Weapons_PvE": true,
  "Can_Hurt_Legs": true,
  "Can_Break_Legs": false,
  "Can_Fix_Legs": true,
  "Can_Start_Bleeding": false,
  "Can_Stop_Bleeding": true,
  "Spawn_With_Max_Skills": false,
  "Spawn_With_Stamina_Skills": false,
  "Allow_Instakill_Headshots": false,
  "Allow_Per_Character_Saves": false,
  "Enable_Terrain_Color_Kick": true
}

```
### Health_Default
Sets the amount of health players start with. Must be between **0** and **255**.
---

### Health_Regen_Min_Food
The minimum food level required to kickstart health regeneration.
---

### Health_Regen_Min_Water
The minimum water level needed to trigger health regeneration.
---

### Health_Regen_Ticks
Defines how frequently health regenerates. A lower value speeds up the process.
---

### Food_Default
Specifies the starting food level for players. Must be between **0** and **255**.
---

### Water_Default
Specifies the initial water level for players. Must be between **0** and **255**.
---

### Virus_Default
Determines the immunity level players spawn with. Must be between **0** and **255**.
---

### Virus_Infect
Sets the immunity threshold at which infections start. Immunity will deplete unless treated. Setting this to **0** disables untreated infections.
---

### Virus_Use_Ticks
Controls how often immunity decreases when below the infection threshold. A lower value means faster depletion.
---

### Virus_Damage_Ticks
Defines how often players take damage when immunity is fully depleted.
---

### Leg_Regen_Ticks
Specifies the duration for recovering from the "Broken Bones" debuff. A lower value reduces recovery time.
---

### Bleed_Damage_Ticks
Determines how frequently players take damage from the "Bleeding" debuff.
---

### Bleed_Regen_Ticks
Specifies the recovery time for the "Bleeding" debuff. A lower value speeds up recovery.
---

### Armor_Multiplier
Sets the damage multiplier for players. Values below **1.0** reduce damage, while values above **1.0** increase it.
---

### Experience_Multiplier
Controls the multiplier for experience gained by players.
---

### Detect_Radius_Multiplier
Adjusts how easily animals and zombies detect players. Higher values make detection easier.
---

### Ray_Aggressor_Distance
Defines the distance (in meters) used to determine the "aggressor" in combat. Relevant to the reputation system.
---

### Lose_Skills_PvP
Specifies the percentage of skills retained after a PvP death. A value of **1** means all skills are retained.
---

### Lose_Skills_PvE
Specifies the percentage of skills retained after a PvE death. A value of **1** means all skills are retained.
---

### Lose_Skill_Levels_PvP
Sets the number of skill levels lost after a PvP death. A value of **0** means no skill levels are lost.
---

### Lose_Skill_Levels_PvE
Specifies the number of skill levels lost after a PvE death. A value of **0** means no skill levels are lost.
---

### Lose_Experience_PvP
Determines the percentage of experience retained after a PvP death. A value of **1** ensures no experience is lost.
---

### Lose_Experience_PvE
Determines the percentage of experience retained after a PvE death. A value of **1** ensures no experience is lost.
---

### Lose_Items_PvP
Specifies the percentage of items lost on a PvP death. A value of **0** means all items are dropped. Skillset loadouts may override this setting.
---

### Lose_Items_PvE
Specifies the percentage of items lost on a PvE death. A value of **0** means all items are dropped. Skillset loadouts may override this setting.
---

### Lose_Clothes_PvP
Determines if clothing items are dropped upon PvP deaths.
---

### Lose_Clothes_PvE
Determines if clothing items are dropped upon PvE deaths.
---

### Lose_Weapons_PvP
Indicates whether weapons in the Primary and Secondary slots are dropped upon PvP deaths.
---

### Lose_Weapons_PvE
Indicates whether weapons in the Primary and Secondary slots are dropped upon PvE deaths.
---

### Can_Hurt_Legs
Specifies whether players can take fall damage.
---

### Can_Break_Legs
Determines if players can receive the "Broken Bones" debuff.
---

### Can_Fix_Legs
Allows players to naturally recover from the "Broken Bones" debuff over time.
---

### Can_Start_Bleeding
Indicates whether players can get the "Bleeding" debuff.
---

### Can_Stop_Bleeding
Allows players to naturally recover from the "Bleeding" debuff over time.
---

### Spawn_With_Max_Skills
Specifies whether players spawn with all skills at maximum level.
---

### Spawn_With_Stamina_Skills
Determines if players spawn with Cardio, Exercise, Diving, and Parkour skills at their maximum levels.
---

### Allow_Instakill_Headshots
Enables instant kills with headshots using ranged weapons for example Ekho, Grizzly, and Timberwolf.
---

### Allow_Per_Character_Saves
Allows players to use multiple character saves enabling separate inventories and stats per character. This is enabled by default in single-player mode but disabled in multiplayer.
---
