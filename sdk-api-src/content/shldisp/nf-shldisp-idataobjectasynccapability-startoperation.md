---
UID: NF:shldisp.IDataObjectAsyncCapability.StartOperation
title: IDataObjectAsyncCapability::StartOperation (shldisp.h)
description: Called by a drop target to indicate that asynchronous data extraction is starting.
old-location: shell\IDataObjectAsyncCapability_StartOperation.htm
tech.root: shell
ms.assetid: 84C1E709-ADFD-4c00-B767-C0DB4C30578A
ms.date: 12/05/2018
ms.keywords: IDataObjectAsyncCapability interface [Windows Shell],StartOperation method, IDataObjectAsyncCapability.StartOperation, IDataObjectAsyncCapability::StartOperation, StartOperation, StartOperation method [Windows Shell], StartOperation method [Windows Shell],IDataObjectAsyncCapability interface, shell.IDataObjectAsyncCapability_StartOperation, shldisp/IDataObjectAsyncCapability::StartOperation
f1_keywords:
- shldisp/IDataObjectAsyncCapability.StartOperation
dev_langs:
- c++
req.header: shldisp.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows 8 [desktop apps only]
req.target-min-winversvr: Windows Server 2012 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Shldisp.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: Shell32.dll (version 6.0 or later)
req.irql: 
topic_type:
- APIRef
- kbSyntax
api_type:
- COM
api_location:
- Shell32.dll
api_name:
- IDataObjectAsyncCapability.StartOperation
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
---

# IDataObjectAsyncCapability::StartOperation


## -description


Called by a drop target to indicate that asynchronous data extraction is starting.


## -parameters




### -param pbcReserved [in, optional]

Type: <b><a href="https://docs.microsoft.com/windows/desktop/api/objidl/nn-objidl-ibindctx">IBindCtx</a>*</b>

Reserved. Set this value to <b>nullptr</b>.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -remarks



The drop target calls this method to notify the data object that asynchronous data extraction is starting. The method should store this information so that it can be returned by <a href="https://docs.microsoft.com/windows/desktop/api/shldisp/nf-shldisp-idataobjectasynccapability-inoperation">IDataObjectAsyncCapability::InOperation</a>. Once <b>StartOperation</b> has been called, the drop target returns the <a href="https://docs.microsoft.com/windows/desktop/api/oleidl/nf-oleidl-idroptarget-drop">IDropTarget::Drop</a> call as it would for normal synchronous data extraction.




## -see-also




<a href="https://docs.microsoft.com/windows/desktop/api/shldisp/nn-shldisp-idataobjectasynccapability">IDataObjectAsyncCapability</a>
 

 

