---
UID: NN:dbgmodel.IDebugHostSymbol2
title: IDebugHostSymbol2 (dbgmodel.h)
description: The IDebugHostSymbol2 (dbgmodel.h) interface defines methods that provide access to a particular symbol.
ms.date: 06/11/2019
keywords: ["IDebugHostSymbol2 interface"]
req.header: dbgmodel.h
req.include-header: 
req.target-type: 
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
targetos: Windows
tech.root: debugger
ms.custom: RS5
f1_keywords:
 - IDebugHostSymbol2
 - dbgmodel/IDebugHostSymbol2
topic_type:
 - apiref
api_type:
 - COM
api_location:
 - dbgmodel.h
api_name:
 - IDebugHostSymbol2
---

# IDebugHostSymbol2 interface


## -description

An interface to a particular symbol.

This version 2 of the interface supports all of the previous methods with identical signatures and includes additional new methods that provide added functionality. The new methods are listed in the header at the end of the section for that interface.

## -inheritance

IDebugHostSymbol2 inherits from [IDebugHostSymbol](nn-dbgmodel-idebughostsymbol.md).

## -remarks

Every symbol that can be returned from the data model host will derive in some fashion from [IDebugHostSymbol](nn-dbgmodel-idebughostsymbol.md). This is the core interface that every symbol implements regardless of the kind of symbol. Depending on the kind of symbol, a given symbol may implement a set of other interfaces which return attributes more unique to the particular kind of symbol represented by this interface.

## -see-also

[Debugger Data Model C++ Overview](/windows-hardware/drivers/debugger/data-model-cpp-overview)
