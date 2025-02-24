---
uid: Microsoft.Quantum.Arrays.MappedByIndex
title: MappedByIndex function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Arrays
qsharp.name: MappedByIndex
qsharp.summary: >-
  Given an array and a function that is defined
  for the indexed elements of the array, returns a new array that consists
  of the images of the original array under the function.
---

# MappedByIndex function

Namespace: [Microsoft.Quantum.Arrays](xref:Microsoft.Quantum.Arrays)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Given an array and a function that is definedfor the indexed elements of the array, returns a new array that consistsof the images of the original array under the function.

```qsharp
function MappedByIndex<'T, 'U> (mapper : ((Int, 'T) -> 'U), array : 'T[]) : 'U[]
```


## Input

### mapper : ([Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals),'T) -> 'U

A function from `(Int, 'T)` to `'U` that is used to map elementsand their indices.


### array : 'T[]

An array of elements over `'T`.



## Output : 'U[]

An array `'U[]` of elements that are mapped by the `mapper` function.

## Type Parameters

### 'T

The type of `array` elements.
### 'U

The result type of the `mapper` function.

## Example

The following two lines are equivalent:```qsharplet arr = MapIndex(f, [x0, x1, x2]);```and```qsharplet arr = [f(0, x0), f(1, x1), f(2, x2)];```

## Remarks

The function is defined for generic types, i.e., whenever we havean array `'T[]` and a function `mapper: (Int, 'T) -> 'U` we can map the elementsof the array and produce a new array of type `'U[]`.

## See Also

- [Microsoft.Quantum.Arrays.Mapped](xref:Microsoft.Quantum.Arrays.Mapped)