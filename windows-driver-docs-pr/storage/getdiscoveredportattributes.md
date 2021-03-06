---
title: GetDiscoveredPortAttributes function
description: The GetDiscoveredPortAttributes WMI method retrieves the attributes for a specified remote Fibre Channel port.
ms.assetid: f71a02cf-035a-4de2-bb28-e1141a92795c
keywords: ["GetDiscoveredPortAttributes function Storage Devices"]
topic_type:
- apiref
api_name:
- GetDiscoveredPortAttributes
api_location:
- Hbaapi.lib
- Hbaapi.dll
api_type:
- LibDef
---

# GetDiscoveredPortAttributes function


The **GetDiscoveredPortAttributes** WMI method retrieves the attributes for a specified remote Fibre Channel port.

Syntax
------

```ManagedCPlusPlus
void GetDiscoveredPortAttributes(
   [in] uint32                                                        PortIndex,
   [in] uint32                                                        DiscoveredPortIndex,
   [out, HBA_STATUS_QUALIFIERS] HBA_STATUS                            HBAStatus,
   [out, HBAType("HBA_PORTATTRIBUTES")] MSFC_HBAPortAttributesResults PortAttributes
);
```

Parameters
----------

*PortIndex*   
The index of the local port of type Nx\_Port through which to query the discovered remote port. This information is delivered to the miniport driver in the **PortIndex** member of a [**GetDiscoveredPortAttributes\_IN**](https://msdn.microsoft.com/library/windows/hardware/ff553927) structure.

*DiscoveredPortIndex*   
The index of the remote port to be queried. This information is delivered to the miniport driver in the **DiscoveredPortIndex** member of a [**GetDiscoveredPortAttributes\_IN**](https://msdn.microsoft.com/library/windows/hardware/ff553927) structure.

*HBAStatus*   
On return, contains a WMI qualifier value that indicates the status of the operation. For a list of allowed values and their descriptions, see [HBA\_STATUS](hba-status.md). The miniport driver returns this information in the **HBAStatus** member of a [**GetDiscoveredPortAttributes\_OUT**](https://msdn.microsoft.com/library/windows/hardware/ff553930) structure.

*PortAttributes*   
A structure of type [**MSFC\_HBAPortAttributesResults**](https://msdn.microsoft.com/library/windows/hardware/ff562510) in which attributes for the discovered FC\_Port may be returned. The miniport driver returns this information in the **PortAttributes** member of a [**GetDiscoveredPortAttributes\_OUT**](https://msdn.microsoft.com/library/windows/hardware/ff553930) structure.

Return value
------------

Not applicable to WMI methods.

Remarks
-------

This WMI method belongs to the [MSFC\_HBAAdapterMethods WMI Class](msfc-hbaadaptermethods-wmi-class.md).

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Target platform</p></td>
<td align="left">Desktop</td>
</tr>
<tr class="even">
<td align="left"><p>Header</p></td>
<td align="left">Hbapiwmi.h (include Hbapiwmi.h, Hbaapi.h, or Hbaapi.h)</td>
</tr>
<tr class="odd">
<td align="left"><p>Library</p></td>
<td align="left">Hbaapi.lib</td>
</tr>
</tbody>
</table>

## <span id="see_also"></span>See also


[**GetDiscoveredPortAttributes\_IN**](https://msdn.microsoft.com/library/windows/hardware/ff553927)

[**GetDiscoveredPortAttributes\_OUT**](https://msdn.microsoft.com/library/windows/hardware/ff553930)

[**MSFC\_HBAPortAttributesResults**](https://msdn.microsoft.com/library/windows/hardware/ff562510)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[storage\storage]:%20GetDiscoveredPortAttributes%20function%20%20RELEASE:%20%281/11/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





