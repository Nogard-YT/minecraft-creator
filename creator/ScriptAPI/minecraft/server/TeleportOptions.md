---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server.TeleportOptions Interface
description: Contents of the @minecraft/server.TeleportOptions class.
---
# TeleportOptions Interface

Contains additional options for teleporting an entity.

## Properties

### **checkForBlocks**
`checkForBlocks?: boolean;`

Whether to check whether blocks will block the entity after teleport.

Type: *boolean*

### **dimension**
`dimension?: Dimension;`

Dimension to potentially move the entity to.  If not specified, the entity is teleported within the dimension that they reside.

Type: [*Dimension*](Dimension.md)

### **facingLocation**
`facingLocation?: Vector3;`

Location that the entity should be facing after teleport.

Type: [*Vector3*](Vector3.md)

### **keepVelocity**
`keepVelocity?: boolean;`

Whether to retain the entities velocity after teleport.

Type: *boolean*

### **rotation**
`rotation?: Vector2;`

Rotation of the entity after teleport.

Type: [*Vector2*](Vector2.md)

#### Examples
##### ***teleportMovement.ts***
```typescript
  const pig = overworld.spawnEntity("minecraft:pig", targetLocation);

  let inc = 1;
  let runId = mc.system.runInterval(() => {
    pig.teleport(
      { x: targetLocation.x + inc / 4, y: targetLocation.y + inc / 4, z: targetLocation.z + inc / 4 },
      {
        facingLocation: targetLocation,
      }
    );

    if (inc > 100) {
      mc.system.clearRun(runId);
    }
    inc++;
  }, 4);
```
