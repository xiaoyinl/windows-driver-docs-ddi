---
UID: NS:d3d12umddi.D3D12DDI_RENDER_PASS_BEGINNING_ACCESS_RESUME_LOCAL_READ_PARAMETERS
title: D3D12DDI_RENDER_PASS_BEGINNING_ACCESS_RESUME_LOCAL_READ_PARAMETERS
author: windows-driver-content
description: 
ms.assetid: e27305cb-2fe3-40e8-b102-05d665ed2698
ms.author: windowsdriverdev
ms.date: 
ms.topic: struct
ms.prod: windows-hardware
ms.technology: windows-devices
ms.keywords: D3D12DDI_RENDER_PASS_BEGINNING_ACCESS_RESUME_LOCAL_READ_PARAMETERS, D3D12DDI_RENDER_PASS_BEGINNING_ACCESS_RESUME_LOCAL_READ_PARAMETERS, 
req.header: d3d12umddi.h
req.include-header:
req.target-type:
req.target-min-winverclnt: Windows 10, version 1809
req.target-min-winversvr:
req.kmdf-ver:
req.umdf-ver:
req.lib:
req.dll:
req.ddi-compliance:
req.unicode-ansi:
req.max-support:
req.typenames: D3D12DDI_RENDER_PASS_BEGINNING_ACCESS_RESUME_LOCAL_READ_PARAMETERS
topic_type: 
-	apiref
api_type: 
-	HeaderDef
api_location: 
-	d3d12umddi.h
api_name: 
-	D3D12DDI_RENDER_PASS_BEGINNING_ACCESS_RESUME_LOCAL_READ_PARAMETERS
product:
-	Windows
targetos: Windows
tech.root: display
---

# D3D12DDI_RENDER_PASS_BEGINNING_ACCESS_RESUME_LOCAL_READ_PARAMETERS structure

## -description

Specifies the kernel size of the read, or how many surrounding pixels are needed.

> [!NOTE] 
> The parameters here must match those on the [D3D12DDI_RENDER_PASS_ENDING_ACCESS_SUSPEND_LOCAL_READ_PARAMETERS](ns-d3d12umddi-d3d12ddi_render_pass_ending_access_suspend_local_read_parameters.md) structure.

## -struct-fields

### -field AdditionalWidth

The width in pixels. '0' means no pixels on either side, '1' pixel means one pixel on each side, for a total of three pixels of width.

### -field AdditionalHeight

The height in pixels.

## -remarks

## -see-also