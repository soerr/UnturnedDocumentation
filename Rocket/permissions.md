---
position: 2
title: Permissions
authors: MCrow
published: true
---

Rocket permissions system allows you to define groups which are also known as ranks or roles. Each group can have a set of permissions to execute certain commands or actions.  

You will find `Permissions.config.xml` file in the `Rocket` directory of your server.

Having done changes to the permissions file, you need to restart the server or use the `/p reload` command to apply the changes.

```xml
<?xml version="1.0" encoding="utf-8"?>
<RocketPermissions xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
  <DefaultGroup>default</DefaultGroup>
  <Groups>
    <Group>
      <Id>default</Id>
      <DisplayName>Guest</DisplayName>
      <Prefix />
      <Suffix />
      <Color>white</Color>
      <Members />
      <Priority>100</Priority>
      <Permissions>
        <Permission Cooldown="0">p</Permission>
        <Permission Cooldown="0">compass</Permission>
        <Permission Cooldown="0">rocket</Permission>
      </Permissions>
    </Group>
    <Group>
      <Id>vip</Id>
      <DisplayName>VIP</DisplayName>
      <Prefix />
      <Suffix />
      <Color>FF9900</Color>
      <Members>
        <Member>76561198016438091</Member>
      </Members>
      <ParentGroup>default</ParentGroup>
      <Priority>100</Priority>
      <Permissions>
        <Permission Cooldown="0">effect</Permission>
        <Permission Cooldown="120">heal</Permission>
        <Permission Cooldown="30">v</Permission>
      </Permissions>
    </Group>
  </Groups>
</RocketPermissions>
```

### DefaultGroup
The `<DefaultGroup>` specifies which of the groups should be used as default that is assigned to every player who joins the server.  
The value must be the `<Id>` value of the group.

### Groups
The `<Groups>` element consists of multiple `<Group>` items.  
When adding a new group, it needs to be placed inside the `<Groups>` element.

### Group
Each `<Group>` element represents a single group with its settings and permissions.

### Id
The `<Id>` element is the unique identifier of the group. It is used to reference the group in other parts of the configuration and when assigning a group to a player using a command, for example: `/p add MCrow vip`.

### DisplayName
As the name suggests, `<DisplayName>` value is a public name of the group shown to players for example when they use `/p` command to view their groups and permissions.

![your groups](assets/your_groups.png "/p command output in-game")

### Prefix
The `<Prefix>` element is used to append a text before the player's name.

```xml
<Prefix>[Survivor] </Prefix>
```

![survivor prefix](assets/survivor_prefix.png "[Survivor] prefix in-game")

> **💡 PRO TIP**  
> Notice the space after the prefix text. It is important to add a space after the prefix text to separate it from the player's name. Same goes for the suffix text.

### Suffix
The `<Suffix>` element is used to append a text after the player's name.

```xml
<Suffix> [VIP]</Suffix>
```

![vip suffix](assets/vip_suffix.png "[Survivor] prefix and [VIP] suffix in-game")

> **💡 PRO TIP**  
> If you give rank with prefix or suffix to a player while they are already on the server, they will have to reconnect to apply the changes.