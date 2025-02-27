---
UID: NF:dwmapi.DwmUnregisterThumbnail
title: DwmUnregisterThumbnail function (dwmapi.h)
description: Removes a Desktop Window Manager (DWM) thumbnail relationship created by the DwmRegisterThumbnail function.
old-location: dwm\dwmunregisterthumbnail.htm
tech.root: dwm
ms.assetid: VS|winui|~\winui\desktopwindowmanager\reference\functions\dwmunregisterthumbnail.htm
ms.date: 12/05/2018
ms.keywords: DwmUnregisterThumbnail, DwmUnregisterThumbnail function [Desktop Window Manager], _udwm_dwmunregisterthumbnail, _udwm_dwmunregisterthumbnail_cpp, dwm.dwmunregisterthumbnail, dwmapi/DwmUnregisterThumbnail, winui._udwm_dwmunregisterthumbnail
f1_keywords:
- dwmapi/DwmUnregisterThumbnail
dev_langs:
- c++
req.header: dwmapi.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Dwmapi.lib
req.dll: Dwmapi.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Dwmapi.dll
api_name:
- DwmUnregisterThumbnail
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# DwmUnregisterThumbnail function


## -description


Removes a Desktop Window Manager (DWM) thumbnail relationship created by the <a href="https://docs.microsoft.com/windows/desktop/api/dwmapi/nf-dwmapi-dwmregisterthumbnail">DwmRegisterThumbnail</a> function.


## -parameters




### -param hThumbnailId

The handle to the thumbnail relationship to be removed. Null or non-existent handles will result in a return value of E_INVALIDARG.


## -returns



If this function succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



Unregistering DWM thumbnail relationships must be done within the process that registered the relationships.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/dwm/thumbnail-ovw">DWM Thumbnail Overview</a>



<a href="https://docs.microsoft.com/windows/desktop/dwm/dwm-overview">Desktop Window Manager Overview</a>



<a href="https://docs.microsoft.com/windows/desktop/api/dwmapi/nf-dwmapi-dwmquerythumbnailsourcesize">DwmQueryThumbnailSourceSize</a>



<a href="https://docs.microsoft.com/windows/desktop/api/dwmapi/nf-dwmapi-dwmupdatethumbnailproperties">DwmUpdateThumbnailProperties</a>
 

 

