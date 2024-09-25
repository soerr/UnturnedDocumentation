---
position: 6
title: Zombies
authors: MCrow
published: true
---

![zombies](assets/zombies.png)

Zombies settings allow you to configure the behavior of zombies on your server. You can change the spawn chance, loot chance, and other settings to make the game more challenging or easier.

```json
"Zombies": {
  "Spawn_Chance": 0.2,
  "Loot_Chance": 0.55,
  "Crawler_Chance": 0.0,
  "Sprinter_Chance": 0.0,
  "Flanker_Chance": 0.0,
  "Burner_Chance": 0.0,
  "Acid_Chance": 0.0,
  "Boss_Electric_Chance": 0.0,
  "Boss_Wind_Chance": 0.0,
  "Boss_Fire_Chance": 0.0,
  "Spirit_Chance": 0.0,
  "DL_Red_Volatile_Chance": 0.0,
  "DL_Blue_Volatile_Chance": 0.0,
  "Boss_Elver_Stomper_Chance": 0.0,
  "Boss_Kuwait_Chance": 0.0,
  "Respawn_Day_Time": 360.0,
  "Respawn_Night_Time": 30.0,
  "Respawn_Beacon_Time": 0.0,
  "Quest_Boss_Respawn_Interval": 600.0,
  "Damage_Multiplier": 0.75,
  "Armor_Multiplier": 1.25,
  "Backstab_Multiplier": 1.25,
  "NonHeadshot_Armor_Multiplier": 1.0,
  "Beacon_Experience_Multiplier": 1.0,
  "Full_Moon_Experience_Multiplier": 2.0,
  "Min_Drops": 1,
  "Max_Drops": 1,
  "Min_Mega_Drops": 5,
  "Max_Mega_Drops": 5,
  "Min_Boss_Drops": 8,
  "Max_Boss_Drops": 10,
  "Slow_Movement": true,
  "Can_Stun": true,
  "Only_Critical_Stuns": false,
  "Weapons_Use_Player_Damage": false,
  "Can_Target_Barricades": true,
  "Can_Target_Structures": true,
  "Can_Target_Vehicles": true,
  "Beacon_Max_Rewards": 0,
  "Beacon_Max_Participants": 0,
  "Beacon_Rewards_Multiplier": 1.0
}
```

### Spawn_Chance
Percent chance (represented as a decimal) for any given zombie spawn node to spawn a zombie. Value must be within a range of **0.0** to **1.0**.

For example **0.2** means **20%** chance to spawn a zombie. Setting this value to **0.0** will prevent zombies from spawning.

Zombie spawn nodes on official maps:
- **PEI** - 1451
- **Washington** - 1137
- **Yukon** - 524
- **Russia** - 2458
- **Germany** - 1955

### Loot_Chance
Percent chance (represented as a decimal) for any given zombie to drop loot. Value must be within a range of **0.0** to **1.0**.

![](assets/zombies_loot_chance.png)


| Zombie Type | Picture | 
| --- | --- |
| Crawler | ![](assets/zombie_crawler.png) |
| Sprinter | ![](assets/zombie_sprinter.png) |
| Flanker | ![](assets/zombie_flanker.png) |
| Burner | ![](assets/zombie_burner.png) |
| Acid | ![](assets/zombie_acid.png) |

### Video Tutorial
Check out our video tutorial on how to increase number of items dropped by zombies and loot on your server.

[video=affd02b0-e416-4fbe-8363-86e4b2639813] 