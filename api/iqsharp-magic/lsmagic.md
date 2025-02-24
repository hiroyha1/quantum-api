---
title: '%lsmagic (magic command)'
description: Returns a list of all currently available magic commands.
author: anjbur
uid: microsoft.quantum.iqsharp.magic-ref.lsmagic
ms.author: anburton
ms.date: 12/05/2022
ms.topic: managed-reference
---

<!--
    NB: This file has been automatically generated from Microsoft.Quantum.IQSharp.Jupyter.dll,
        please do not manually edit it.

    [DEBUG] JSON source:
        {"Name": "%lsmagic", "Documentation": {"Summary": "Returns a list of all currently available magic commands.", "Full": null, "Description": "\r\nThis magic command lists all of the magic commands available in the IQ# kernel,\r\nas well as those defined in any packages that have been loaded in the current\r\nsession via the [`%package` magic command](https://docs.microsoft.com/qsharp/api/iqsharp-magic/package).\r\n                ", "Remarks": null, "Examples": ["\r\nDisplay the list of available magic commands:\r\n```\r\nIn []: %lsmagic\r\nOut[]: <detailed list of all available magic commands>\r\n```\r\n                    "], "SeeAlso": null}, "AssemblyName": "Microsoft.Quantum.IQSharp.Jupyter"}
-->

# `%lsmagic`

## Summary

Returns a list of all currently available magic commands.

## Description

This magic command lists all of the magic commands available in the IQ# kernel,
as well as those defined in any packages that have been loaded in the current
session via the [`%package` magic command](https://docs.microsoft.com/qsharp/api/iqsharp-magic/package).

## Examples for `%lsmagic`

### Example 1

Display the list of available magic commands:
```
In []: %lsmagic
Out[]: <detailed list of all available magic commands>
```
