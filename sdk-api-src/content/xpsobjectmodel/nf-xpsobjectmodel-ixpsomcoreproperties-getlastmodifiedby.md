---
UID: NF:xpsobjectmodel.IXpsOMCoreProperties.GetLastModifiedBy
title: IXpsOMCoreProperties::GetLastModifiedBy (xpsobjectmodel.h)
description: Gets the lastModifiedBy property.
old-location: xps\ixpsomcoreproperties_getlastmodifiedby.htm
tech.root: printdocs
ms.assetid: e3e68656-ae4d-45f4-bb2a-3c4c5cecbbae
ms.date: 12/05/2018
ms.keywords: GetLastModifiedBy, GetLastModifiedBy method [XPS Documents and Packaging], GetLastModifiedBy method [XPS Documents and Packaging],IXpsOMCoreProperties interface, IXpsOMCoreProperties interface [XPS Documents and Packaging],GetLastModifiedBy method, IXpsOMCoreProperties.GetLastModifiedBy, IXpsOMCoreProperties::GetLastModifiedBy, xps.ixpsomcoreproperties_getlastmodifiedby, xpsobjectmodel/IXpsOMCoreProperties::GetLastModifiedBy
f1_keywords:
- xpsobjectmodel/IXpsOMCoreProperties.GetLastModifiedBy
dev_langs:
- c++
req.header: xpsobjectmodel.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 7, Windows Vista with SP2 and Platform Update for Windows Vista [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2008 R2, Windows Server 2008 with SP2 and Platform Update for Windows Server 2008 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: XpsObjectModel.idl
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
- COM
api_location:
- xpsobjectmodel.h
api_name:
- IXpsOMCoreProperties.GetLastModifiedBy
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IXpsOMCoreProperties::GetLastModifiedBy


## -description


Gets the <b>lastModifiedBy</b> property.


## -parameters




### -param lastModifiedBy [out, retval]

The value that is read from the <b>lastModifiedBy</b> property.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the table that follows. For information about  XPS document API return values that are not listed in this table, see <a href="https://docs.microsoft.com/previous-versions/windows/desktop/dd372955(v=vs.85)">XPS Document Errors</a>.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_POINTER</b></dt>
</dl>
</td>
<td width="60%">
<i>lastModifiedBy</i> is <b>NULL</b>.

</td>
</tr>
</table>
 




## -remarks



The <b>lastModifiedBy</b> property describes the user who performed the last modification.

This method allocates the memory used by the string that is returned in <i>lastModifiedBy</i>.  If <i>lastModifiedBy</i> is not <b>NULL</b>, use the <a href="https://docs.microsoft.com/windows/desktop/api/combaseapi/nf-combaseapi-cotaskmemfree">CoTaskMemFree</a> function  to free the memory.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/xpsobjectmodel/nn-xpsobjectmodel-ixpsomcoreproperties">IXpsOMCoreProperties</a>



<a href="https://go.microsoft.com/fwlink/p/?linkid=123375">Standard ECMA-376, Office Open XML File Formats</a>



<a href="http://go.microsoft.com/?linkid=8435939">XML Paper Specification</a>



<a href="https://docs.microsoft.com/previous-versions/windows/desktop/dd372955(v=vs.85)">XPS Document Errors</a>
 

 

