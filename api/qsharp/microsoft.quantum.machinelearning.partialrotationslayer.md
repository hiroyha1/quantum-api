---
uid: Microsoft.Quantum.MachineLearning.PartialRotationsLayer
title: PartialRotationsLayer function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.MachineLearning
qsharp.name: PartialRotationsLayer
qsharp.summary: >-
  Returns an array of single-qubit rotations along a given
  axis, parameterized by distinct model parameters.
---

# PartialRotationsLayer function

Namespace: [Microsoft.Quantum.MachineLearning](xref:Microsoft.Quantum.MachineLearning)

Package: [Microsoft.Quantum.MachineLearning](https://nuget.org/packages/Microsoft.Quantum.MachineLearning)


Returns an array of single-qubit rotations along a givenaxis, parameterized by distinct model parameters.

```qsharp
function PartialRotationsLayer (idxsQubits : Int[], axis : Pauli) : Microsoft.Quantum.MachineLearning.ControlledRotation[]
```


## Input

### idxsQubits : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)[]

Indices for the qubits to be used as the targets for each rotation.


### axis : [Pauli](xref:microsoft.quantum.qsharp.valueliterals#pauli-literals)

The rotation axis for each rotation in the given layer.



## Output : [ControlledRotation](xref:Microsoft.Quantum.MachineLearning.ControlledRotation)[]

An array of controlled rotations about the given axis, one on each of`nQubits` qubits.