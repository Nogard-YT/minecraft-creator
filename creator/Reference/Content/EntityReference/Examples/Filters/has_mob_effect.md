---
author: mammerla
ms.author: mikeam
title: Entity Documentation - has_mob_effect
ms.prod: gaming
description: "A reference document detailing the 'has_mob_effect' entity filter"
---

# Entity Documentation - has_mob_effect

Tests whether the Subject has the specified mob effect.

## Parameters

> [!IMPORTANT]
> `has_mob_effect` does **not** require any parameters to work properly. It can be used as a standalone filter.
>
> `has_mob_effect` can use `subject`. [operator](../Definitions/NestedTables/operator.md) and `value` parameters.

### subject

| Options| Description |
|:-----------|:-----------|
| block| The block involved with the interaction. |
| damager| The damaging entity involved with the interaction. |
| other| The other member of an interaction, not the caller. |
| parent| The caller's current parent. |
| player| The player involved with the interaction. |
| self| The entity or object calling the test |
| target| The caller's current target. |

### operator

| Options| Description |
|:-----------|:-----------|
| !=| Test for inequality. |
| <| Test for less-than the value. |
| <=| Test for less-than or equal to the value. |
| <>| Test for inequality. |
| =| Test for equality. |
| ==| Test for equality. |
| >| Test for greater-than the value. |
| >=| Test for greater-than or equal to the value. |
| equals| Test for equality. |
| not| Test for inequality. |

### value

|Name |Default Value  |Type  |Description  |
|---------|---------|---------|---------|
|value |*not set* |String |(Optional) A string value. |

## Example

### Full

```json
{ "test": "has_mob_effect", "subject": "self", "operator": "equals", "value": "" }
```

### Short (using Defaults)

```json
{ "test": "has_mob_effect" }
```

## Vanilla entities examples

### player

```json
{ "test": "has_mob_effect", "subject": "self", "value": "bad_omen" }
```

## Vanilla entities using `has_mob_effect`

- [player](../../../../Source/VanillaBehaviorPack_Snippets/entities/player.md)
