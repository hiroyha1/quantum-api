---
uid: Microsoft.Quantum.ErrorCorrection.RecoverCSS
title: RecoverCSS operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.ErrorCorrection
qsharp.name: RecoverCSS
qsharp.summary: >-
  Performs a single round of error correction by a quantum code
  described by a `CSS` type.
---

# RecoverCSS operation

Namespace: [Microsoft.Quantum.ErrorCorrection](xref:Microsoft.Quantum.ErrorCorrection)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Performs a single round of error correction by a quantum codedescribed by a `CSS` type.

```qsharp
operation RecoverCSS (code : Microsoft.Quantum.ErrorCorrection.CSS, fnX : Microsoft.Quantum.ErrorCorrection.RecoveryFn, fnZ : Microsoft.Quantum.ErrorCorrection.RecoveryFn, logicalRegister : Microsoft.Quantum.ErrorCorrection.LogicalRegister) : Unit
```


## Input

### code : [CSS](xref:Microsoft.Quantum.ErrorCorrection.CSS)

A quantum CSS error-correcting code packaged as a `CSS` type describesthe encoding and decoding of quantum data, and how error syndromesare to be measured.


### fnX : [RecoveryFn](xref:Microsoft.Quantum.ErrorCorrection.RecoveryFn)

A `RecoveryFn` that maps each $X$ error syndrome to the `Pauli[]` operationsthat correct the detected error.


### fnZ : [RecoveryFn](xref:Microsoft.Quantum.ErrorCorrection.RecoveryFn)

A `RecoveryFn` that maps each $Z$ error syndrome to the `Pauli[]` operationsthat correct the detected error.


### logicalRegister : [LogicalRegister](xref:Microsoft.Quantum.ErrorCorrection.LogicalRegister)

An array of qubits where the stabilizer code is defined.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## See Also

- [Microsoft.Quantum.ErrorCorrection.CSS](xref:Microsoft.Quantum.ErrorCorrection.CSS)
- [Microsoft.Quantum.ErrorCorrection.RecoveryFn](xref:Microsoft.Quantum.ErrorCorrection.RecoveryFn)
- [Microsoft.Quantum.ErrorCorrection.LogicalRegister](xref:Microsoft.Quantum.ErrorCorrection.LogicalRegister)