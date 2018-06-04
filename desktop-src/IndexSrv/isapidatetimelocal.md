---
Description: IsapiDateTimeLocal
ms.assetid: 084713d0-38bb-4b72-95c3-a775facddb55
title: IsapiDateTimeLocal
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IsapiDateTimeLocal

> [!Note]  
> Indexing Service is no longer supported as of Windows XP and is unavailable for use as of Windows 8. Instead, use [Windows Search](https://msdn.microsoft.com/windows/desktop/6da601c6-3742-40ad-99f2-8817f7f642b3) for client side search and [Microsoft Search Server Express]( http://go.microsoft.com/fwlink/p/?linkid=258445) for server side search.

 

The **IsapiDateTimeLocal** entry specifies the time zone to use when formatting the date and time for ISAPI queries.

### Summary



|          |                |
|----------|----------------|
| Type:    | **REG\_DWORD** |
| Default: | 0              |
| Range:   | 0 - 1          |



 

### Remarks

The value of the **IsapiDateTimeLocal** entry can be one of the following values.



| Value | Formatting                                                                                                                |
|-------|---------------------------------------------------------------------------------------------------------------------------|
| 0     | Display the date and time as Coordinated Universal Time (UTC). This is the default behavior for Index Server 1.x and 2.0. |
| 1     | Display the date and time in the local time zone of the system that processes the query.                                  |



 

The value of an identically named entry under the [**Catalog**](catalog--property--and-scope-registry-entries.md) subkey for a specific catalog cannot override the value of this entry.

## Related topics

<dl> <dt>

[IsapiDateTimeFormatting](isapidatetimeformatting.md)
</dt> <dt>

[Main Registry Entries](main-registry-entries.md)
</dt> </dl>

 

 


