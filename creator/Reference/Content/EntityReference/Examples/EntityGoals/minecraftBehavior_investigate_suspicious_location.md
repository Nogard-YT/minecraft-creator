---
author: iconicNurdle
ms.author: mikeam
title: Entity Documentation - minecraft:behavior.investigate_suspicious_location
ms.prod: gaming
description: "A reference document detailing the 'behavior.investigate_suspicious_location' entity goal"
---

# Entity Documentation - minecraft:behavior.investigate_suspicious_location

`minecraft:behavior.investigate_suspicious_location` compels the entity to move towards a "suspicious" position based on data gathered in `minecraft:suspect_tracking`.

## Parameters

| Name| Default Value| Type| Description |
|:-----------:|:-----------:|:-----------:|:-----------:|
| goal_radius| 1.5| Decimal| Distance in blocks within the entity considers it has reached its target position. |
| priority|*not set*|Integer|The higher the priority, the sooner this behavior will be executed as a goal.|
| speed_multiplier| 1| Decimal| Movement speed multiplier. |

## Vanilla entities examples

### warden

```json
"minecraft:behavior.investigate_suspicious_location": {
  "priority": 5,
  "speed_multiplier": 0.7
}
```

## Vanilla entities using `investigate_suspicious_location`

- [warden](../../../../Source/VanillaBehaviorPack_Snippets/entities/warden.md)
