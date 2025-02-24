---
uid: Microsoft.Quantum.Synthesis.ApplyXControlledOnTruthTable
title: ApplyXControlledOnTruthTable operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Synthesis
qsharp.name: ApplyXControlledOnTruthTable
qsharp.summary: >-
  Applies the @"Microsoft.Quantum.Intrinsic.X" operation on `target`, if the Boolean function `func` evaluates
  to true for the classical assignment in `controlRegister`.
---

# ApplyXControlledOnTruthTable operation

Namespace: [Microsoft.Quantum.Synthesis](xref:Microsoft.Quantum.Synthesis)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Applies the @"Microsoft.Quantum.Intrinsic.X" operation on `target`, if the Boolean function `func` evaluatesto true for the classical assignment in `controlRegister`.

```qsharp
operation ApplyXControlledOnTruthTable (func : BigInt, controlRegister : Qubit[], target : Qubit) : Unit is Adj + Ctl
```


## Description

The operation implements the unitary operation\begin{align}U\ket{x}\ket{y} = \ket{x}\ket{y \oplus f(x)}\end{align}where $x$ and $y$ represent `controlRegister` and `target`, respectively.The Boolean function $f$ is represented as a truth table in terms of a big integer.For example, the majority function on three inputs is represented by the bitstring`11101000`, where the most significant bit `1` corresponds to the input assignment `(1, 1, 1)`,and the least significant bit `0` corresponds to the input assignment `(0, 0, 0)`.It can be represented by the big integer `0xE8L` in hexadecimal notation or as `232L`in decimal notation.  The `L` suffix indicates that the constant is of type `BigInt`.More details on this representation can also be found in the [truth tables kata](https://github.com/microsoft/QuantumKatas/tree/main/TruthTables).The implementation makes use of @"Microsoft.Quantum.Intrinsic.CNOT"and @"Microsoft.Quantum.Intrinsic.R1" gates.

## Input

### func : [BigInt](xref:microsoft.quantum.qsharp.valueliterals#bigint-literals)

Boolean truth table represented as big integer


### controlRegister : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

Register of control qubits


### target : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Target qubit



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## References

- [*N. Schuch*, *J. Siewert*, PRL 91, no. 027902, 2003, arXiv:quant-ph/0303063](https://arxiv.org/abs/quant-ph/0303063)- [*Mathias Soeken*, *Martin Roetteler*, arXiv:2005.12310](https://arxiv.org/abs/2005.12310)

## See Also

- [Microsoft.Quantum.Synthesis.ApplyXControlledOnTruthTableWithCleanTarget](xref:Microsoft.Quantum.Synthesis.ApplyXControlledOnTruthTableWithCleanTarget)