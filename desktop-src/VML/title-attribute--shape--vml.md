---
title: Title Attribute (Shape)(VML)
description: Title Attribute (Shape)(VML)
ms.assetid: 08680706-5274-46d4-9199-4fdbf32f884b
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Title Attribute (Shape)(VML)

This topic describes VML, a feature that is deprecated as of Windows Internet Explorer 9. Webpages and applications that rely on VML should be [migrated to SVG](http://go.microsoft.com/fwlink/p/?LinkID=236964) or other widely supported standards.

> [!Note]  
> As of December 2011, this topic has been archived. As a result, it is no longer actively maintained. For more information, see [Archived Content](https://msdn.microsoft.com/library/hh772377). For information, recommendations, and guidance regarding the current version of Windows Internet Explorer, see [Internet Explorer Developer Center](http://go.microsoft.com/fwlink/p/?linkid=204313).

 

Defines the text displayed when the mouse pointer moves over the shape. Read/write. **String**.

**Applies To**

[Shape](shape-element--vml.md)

**Tag Syntax**

&lt;v: *element* title=" *expression* "&gt;

**Script Syntax**

*element* .title="*expression*"

*expression*=*element*.title

**Remarks**

The **Title** attribute is similar to the standard HTML **Title** attribute. The behavior of a title is similar to a Microsoft Windows ToolTip.

**VML Standard Attribute**

**Example**

The title of the shape is "ToolTip display" and will appear when the mouse pointer moves over the shape.


```HTML
   <v:rect id=myrect fillcolor="red" title="ToolTip display"
   style="position:relative;top:1;left:1;width:20;height:20">
   </v:rect>
```



[Title Attribute Example](http://samples.msdn.microsoft.com/workshop/samples/vml/shape/examples/x_title.md). (Requires Microsoft Internet Explorer 5 or greater.)

 

 



