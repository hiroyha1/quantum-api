---
uid: Microsoft.Quantum.Bitwise.RightShiftedI
title: RightShiftedI function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Bitwise
qsharp.name: RightShiftedI
qsharp.summary: >-
  Shifts the bitwise representation of a number right by a given number of
  bits.
---

# RightShiftedI function

Namespace: [Microsoft.Quantum.Bitwise](xref:Microsoft.Quantum.Bitwise)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Shifts the bitwise representation of a number right by a given number ofbits.

```qsharp
function RightShiftedI (value : Int, amount : Int) : Int
```


## Input

### value : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The number whose bitwise representation is to be shifted to the right(less significant).


### amount : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The number of bits by which `value` is to be shifted to the right.



## Output : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The value of `value`, shifted right by `amount` bits.

## Remarks

The following are equivalent:```qsharplet c = a >>> b;let c = RightShiftedI(a, b);```