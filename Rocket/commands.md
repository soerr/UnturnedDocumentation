---
position: 1
title: Commands
authors: MCrow
published: true
---

### Admin
The `admin` command is used to give a player admin blue hammer. Admin can use all commands and has access to all permissions.

**Syntax:** `/admin <player>`
- `<player>`: The name of the player to give admin to.

**Example:** `/admin MCrow`

### Unadmin
The `unadmin` command is used to remove admin blue hammer from a player.

**Syntax:** `/unadmin <player>`
- `<player>`: The name of the player to remove admin from.

**Example:** `/unadmin MCrow`

> **💡 PRO TIP**  
> Unfortunately there is no way to remove admin from someone who is offline. If you want you can delete all admins.  
Stop the server and delete the `Adminlist.dat` file which you will find in the same directory as `Commands.dat`.

### Ban
The `ban` command is used to ban a player from the server for a specified time.  

**Syntax:** `/ban <player> [reason] [time]`
- `<player>`: The name or Steam ID of the player to ban.
- `[reason]`: The reason for the ban.
- `[time]`: The duration of the ban in seconds. If not specified, the ban is permanent.

**Example:** `/ban MCrow "Griefing and cross-teaming" 3600`

> **💡 PRO TIP**  
> Remember to use the quotation marks for the reason if it has more than one word.

### Unban
The `unban` command is used to unban a player from the server. 

**Syntax:** `/unban <player>`
- `<player>`: The Steam ID of the player to unban.

**Example:** `/unban 76561198285897058`

> **💡 PRO TIP**  
> If you want to delete all bans from the server, stop the server and delete the `Blacklist.dat` file in the same directory as `Commands.dat`.

### Kick
The `kick` command is used to kick a player from the server.

**Syntax:** `/kick <player> [reason]`
- `<player>`: The name of the player to kick.
- `[reason]`: The reason for the kick.

**Example:** `/kick MCrow "Abusive language"`

### Spy
The `spy` command is used to take a screenshot of a player's screen. After using the command, you can view when you press the `ESC` key.

**Syntax:** `/spy <player>`
- `<player>`: The name of the player to spy on.

**Example:** `/spy MCrow`

### Kill
The `kill` command is used to kill a player.

**Syntax:** `/kill <player>`
- `<player>`: The name of the player to kill.

**Example:** `/kill MCrow`

### Permissions
The `permissions` command is used to display a list of all permissions.

**Syntax:** `/p`

### Vanish
The `vanish` command is used to make yourself invisible. It can be also used to disable the vanish mode.

**Syntax:** `/vanish`

### God
The `god` command is used to enable or disable god mode. When god mode is enabled, you are invincible.

**Syntax:** `/god`

### Heal
The `heal` command is used to heal a player or yourself.

**Syntax:** `/heal [player]`
- `[player]`: The name of the player to heal.

**Example:** `/heal MCrow`

### Tp
The `tp` command is used to teleport to a player.

**Syntax:** `/tp <player>`
- `<player>`: The name of the player to teleport to.

**Example:** `/tp MCrow`

### Tphere
The `tphere` command is used to teleport a player to you.

**Syntax:** `/tphere <player>`
- `<player>`: The name of the player to teleport to you.

**Example:** `/tphere MCrow`

### Item
The `item` command is used to spawn in items.

**Syntax:** `/i <item> [amount]`
- `<item>`: The name or id of the item to spawn.
- `[amount]`: The number of items to spawn. If not specified, the default amount is 1.

**Example:** `/i candy 20`

### Vehicle
The `vehicle` command is used to spawn in vehicles.

**Syntax:** `/v <vehicle>`
- `<vehicle>`: The name or id of the vehicle to spawn.

**Example:** `/v apc`
