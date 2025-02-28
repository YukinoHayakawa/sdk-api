---
UID: NF:winuser.GetCursorInfo
title: GetCursorInfo function (winuser.h)
description: Retrieves information about the global cursor.
old-location: menurc\getcursorinfo.htm
tech.root: menurc
ms.assetid: VS|winui|~\winui\windowsuserinterface\resources\cursors\cursorreference\cursorfunctions\getcursorinfo.htm
ms.date: 12/05/2018
ms.keywords: GetCursorInfo, GetCursorInfo function [Menus and Other Resources], _win32_GetCursorInfo, _win32_getcursorinfo_cpp, menurc.getcursorinfo, winui._win32_getcursorinfo, winuser/GetCursorInfo
f1_keywords:
- winuser/GetCursorInfo
dev_langs:
- c++
req.header: winuser.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: User32.lib
req.dll: User32.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- User32.dll
- Ext-MS-Win-NTUser-GUI-l1-1-0.dll
- Ext-MS-Win-NTUser-GUI-l1-1-1.dll
- Ext-MS-Win-NTUser-GUI-l1-2-0.dll
- api-ms-win-ntuser-ie-gui-l1-1-0.dll
- ie_stubs.dll
- ext-ms-win-ntuser-gui-l1-2-1.dll
- Ext-MS-Win-RTCore-NTUser-Cursor-L1-1-0.dll
- MinUser.dll
api_name:
- GetCursorInfo
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# GetCursorInfo function


## -description


Retrieves information about the global cursor.


## -parameters




### -param pci [in, out]

Type: <b>PCURSORINFO</b>

A pointer to a <a href="https://docs.microsoft.com/windows/desktop/menurc/o">CURSORINFO</a> structure that receives the information. Note that you must set the <b>cbSize</b> member to <code>sizeof(CURSORINFO)</code> before calling this function. 


## -returns



Type: <b>BOOL</b>

If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call <a href="https://docs.microsoft.com/windows/desktop/api/errhandlingapi/nf-errhandlingapi-getlasterror">GetLastError</a>. 




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/menurc/o">CURSORINFO</a>



<b>Conceptual</b>



<a href="https://docs.microsoft.com/windows/desktop/menurc/cursors">Cursors</a>



<a href="https://docs.microsoft.com/windows/desktop/api/winuser/nf-winuser-getguithreadinfo">GetGUIThreadInfo</a>



<b>Reference</b>
 

 

