---
title: HH\_HELP\_FINDER command
description: HH\_HELP\_FINDER command
ms.assetid: 0D0E66EF-4239-4009-B1DE-4C6B51918D0B
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# HH\_HELP\_FINDER command

Opens a help topic in a specified help window. This is the WinHelp equivalent of **HH\_DISPLAY\_TOPIC**.

If a window type is not specified, a default window type is used. If the window type or default window type is open, the help topic replaces the current topic in the window.



| *pszFile*                                                                                                                                                                                                            | *dwData*                                                            |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------|
| Specifies a compiled help (.chm) file, or a specific topic within a compiled help file. To specify a defined window type, insert a greater-than (&gt;) character followed by the name of the window type.<br/> | Specifies NULL or a pointer to a topic within a compiled help file. |



 

## Example


```
HWND hwnd =
   HtmlHelp(
             GetDesktopWindow(),
             "c:\\help.chm::/intro.htm>;mainwin",
             HH_HELP_FINDER,
             NULL) ;
```



## Return Value

The handle (hwnd) of the help window.

## Remarks

-   For backward compatibility with **WinHelp()**, **HH\_DISPLAY\_TOPIC** and **HH\_HELP\_FINDER** provide the same functionality.
-   A default help window contains only the Topic pane and is not a three-pane Help Viewer.

## Related topics

<dl> <dt>

[About Commands](about-commands.md)
</dt> <dt>

[HH\_HELP\_CONTEXT](hh-help-context-command.md)
</dt> </dl>

 

 




