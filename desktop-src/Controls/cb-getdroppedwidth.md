---
title: CB\_GETDROPPEDWIDTH message
description: Gets the minimum allowable width, in pixels, of the list box of a combo box with the CBS\_DROPDOWN or CBS\_DROPDOWNLIST style.
ms.assetid: d7f37a6c-a623-4b15-8ef7-4b64d85c15fa
keywords:
- CB_GETDROPPEDWIDTH message Windows Controls
topic_type:
- apiref
api_name:
- CB_GETDROPPEDWIDTH
api_location:
- Winuser.h
api_type:
- HeaderDef
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# CB\_GETDROPPEDWIDTH message

Gets the minimum allowable width, in pixels, of the list box of a combo box with the [**CBS\_DROPDOWN**](https://www.bing.com/search?q=**CBS\_DROPDOWN**) or [**CBS\_DROPDOWNLIST**](https://www.bing.com/search?q=**CBS\_DROPDOWNLIST**) style.

## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>

Not used; must be zero.

</dd> <dt>

*lParam* 
</dt> <dd>

Not used; must be zero.

</dd> </dl>

## Return value

If the message succeeds, the return value is the width, in pixels.

If the message fails, the return value is CB\_ERR.

## Remarks

By default, the minimum allowable width of the drop-down list box is zero. The width of the list box is either the minimum allowable width or the combo box width, whichever is larger.

## Requirements



|                                     |                                                                                                          |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                                           |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                                     |
| Header<br/>                   | <dl> <dt>Winuser.h (include Windows.h)</dt> </dl> |



## See also

<dl> <dt>

[**CB\_SETDROPPEDWIDTH**](cb-setdroppedwidth.md)
</dt> </dl>

 

 




