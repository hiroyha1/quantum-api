---
uid: Microsoft.Quantum.Logical.EqualB
title: EqualB function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Logical
qsharp.name: EqualB
qsharp.summary: Returns true if and only if two inputs are equal.
---

# EqualB function

Namespace: [Microsoft.Quantum.Logical](xref:Microsoft.Quantum.Logical)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Returns true if and only if two inputs are equal.

```qsharp
function EqualB (a : Bool, b : Bool) : Bool
```


## Input

### a : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)

The first value to be compared.


### b : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)

The second value to be compared.



## Output : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)

`true` if and only if `a` is equal to `b`.

## Remarks

The following are equivalent:```qsharplet cond = a == b;let cond = EqualB(a, b);```