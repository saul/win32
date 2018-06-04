---
title: IpcfGetSerializedLicenseFromFileStream function
description: Gets the license associated with a file stream.
audience: developer
author: REDMOND\\bruceper
manager: REDMOND\\mbaldwin
ms.assetid: 3F3D35D8-773C-4C5F-99D0-DC63BACD486C
ms.prod: windows-server-dev
ms.technology: active-directory-rights-management
ms.tgt_platform: multiple
keywords:
- IpcfGetSerializedLicenseFromFileStream function Active Directory Rights Management Services SDK 2.0
topic_type:
- apiref
api_name:
- IpcfGetSerializedLicenseFromFileStream
api_location:
- Msipc.dll
api_type:
- DllExport
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# IpcfGetSerializedLicenseFromFileStream function

Gets the license associated with a file stream.

## Syntax


```C++
HRESULT WINAPI IpcfGetSerializedLicenseFromFileStream(
  _In_  ILockBytes  *pInputFileStream,
  _In_  LPCWSTR     wszInputFilePath,
  _Out_ PIPC_BUFFER *ppvLicense
);
```



## Parameters

<dl> <dt>

*pInputFileStream* \[in\]
</dt> <dd>

Pointer to the byte stream from which to get the serialized license.

</dd> <dt>

*wszInputFilePath* \[in\]
</dt> <dd>

The path to the file from which to get the serialized license. The path must include the file name and, if one exists, the file name extension.

This parameter is only used determine the file format, based on the file name extension of the file in the input file stream.

The path is limited to **MAX\_PATH** characters. To extend this limit to 32,767 characters, prepend "\\\\?\\" to the path. For more information, see [Naming Files, Paths, and Namespaces](https://msdn.microsoft.com/library/windows/desktop/aa365247.aspx).

</dd> <dt>

*ppvLicense* \[out\]
</dt> <dd>

A pointer to a variable that receives a pointer to a buffer that holds the license. The buffer is allocated by the File API and must be freed using [**IpcFreeMemory**](ipcfreememory.md).

</dd> </dl>

## Return value

If the function succeeds, the return value is **S\_OK**. If the function fails, it returns an **HRESULT** value that indicates the error.

For more information, see [**Error codes**](error-codes.md) for a description of all RMS SDK 2.1 return values.

## Remarks

For supporting information on using the File API part of RMS SDK 2.1 see, [Supported File Formats](supported-file-formats.md), [File API configuration](file-api-configuration.md) and [Setting the API security](setting-the-api-security-mode--api-mode-.md) mode in the [AD RMS developer notes](developer-notes.md) topic.

## Requirements



|                                     |                                                                                                        |
|-------------------------------------|--------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista with SP2<br/>                                                                      |
| Minimum supported server<br/> | Windows Server 2008<br/>                                                                         |
| Header<br/>                   | <dl> <dt>Ipcfile.h (include Msipc.h)</dt> </dl> |
| Library<br/>                  | <dl> <dt>Msipc.lib</dt> </dl>                   |
| DLL<br/>                      | <dl> <dt>Msipc.dll</dt> </dl>                   |



## See also

<dl> <dt>

[Naming Files, Paths, and Namespaces](https://msdn.microsoft.com/library/windows/desktop/aa365247.aspx)
</dt> <dt>

[**IpcFreeMemory**](ipcfreememory.md)
</dt> <dt>

[Supported File Formats](supported-file-formats.md)
</dt> <dt>

[File API configuration](file-api-configuration.md)
</dt> <dt>

[Setting the API security](setting-the-api-security-mode--api-mode-.md)
</dt> <dt>

[AD RMS developer notes](developer-notes.md)
</dt> <dt>

[**Error codes**](error-codes.md)
</dt> </dl>

 

 




