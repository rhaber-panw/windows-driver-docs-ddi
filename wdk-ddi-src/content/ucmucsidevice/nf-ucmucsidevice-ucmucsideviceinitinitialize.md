---
UID: NF:ucmucsidevice.UcmUcsiDeviceInitInitialize
title: UcmUcsiDeviceInitInitialize function (ucmucsidevice.h)
tech.root: usbref
description: Initializes the **WDFDEVICE_INIT** provided by the framework.
ms.date: 09/30/2018
keywords: ["UcmUcsiDeviceInitInitialize function"]
ms.keywords: UcmUcsiDeviceInitInitialize
req.header: ucmucsidevice.h
req.include-header: UcmUcsiCx.h
req.target-type: 
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 1.27
req.umdf-ver: N/A
req.lib: UcmUcsiCxStub.lib
req.dll: 
req.irql: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
targetos: Windows
ms.custom: RS5
f1_keywords:
 - UcmUcsiDeviceInitInitialize
 - ucmucsidevice/UcmUcsiDeviceInitInitialize
topic_type:
 - apiref
api_type:
 - LibDef
api_location:
 - UcmUcsiCxStub.lib
api_name:
 - UcmUcsiDeviceInitInitialize
---

# UcmUcsiDeviceInitInitialize function


## -description

Intializes the [**WDFDEVICE_INIT**](/windows-hardware/drivers/wdf/wdfdevice_init) provided by the framework.

## -parameters

### -param DeviceInit

A pointer to a framework-allocated [**WDFDEVICE_INIT**](/windows-hardware/drivers/wdf/wdfdevice_init) structure.

## -returns

Returns STATUS_SUCCESS if the operation succeeds. Otherwise, returns an appropriate [NTSTATUS](/windows-hardware/drivers/kernel/ntstatus-values) code.

## -remarks

The client driver must call this function after calling [**WdfDeviceInitSetPnpPowerEventCallbacks**](../wdfdevice/nf-wdfdevice-wdfdeviceinitsetpnppowereventcallbacks.md). This function initializes the UCSI extension (UcmUcsiCx) with the framework **WDFDEVICE_INIT** structure that contains pointers to PnP and power callback functions implemented by the client driver.

## -see-also

