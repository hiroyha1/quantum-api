---
uid: Microsoft.Quantum.Arithmetic.MeasureInteger
title: MeasureInteger operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Arithmetic
qsharp.name: MeasureInteger
qsharp.summary: >-
  Measures the content of a quantum register and converts
  it to an integer. The measurement is performed with respect
  to the standard computational basis, i.e., the eigenbasis of `PauliZ`.
---

# MeasureInteger operation

Namespace: [Microsoft.Quantum.Arithmetic](xref:Microsoft.Quantum.Arithmetic)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Measures the content of a quantum register and convertsit to an integer. The measurement is performed with respectto the standard computational basis, i.e., the eigenbasis of `PauliZ`.

```qsharp
operation MeasureInteger (target : Microsoft.Quantum.Arithmetic.LittleEndian) : Int
```


## Input

### target : [LittleEndian](xref:Microsoft.Quantum.Arithmetic.LittleEndian)

A quantum register in the little-endian encoding.



## Output : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

An unsigned integer that contains the measured value of `target`.

## Remarks

This operation resets its input register to the $\ket{00\cdots 0}$ state,suitable for releasing back to a target machine.