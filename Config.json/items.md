---
position: 4
title: Items
authors: MCrow
published: true
---

```json
"Items": {
    "Spawn_Chance": 0.35,
    "Despawn_Dropped_Time": 600.0,
    "Despawn_Natural_Time": 900.0,
    "Respawn_Time": 50.0,
    "Quality_Full_Chance": 0.1,
    "Quality_Multiplier": 1.0,
    "Gun_Bullets_Full_Chance": 0.1,
    "Gun_Bullets_Multiplier": 1.0,
    "Magazine_Bullets_Full_Chance": 0.1,
    "Magazine_Bullets_Multiplier": 1.0,
    "Crate_Bullets_Full_Chance": 0.1,
    "Crate_Bullets_Multiplier": 1.0,
    "Has_Durability": false,
    "Food_Spawns_At_Full_Quality": true,
    "Water_Spawns_At_Full_Quality": true,
    "Clothing_Spawns_At_Full_Quality": true,
    "Weapons_Spawn_At_Full_Quality": true,
    "Default_Spawns_At_Full_Quality": true,
    "Clothing_Has_Durability": false,
    "Weapons_Have_Durability": false
}
```

### Has_Durability
Original option for disabling item quality. If false, items spawn at 100% quality and their quality doesn't decrease.  
If this is set to false, then all below settings are ignored.

### Food_Spawns_At_Full_Quality
Food-specific replacement for `Has_Durability`. If true, food spawns at 100% quality.

### Water_Spawns_At_Full_Quality
Water-specific replacement for `Has_Durability`. If true, water spawns at 100% quality.

### Clothing_Spawns_At_Full_Quality
Clothing-specific replacement for `Has_Durability`. If true, clothing spawns at 100% quality.

### Weapons_Spawn_At_Full_Quality
Weapon-specific replacement for `Has_Durability`. If true, weapons spawns at 100% quality.

### Default_Spawns_At_Full_Quality
Fallback used when spawning an item that doesn't fit into one of the other quality/durability settings. If true, items spawn at 100% quality.

### Clothing_Has_Durability
Clothing-specific replacement for `Has_Durability`. If false, clothing quality doesn't decrease when damaged.

### Weapons_Have_Durability
Melee and gun replacement for `Has_Durability`. Defaults to true. If false, weapons quality doesn't decrease when used.

### Video Tutorial
Check out our video tutorial on how to increase spawn chance of items and loot on your server.

[video=affd02b0-e416-4fbe-8363-86e4b2639813] 