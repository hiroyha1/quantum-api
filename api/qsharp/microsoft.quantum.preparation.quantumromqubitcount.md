---
uid: Microsoft.Quantum.Preparation.QuantumROMQubitCount
title: QuantumROMQubitCount function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Preparation
qsharp.name: QuantumROMQubitCount
qsharp.summary: >-
  > [!WARNING]

  > QuantumROMQubitCount has been deprecated. Please use <xref:Microsoft.Quantum.Preparation.PurifiedMixedStateRequirements> instead.


  Returns the total number of qubits that must be allocated
  to the operation returned by `QuantumROM`.
---

# QuantumROMQubitCount function

Namespace: [Microsoft.Quantum.Preparation](xref:Microsoft.Quantum.Preparation)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


> [!WARNING]
> QuantumROMQubitCount has been deprecated. Please use <xref:Microsoft.Quantum.Preparation.PurifiedMixedStateRequirements> instead.

Returns the total number of qubits that must be allocatedto the operation returned by `QuantumROM`.

```qsharp
function QuantumROMQubitCount (targetError : Double, nCoeffs : Int) : (Int, (Int, Int))
```


## Input

### targetError : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

The target error $\epsilon$.


### nCoeffs : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

Number of coefficients specified in `QuantumROM`.



## Output : ([Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals),([Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals),[Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)))

## First parameterA tuple `(x,(y,z))` where `x = y + z` is the total number of qubits allocated,`y` is the number of qubits for the `LittleEndian` register, and `z` is the Numberof garbage qubits.