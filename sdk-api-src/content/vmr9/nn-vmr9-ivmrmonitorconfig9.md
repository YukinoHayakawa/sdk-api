---
UID: NN:vmr9.IVMRMonitorConfig9
title: IVMRMonitorConfig9 (vmr9.h)
description: The IVMRMonitorConfig9 interface is implemented by the Video Mixing Renderer Filter 9 (VMR-9).
old-location: dshow\ivmrmonitorconfig9.htm
tech.root: DirectShow
ms.assetid: 27a3a598-d8de-48b2-8b8c-6b5497db4c6c
ms.date: 12/05/2018
ms.keywords: IVMRMonitorConfig9, IVMRMonitorConfig9 interface [DirectShow], IVMRMonitorConfig9 interface [DirectShow],described, IVMRMonitorConfig9Interface, dshow.ivmrmonitorconfig9, vmr9/IVMRMonitorConfig9
f1_keywords:
- vmr9/IVMRMonitorConfig9
dev_langs:
- c++
req.header: vmr9.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2 [desktop apps only]
req.target-min-winversvr: Windows Server 2003 R2 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Strmiids.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Strmiids.lib
- Strmiids.dll
api_name:
- IVMRMonitorConfig9
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IVMRMonitorConfig9 interface


## -description



The <code>IVMRMonitorConfig9</code> interface is implemented by the <a href="https://docs.microsoft.com/windows/desktop/DirectShow/video-mixing-renderer-filter-9">Video Mixing Renderer Filter 9</a> (VMR-9). Applications use this interface to determine the capabilities of the display devices on the system and to control which device is used to display the output. For example, if the system contains a hardware DVD decoder and the VMR is rendering the output from that decoder, then on a multi-monitor system, an application must use this interface to specify the display device that is connected to the decoder.

The VMR-9 supports a maximum of 16 display devices.




## -inheritance

The <b xmlns:loc="http://microsoft.com/wdcml/l10n">IVMRMonitorConfig9</b> interface inherits from the <a href="https://docs.microsoft.com/windows/desktop/api/unknwn/nn-unknwn-iunknown">IUnknown</a> interface. <b>IVMRMonitorConfig9</b> also has these types of members:
<ul>
<li><a href="https://docs.microsoft.com/">Methods</a></li>
</ul>

## -members

The <b>IVMRMonitorConfig9</b> interface has these methods.
<table class="members" id="memberListMethods">
<tr>
<th align="left" width="37%">Method</th>
<th align="left" width="63%">Description</th>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/vmr9/nf-vmr9-ivmrmonitorconfig9-getavailablemonitors">GetAvailableMonitors</a>
</td>
<td align="left" width="63%">
Retrieves information about the monitors currently available on the system.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/vmr9/nf-vmr9-ivmrmonitorconfig9-getdefaultmonitor">GetDefaultMonitor</a>
</td>
<td align="left" width="63%">
Retrieves the default monitor that all future instances of the VMR will use for video playback.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/vmr9/nf-vmr9-ivmrmonitorconfig9-getmonitor">GetMonitor</a>
</td>
<td align="left" width="63%">
Retrieves the monitor that this instance of the VMR is using for video playback.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/vmr9/nf-vmr9-ivmrmonitorconfig9-setdefaultmonitor">SetDefaultMonitor</a>
</td>
<td align="left" width="63%">
Specifies the default monitor that all future instances of the VMR should use for video playback.

</td>
</tr>
<tr data="declared;">
<td align="left" width="37%">
<a href="https://docs.microsoft.com/windows/desktop/api/vmr9/nf-vmr9-ivmrmonitorconfig9-setmonitor">SetMonitor</a>
</td>
<td align="left" width="63%">
On a multi-monitor system, specifies the monitor that this instance of the VMR should use for video playback.

</td>
</tr>
</table> 


## -remarks



Include DShow.h and D3d9.h before Vmr9.h.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/DirectShow/using-the-video-mixing-renderer">Using the Video Mixing Renderer</a>
 

 

