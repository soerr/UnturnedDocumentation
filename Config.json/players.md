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
Determines the amount of health a player spawns with. Must be between **0** and **255**.
- Default: **100**
- Example: Setting this to **200** means players will spawn with double the health.

---

### Health_Regen_Min_Food
The minimum amount of food required for health regeneration to begin.
- Default: **90**
- Example: Lowering this to **50** makes it easier for health to regenerate with less food.

---

### Health_Regen_Min_Water
The minimum amount of water required for health regeneration to begin.
- Default: **90**
- Example: Reducing this to **60** allows health to regenerate even with lower hydration levels.

---

### Health_Regen_Ticks
Controls how often health regenerates, measured in ticks. A lower value regenerates health faster.
- Default: **60**
- Example: Setting this to **30** will make health regenerate twice as quickly.

---

### Food_Default
The starting amount of food players have when they spawn, between **0** and **255**.
- Default: **100**
- Example: If this is set to **85**, players spawn with slightly less food.

---

### Water_Default
The starting amount of water players have when they spawn, between **0** and **255**.
- Default: **100**
- Example: Setting this to **85** means players start with less hydration.

---

### Virus_Default
The immunity level players start with upon spawning. Must be between **0** and **255**.
- Default: **100**
- Example: Lowering this to **50** means players are more susceptible to infections.

---

### Virus_Infect
Threshold at which immunity begins to deplete until treated. Setting to **0** disables untreated infections.
- Default: **50**
- Example: Raising this to **75** makes it harder for infections to occur.
