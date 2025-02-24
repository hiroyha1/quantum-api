---
uid: Microsoft.Quantum.Preparation.PrepareEntangledState
title: PrepareEntangledState operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Preparation
qsharp.name: PrepareEntangledState
qsharp.summary: >-
  Pairwise entangles two qubit registers.

  That is, given two registers, prepares the maximally entangled state
  $\frac{1}{\sqrt{2}} \left(\ket{00} + \ket{11} \right)$ between each pair of qubits on the respective registers,
  assuming that each register starts in the $\ket{0\cdots 0}$ state.
---

# PrepareEntangledState operation

Namespace: [Microsoft.Quantum.Preparation](xref:Microsoft.Quantum.Preparation)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Pairwise entangles two qubit registers.That is, given two registers, prepares the maximally entangled state$\frac{1}{\sqrt{2}} \left(\ket{00} + \ket{11} \right)$ between each pair of qubits on the respective registers,assuming that each register starts in the $\ket{0\cdots 0}$ state.

```qsharp
operation PrepareEntangledState (left : Qubit[], right : Qubit[]) : Unit is Adj + Ctl
```


## Input

### left : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

A qubit array in the $\ket{0\cdots 0}$ state


### right : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

A qubit array in the $\ket{0\cdots 0}$ state



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

