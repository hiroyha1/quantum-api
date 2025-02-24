---
uid: Microsoft.Quantum.Intrinsic.Exp
title: Exp operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Intrinsic
qsharp.name: Exp
qsharp.summary: Applies the exponential of a multi-qubit Pauli operator.
---

# Exp operation

Namespace: [Microsoft.Quantum.Intrinsic](xref:Microsoft.Quantum.Intrinsic)

Package: [Microsoft.Quantum.QSharp.Core](https://nuget.org/packages/Microsoft.Quantum.QSharp.Core)


Applies the exponential of a multi-qubit Pauli operator.

```qsharp
operation Exp (paulis : Pauli[], theta : Double, qubits : Qubit[]) : Unit is Adj + Ctl
```


## Description

\begin{align}e^{i \theta [P_0 \otimes P_1 \cdots P_{N-1}]},\end{align}where $P_i$ is the $i$th element of `paulis`, and where$N = $`Length(paulis)`.

## Input

### paulis : [Pauli](xref:microsoft.quantum.qsharp.valueliterals#pauli-literals)[]

Array of single-qubit Pauli values indicating the tensor productfactors on each qubit.


### theta : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

Angle about the given multi-qubit Pauli operator by which thetarget register is to be rotated. Expressed in radians.


### qubits : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

Register to apply the given rotation to.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

