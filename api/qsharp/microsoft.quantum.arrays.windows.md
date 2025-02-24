---
uid: Microsoft.Quantum.Arrays.Windows
title: Windows function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Arrays
qsharp.name: Windows
qsharp.summary: Returns all consecutive subarrays of length `size`.
---

# Windows function

Namespace: [Microsoft.Quantum.Arrays](xref:Microsoft.Quantum.Arrays)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Returns all consecutive subarrays of length `size`.

```qsharp
function Windows<'T> (size : Int, array : 'T[]) : 'T[][]
```


## Description

This function returns all `n - size + 1` subarrays oflength `size` in order, where `n` is the length of `arr`.The first subarrays are `arr[0..size - 1], arr[1..size], arr[2..size + 1]`until the last subarray `arr[n - size..n - 1]`.If `size <= 0` or `size > n`, an empty array is returned.

## Input

### size : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

Length of the subarrays.


### array : 'T[]

An array of elements.



## Output : 'T[][]



## Type Parameters

### 'T

The type of `array` elements.

## Example

```qsharp// same as [[1, 2, 3], [2, 3, 4], [3, 4, 5]]let windows = Windows(3, [1, 2, 3, 4, 5]);```