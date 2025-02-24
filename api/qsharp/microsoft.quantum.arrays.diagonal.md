---
uid: Microsoft.Quantum.Arrays.Diagonal
title: Diagonal function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Arrays
qsharp.name: Diagonal
qsharp.summary: Returns an array of diagonal elements of a 2-dimensional array
---

# Diagonal function

Namespace: [Microsoft.Quantum.Arrays](xref:Microsoft.Quantum.Arrays)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Returns an array of diagonal elements of a 2-dimensional array

```qsharp
function Diagonal<'T> (matrix : 'T[][]) : 'T[]
```


## Description

If the 2-dimensional array has not a square shape, the diagonal overthe minimum over the number of rows and columns will be returned.

## Input

### matrix : 'T[][]

2-dimensional matrix in row-wise order



## Output : 'T[]



## Type Parameters

### 'T

The type of each element of `matrix`.

## Example

```qsharplet matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]];let diagonal = Diagonal(matrix);// same as: column = [1, 5, 9]```

## See Also

- [Microsoft.Quantum.Arrays.Transposed](xref:Microsoft.Quantum.Arrays.Transposed)