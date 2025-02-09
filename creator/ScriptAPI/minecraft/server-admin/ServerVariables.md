---
# DO NOT TOUCH — This file was automatically generated. See https://github.com/mojang/minecraftapidocsgenerator to modify descriptions, examples, etc.
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server-admin.ServerVariables Class
description: Contents of the @minecraft/server-admin.ServerVariables class.
---
# ServerVariables Class

A collection of server variables defined in dedicated server configuration.

## Properties

### **names**
`read-only names: string[];`

A list of available, configured server variables.

Type: *string*[]

## Methods
- [get](#get)

### **get**
`
"get"(name: string): any | undefined
`

Returns the value of variable that has been configured in a dedicated server configuration JSON file.

#### **Parameters**
- **name**: *string*

#### **Returns** *any* | *undefined*

> [!IMPORTANT]
> This function can't be called in read-only mode.

#### Examples
##### ***getPlayerProfile.ts***
```typescript
  const serverUrl = mcsa.variables.get("serverEndpoint");

  const req = new mcnet.HttpRequest(serverUrl + "getPlayerProfile");

  req.body = JSON.stringify({
    playerId: "johndoe",
  });

  const authTokenSec = mcsa.secrets.get("authtoken");

  if (!authTokenSec) {
    throw new Error("authtoken secret not defined.");
  }

  req.method = mcnet.HttpRequestMethod.POST;
  req.headers = [new mcnet.HttpHeader("Content-Type", "application/json"), new mcnet.HttpHeader("auth", authTokenSec)];

  await mcnet.http.request(req);
```
