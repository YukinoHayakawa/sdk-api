---
UID: NF:d3d9helper.IDirect3DTexture9.AddDirtyRect
title: IDirect3DTexture9::AddDirtyRect (d3d9helper.h)
description: Adds a dirty region to a texture resource.
old-location: direct3d9\idirect3dtexture9__adddirtyrect.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3dtexture9__adddirtyrect.htm
ms.date: 12/05/2018
ms.keywords: 5056714a-00c4-8318-bc7b-f4fc70438ea2, AddDirtyRect, AddDirtyRect method [Direct3D 9], AddDirtyRect method [Direct3D 9],IDirect3DTexture9 interface, IDirect3DTexture9 interface [Direct3D 9],AddDirtyRect method, IDirect3DTexture9.AddDirtyRect, IDirect3DTexture9::AddDirtyRect, d3d9helper/IDirect3DTexture9::AddDirtyRect, direct3d9.idirect3dtexture9__adddirtyrect
f1_keywords:
- d3d9helper/IDirect3DTexture9.AddDirtyRect
dev_langs:
- c++
req.header: d3d9helper.h
req.include-header: D3D9.h
req.target-type: Windows
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
req.lib: D3D9.lib
req.dll: 
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- D3D9.lib
- D3D9.dll
api_name:
- IDirect3DTexture9.AddDirtyRect
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDirect3DTexture9::AddDirtyRect


## -description


Adds a dirty region to a texture resource.


## -parameters




### -param pDirtyRect [in]

Type: <b>const <a href="/windows/desktop/api/windef/ns-windef-rect">RECT</a>*</b>

Pointer to a <a href="/windows/desktop/api/windef/ns-windef-rect">RECT</a> structure, specifying the dirty region to add. Specifying <b>NULL</b> expands the dirty region to cover the entire texture. 


## -returns



Type: <b><a href="/windows/win32/com/structure-of-com-error-codes">HRESULT</a></b>

If the method succeeds, the return value is D3D_OK. If the method fails, the return value can be D3DERR_INVALIDCALL.




## -remarks



For performance reasons, dirty regions are only recorded for level zero of a texture. For sublevels, it is assumed that the corresponding (scaled) rectangle or box is also dirty. Dirty regions are automatically recorded when <a href="https://docs.microsoft.com/windows/desktop/api/d3d9helper/nf-d3d9helper-idirect3dtexture9-lockrect">IDirect3DTexture9::LockRect</a> is called without <a href="https://docs.microsoft.com/windows/desktop/direct3d9/d3dlock">D3DLOCK_NO_DIRTY_UPDATE</a> or <a href="https://docs.microsoft.com/windows/desktop/direct3d9/d3dlock">D3DLOCK_READONLY</a>. The destination surface of <a href="https://docs.microsoft.com/windows/desktop/api/d3d9/nf-d3d9-idirect3ddevice9-updatesurface">IDirect3DDevice9::UpdateSurface</a> is also marked dirty automatically.

Using <a href="https://docs.microsoft.com/windows/desktop/direct3d9/d3dlock">D3DLOCK_NO_DIRTY_UPDATE</a> and explicitly specifying dirty regions can be used to increase the efficiency of <a href="https://docs.microsoft.com/windows/desktop/api/d3d9/nf-d3d9-idirect3ddevice9-updatetexture">IDirect3DDevice9::UpdateTexture</a>. Using this method, applications can optimize what subset of a resource is copied by specifying dirty regions on the resource. However, the dirty regions may be expanded to optimize alignment.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/d3d9helper/nn-d3d9helper-idirect3dtexture9">IDirect3DTexture9</a>
 

 

