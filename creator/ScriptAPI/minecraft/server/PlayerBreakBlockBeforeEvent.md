---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server.PlayerBreakBlockBeforeEvent Class
description: Contents of the @minecraft/server.PlayerBreakBlockBeforeEvent class.
---
# PlayerBreakBlockBeforeEvent Class

> [!CAUTION]
> This class is still in pre-release.  Its signature may change or it may be removed in future releases.

## Extends
- [*BlockEvent*](BlockEvent.md)

Contains information regarding an event before a player breaks a block.

## Properties

### **cancel**
`cancel: boolean;`

If set to true, cancels the block break event.

Type: *boolean*

### **itemStack**
`itemStack?: ItemStack;`

The item stack that is being used to break the block, or undefined if empty hand.

Type: [*ItemStack*](ItemStack.md)

### **player**
`read-only player: Player;`

Player breaking the block for this event.

Type: [*Player*](Player.md)
