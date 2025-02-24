---
uid: Microsoft.Quantum.MachineLearning.ControlledRotation
title: ControlledRotation user defined type
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: udt
qsharp.namespace: Microsoft.Quantum.MachineLearning
qsharp.name: ControlledRotation
qsharp.summary: >-
  Describes a controlled rotation in terms of its target and control
  indices, rotation axis, and index into a model parameter vector.
---

# ControlledRotation user defined type

Namespace: [Microsoft.Quantum.MachineLearning](xref:Microsoft.Quantum.MachineLearning)

Package: [Microsoft.Quantum.MachineLearning](https://nuget.org/packages/Microsoft.Quantum.MachineLearning)


Describes a controlled rotation in terms of its target and controlindices, rotation axis, and index into a model parameter vector.

```qsharp

newtype ControlledRotation = ((TargetIndex : Int, ControlIndices : Int[]), Axis : Pauli, ParameterIndex : Int);
```



## Named Items

### TargetIndex : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

Index of the target qubit for this controlled rotation.
### ControlIndices : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)[]

An array of the control qubit indices for this rotation.
### Axis : [Pauli](xref:microsoft.quantum.qsharp.valueliterals#pauli-literals)

The axis for this rotation.
### ParameterIndex : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

An index into a model parameter vector describing the anglefor this rotation.

## Example

The following represents a rotation about the $X$-axis of the firstqubit in a register, controlled on the second qubit, and with anangle given by the fourth parameter in a sequential model:```qsharplet controlledRotation = ControlledRotation(    (0, [1]),    PauliX,    3)```

## Remarks

An uncontrolled rotation can be represented by setting `ControlIndices`to an empty array of indexes, `new Int[0]`.