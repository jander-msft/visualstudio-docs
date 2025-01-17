---
description: "Sets the locale for the port supplier."
title: IDebugPortSupplierLocale2::SetLocale
ms.date: 11/04/2016
ms.topic: reference
helpviewer_keywords:
- IDebugPortSupplierLocale2::SetLocale
author: maiak
ms.author: maiak
manager: jmartens
ms.technology: vs-ide-debug
dev_langs:
- CPP
- CSharp
---
# IDebugPortSupplierLocale2::SetLocale

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Sets the locale for the port supplier.

## Syntax

### [C#](#tab/csharp)
```csharp
int SetLocale(
   ushort wLangID
);
```
### [C++](#tab/cpp)
```cpp
HRESULT SetLocale(
   WORD wLangID
);
```
---

## Parameters
`wLangID`\
Identifier for the locale to set.

## Return Value
 If successful, returns `S_OK`; otherwise, returns an error code.

## See also
- [IDebugPortSupplierLocale2](../../../extensibility/debugger/reference/idebugportsupplierlocale2.md)
