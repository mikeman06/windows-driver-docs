---
title: \_DXGKARG\_DESCRIBEPAGETABLE structure
description: The DXGKARG\_DESCRIBEPAGETABLE structure is reserved for system use. Do not use it in your driver.
ms.assetid: f439ba7c-216e-4286-9a63-d8f596996ac2
keywords: ["_DXGKARG_DESCRIBEPAGETABLE structure Display Devices", "DXGKARG_DESCRIBEPAGETABLE structure Display Devices"]
topic_type:
- apiref
api_name:
- DXGKARG_DESCRIBEPAGETABLE
api_location:
- d3dkmddi.h
api_type:
- HeaderDef
ms.author: windowsdriverdev
ms.date: 01/05/2018
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# \_DXGKARG\_DESCRIBEPAGETABLE structure


The DXGKARG\_DESCRIBEPAGETABLE structure is reserved for system use. Do not use it in your driver.

Syntax
------

```ManagedCPlusPlus
typedef struct _DXGKARG_DESCRIBEPAGETABLE {
  D3DGPU_VIRTUAL_ADDRESS CoverageStart;
  UINT                   CoverageSizeInBytes;
  UINT                   SizeInBytes;
  UINT                   SubtableOffset1;
  UINT                   SubtableOffset2;
} DXGKARG_DESCRIBEPAGETABLE;
```

Members
-------

**CoverageStart**
Reserved for system use.

**CoverageSizeInBytes**
Reserved for system use.

**SizeInBytes**
Reserved for system use.

**SubtableOffset1**
Reserved for system use.

**SubtableOffset2**
Reserved for system use.

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Version</p></td>
<td align="left"><p>Available in Windows 7 and later versions of the Windows operating systems.</p></td>
</tr>
<tr class="even">
<td align="left"><p>Header</p></td>
<td align="left">D3dkmddi.h (include D3dkmddi.h)</td>
</tr>
</tbody>
</table>

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[display\display]:%20_DXGKARG_DESCRIBEPAGETABLE%20structure%20%20RELEASE:%20%281/4/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




