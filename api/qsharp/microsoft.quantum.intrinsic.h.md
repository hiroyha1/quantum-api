---
uid: Microsoft.Quantum.Intrinsic.H
title: H operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Intrinsic
qsharp.name: H
qsharp.summary: Applies the Hadamard transformation to a single qubit.
---

# H operation

Namespace: [Microsoft.Quantum.Intrinsic](xref:Microsoft.Quantum.Intrinsic)

Package: [Microsoft.Quantum.QSharp.Core](https://nuget.org/packages/Microsoft.Quantum.QSharp.Core)


Applies the Hadamard transformation to a single qubit.

```qsharp
operation H (qubit : Qubit) : Unit is Adj + Ctl
```


## Description

\begin{align}H \mathrel{:=}\frac{1}{\sqrt{2}}\begin{bmatrix}1 & 1 \\\\1 & -1\end{bmatrix}.\end{align}

## Input

### qubit : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Qubit to which the gate should be applied.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

