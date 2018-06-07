---
title: WM\_NEXTMENU message
description: Sent to an application when the right or left arrow key is used to switch between the menu bar and the system menu.
ms.assetid: 3fa50fd3-47a6-4dae-9ceb-2abb6626e0a6
keywords:
- WM_NEXTMENU message Menus and Other Resources
topic_type:
- apiref
api_name:
- WM_NEXTMENU
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

# WM\_NEXTMENU message

Sent to an application when the right or left arrow key is used to switch between the menu bar and the system menu.


```C++
#define WM_NEXTMENU                     0x0213
```



## Parameters

<dl> <dt>

*wParam* 
</dt> <dd>

The virtual-key code of the key. See [**Virtual-Key Codes**](https://msdn.microsoft.com/library/windows/desktop/dd375731).

</dd> <dt>

*lParam* 
</dt> <dd>

A pointer to a [**MDINEXTMENU**](/windows/desktop/api/Winuser/ns-winuser-tagmdinextmenu) structure that contains information about the menu to be activated.

</dd> </dl>

## Remarks

In responding to this message, the application can specify the menu to switch to in the **hmenuNext** member of [**MDINEXTMENU**](/windows/desktop/api/Winuser/ns-winuser-tagmdinextmenu) and the window to receive the menu notification messages in the **hwndNext** member of the **MDINEXTMENU** structure. You must set both members for the changes to take effect (they are initially **NULL**).

## Requirements



|                                     |                                                                                                          |
|-------------------------------------|----------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                                               |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                                     |
| Header<br/>                   | <dl> <dt>Winuser.h (include Windows.h)</dt> </dl> |



## See also

<dl> <dt>

**Reference**
</dt> <dt>

[**MDINEXTMENU**](/windows/desktop/api/Winuser/ns-winuser-tagmdinextmenu)
</dt> <dt>

**Conceptual**
</dt> <dt>

[Menus](menus.md)
</dt> </dl>

 

 




