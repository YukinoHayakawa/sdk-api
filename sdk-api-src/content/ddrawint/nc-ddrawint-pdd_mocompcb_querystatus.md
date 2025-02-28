---
UID: NC:ddrawint.PDD_MOCOMPCB_QUERYSTATUS
title: PDD_MOCOMPCB_QUERYSTATUS (ddrawint.h)
description: The DdMoCompQueryStatus callback function queries the status of the most recent rendering operation to the specified surface.
old-location: display\ddmocompquerystatus.htm
tech.root: display
ms.assetid: af62d169-665a-43d2-ac0c-cc8ce6ce42d0
ms.date: 12/05/2018
ms.keywords: DdMoCompQueryStatus, DdMoCompQueryStatus callback function [Display Devices], PDD_MOCOMPCB_QUERYSTATUS, PDD_MOCOMPCB_QUERYSTATUS callback, ddfncs_8610d619-2c4f-41b4-8b28-4451019063b7.xml, ddrawint/DdMoCompQueryStatus, display.ddmocompquerystatus
f1_keywords:
- ddrawint/DdMoCompQueryStatus
dev_langs:
- c++
req.header: ddrawint.h
req.include-header: Winddi.h
req.target-type: Desktop
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- UserDefined
api_location:
- ddrawint.h
api_name:
- DdMoCompQueryStatus
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# PDD_MOCOMPCB_QUERYSTATUS callback function


## -description


The <b>DdMoCompQueryStatus</b> callback function queries the status of the most recent rendering operation to the specified surface. 


## -parameters




### -param Arg1








#### - lpStatusData

Points to a <a href="https://docs.microsoft.com/windows/desktop/api/ddrawint/ns-ddrawint-dd_querymocompstatusdata">DD_QUERYMOCOMPSTATUSDATA</a> structure that contains the information needed to query the status.


## -returns



<b>DdMoCompQueryStatus</b> returns one of the following callback codes:




## -remarks



DirectDraw drivers that support motion compensation must implement <b>DdMoCompQueryStatus</b>.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/ddrawint/ns-ddrawint-dd_querymocompstatusdata">DD_QUERYMOCOMPSTATUSDATA</a>
 

 

