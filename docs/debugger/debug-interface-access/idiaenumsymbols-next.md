---
description: "Retrieves a specified number of symbols in the enumeration sequence."
title: "IDiaEnumSymbols::Next"
ms.date: "11/04/2016"
ms.topic: "reference"
dev_langs:
  - "C++"
helpviewer_keywords:
  - "IDiaEnumSymbols::Next method"
author: "mikejo5000"
ms.author: "mikejo"
manager: jmartens
ms.technology: vs-ide-debug
---
# IDiaEnumSymbols::Next

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Retrieves a specified number of symbols in the enumeration sequence.

## Syntax

```C++
HRESULT Next ( 
   ULONG        celt,
   IDiaSymbol** rgelt,
   ULONG*       pceltFetched
);
```

#### Parameters
 celt

[in] The number of symbols in the enumerator to be retrieved.

 rgelt

[out] An array that is to be filled in with the [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md) objects that represent the desired symbols.

 pceltFetched

[out] Returns the number of symbols in the fetched enumerator.

## Return Value
 If successful, returns `S_OK`. Returns `S_FALSE` if there are no more symbols. Otherwise, returns an error code.

## Example

```C++
IDiaEnumSymbols* pEnum
CComPtr< IDiaSymbol> pSym;
DWORD celt;
pEnum->Next( 1, &pSym, &celt );
```

## See also
- [IDiaEnumSymbols](../../debugger/debug-interface-access/idiaenumsymbols.md)
- [IDiaSession::findLinesByLinenum](../../debugger/debug-interface-access/idiasession-findlinesbylinenum.md)
- [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md)
