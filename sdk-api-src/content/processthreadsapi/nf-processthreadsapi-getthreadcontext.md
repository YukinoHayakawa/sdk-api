---
UID: NF:processthreadsapi.GetThreadContext
title: GetThreadContext function (processthreadsapi.h)
description: Retrieves the context of the specified thread.
old-location: base\getthreadcontext.htm
tech.root: Debug
ms.assetid: 3b65283e-34d2-4374-87fe-fa8ae45fbbcf
ms.date: 12/05/2018
ms.keywords: GetThreadContext, GetThreadContext function, _win32_getthreadcontext, base.getthreadcontext, processthreadsapi/GetThreadContext
f1_keywords:
- processthreadsapi/GetThreadContext
dev_langs:
- c++
req.header: processthreadsapi.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP [desktop apps \| UWP apps]
req.target-min-winversvr: Windows Server 2003 [desktop apps \| UWP apps]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Kernel32.lib
req.dll: Kernel32.dll
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- DllExport
api_location:
- Kernel32.dll
- API-MS-Win-Core-ProcessThreads-l1-1-1.dll
- KernelBase.dll
- MinKernelBase.dll
- API-MS-Win-Core-ProcessThreads-l1-1-2.dll
- api-ms-win-downlevel-kernel32-l1-1-0.dll
- API-MS-Win-Core-ProcessThreads-L1-1-3.dll
api_name:
- GetThreadContext
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# GetThreadContext function


## -description


Retrieves the context of the specified thread.

A 64-bit application can retrieve the context of a WOW64 thread using the 
    <a href="https://docs.microsoft.com/windows/desktop/api/winbase/nf-winbase-wow64getthreadcontext">Wow64GetThreadContext</a> function.


## -parameters




### -param hThread [in]

A handle to the thread whose context is to be retrieved. The handle must have 
      <b>THREAD_GET_CONTEXT</b> access to the thread. For more information, see 
      <a href="https://docs.microsoft.com/windows/desktop/ProcThread/thread-security-and-access-rights">Thread Security and Access Rights</a>.
      

<b>WOW64:  </b>The handle must also have <b>THREAD_QUERY_INFORMATION</b> access.


### -param lpContext [in, out]

A pointer to a <a href="https://docs.microsoft.com/windows/desktop/api/winnt/ns-winnt-arm64_nt_context">CONTEXT</a> structure that receives the 
      appropriate context of the specified thread. The value of the <b>ContextFlags</b> member of 
      this structure specifies which portions of a thread's context are retrieved. The 
      <b>CONTEXT</b> structure is highly processor specific. Refer to 
      the WinNT.h header file for processor-specific definitions of this structures and any alignment 
      requirements.


## -returns



If the function succeeds, the return value is nonzero.

If the function fails, the return value is zero. To get extended error information, call 
       <a href="https://docs.microsoft.com/windows/desktop/api/errhandlingapi/nf-errhandlingapi-getlasterror">GetLastError</a>.




## -remarks



This function is used to retrieve the thread context of the specified thread. The function retrieves a 
    selective context based on the value of the <b>ContextFlags</b> member of the 
    context structure. The thread identified by the <i>hThread</i> parameter is typically being 
    debugged, but the function can also operate when the thread is not being debugged.

You cannot get a valid context for a running thread. Use the 
    <a href="https://docs.microsoft.com/windows/desktop/api/processthreadsapi/nf-processthreadsapi-suspendthread">SuspendThread</a> function to suspend the thread before 
    calling <b>GetThreadContext</b>.

If you call <b>GetThreadContext</b> for the current 
    thread, the function returns successfully; however, the context returned is not valid.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/winnt/ns-winnt-arm64_nt_context">CONTEXT</a>



<a href="https://docs.microsoft.com/windows/desktop/Debug/debugging-functions">Debugging Functions</a>



<a href="https://docs.microsoft.com/windows/desktop/api/winbase/nf-winbase-getxstatefeaturesmask">GetXStateFeaturesMask</a>



<a href="https://docs.microsoft.com/windows/desktop/api/processthreadsapi/nf-processthreadsapi-setthreadcontext">SetThreadContext</a>



<a href="https://docs.microsoft.com/windows/desktop/api/processthreadsapi/nf-processthreadsapi-suspendthread">SuspendThread</a>



<a href="https://docs.microsoft.com/windows/desktop/api/winbase/nf-winbase-wow64getthreadcontext">Wow64GetThreadContext</a>
 

 

