---
position: 2
title: Permissions
authors: MCrow
published: true
---

Rocket permissions system allows you to define groups which are also known as ranks or roles. Each group can have a set of permissions to execute certain commands or actions.  

You will find `Permissions.config.xml` file in the `Rocket` directory.

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

### Prefix
The `<Prefix>` element is used to append a text before the player's name in chat.
