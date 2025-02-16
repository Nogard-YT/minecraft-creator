---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server.WeatherChangeAfterEventSignal Class
description: Contents of the @minecraft/server.WeatherChangeAfterEventSignal class.
---
# WeatherChangeAfterEventSignal Class

> [!CAUTION]
> This class is still in pre-release.  Its signature may change or it may be removed in future releases.

Manages callbacks that are connected to weather changing.

## Methods
- [subscribe](#subscribe)
- [unsubscribe](#unsubscribe)

### **subscribe**
`
subscribe(callback: (arg: WeatherChangeAfterEvent) => void): (arg: WeatherChangeAfterEvent) => void
`

Adds a callback that will be called when weather changes.

#### **Parameters**
- **callback**: (arg: [*WeatherChangeAfterEvent*](WeatherChangeAfterEvent.md)) => *void*

#### **Returns** (arg: [*WeatherChangeAfterEvent*](WeatherChangeAfterEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

### **unsubscribe**
`
unsubscribe(callback: (arg: WeatherChangeAfterEvent) => void): void
`

Removes a callback from being called when weather changes.

#### **Parameters**
- **callback**: (arg: [*WeatherChangeAfterEvent*](WeatherChangeAfterEvent.md)) => *void*

> [!IMPORTANT]
> This function can't be called in read-only mode.

> [!WARNING]
> This function can throw errors.
