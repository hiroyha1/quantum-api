---
uid: Microsoft.Quantum.Chemistry.JordanWigner.PrepareSparseMultiConfigurationalState
title: PrepareSparseMultiConfigurationalState operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Chemistry.JordanWigner
qsharp.name: PrepareSparseMultiConfigurationalState
qsharp.summary: >-
  Sparse multi-configurational state preparation of trial state by adding excitations
  to initial trial state.
---

# PrepareSparseMultiConfigurationalState operation

Namespace: [Microsoft.Quantum.Chemistry.JordanWigner](xref:Microsoft.Quantum.Chemistry.JordanWigner)

Package: [Microsoft.Quantum.Chemistry](https://nuget.org/packages/Microsoft.Quantum.Chemistry)


Sparse multi-configurational state preparation of trial state by adding excitationsto initial trial state.

```qsharp
operation PrepareSparseMultiConfigurationalState (initialStatePreparation : (Qubit[] => Unit), excitations : Microsoft.Quantum.Chemistry.JordanWigner.JordanWignerInputState[], qubits : Qubit[]) : Unit
```


## Input

### initialStatePreparation : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[] => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal) 

Unitary to prepare initial trial state.


### excitations : [JordanWignerInputState](xref:Microsoft.Quantum.Chemistry.JordanWigner.JordanWignerInputState)[]

Excitations of initial trial state represented bythe amplitude of the excitation and the qubit indicesthe excitation acts on.


### qubits : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

Qubits of Hamiltonian.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

