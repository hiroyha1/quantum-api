---
uid: Microsoft.Quantum.Arithmetic.PrepareFxP
title: PrepareFxP operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Arithmetic
qsharp.name: PrepareFxP
qsharp.summary: Initialize a quantum fixed-point number to a classical constant.
---

# PrepareFxP operation

Namespace: [Microsoft.Quantum.Arithmetic](xref:Microsoft.Quantum.Arithmetic)

Package: [Microsoft.Quantum.Numerics](https://nuget.org/packages/Microsoft.Quantum.Numerics)


Initialize a quantum fixed-point number to a classical constant.

```qsharp
operation PrepareFxP (constant : Double, fp : Microsoft.Quantum.Arithmetic.FixedPoint) : Unit is Adj + Ctl
```


## Input

### constant : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

Constant to which to initialize the quantum fixed-point number.


### fp : [FixedPoint](xref:Microsoft.Quantum.Arithmetic.FixedPoint)

Fixed-point number (of type FixedPoint) to initialize.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

