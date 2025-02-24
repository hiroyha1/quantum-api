---
uid: Microsoft.Quantum.Canon.ApplyPauliFromBitString
title: ApplyPauliFromBitString operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: ApplyPauliFromBitString
qsharp.summary: >-
  Applies a Pauli operator on each qubit in an array if the corresponding
  bit of a Boolean array matches a given input.
---

# ApplyPauliFromBitString operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Applies a Pauli operator on each qubit in an array if the correspondingbit of a Boolean array matches a given input.

```qsharp
operation ApplyPauliFromBitString (pauli : Pauli, bitApply : Bool, bits : Bool[], qubits : Qubit[]) : Unit is Adj + Ctl
```


## Input

### pauli : [Pauli](xref:microsoft.quantum.qsharp.valueliterals#pauli-literals)

Pauli operator to apply to `qubits[idx]` where `bitsApply == bits[idx]`


### bitApply : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)

apply Pauli if bit is this value


### bits : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)[]

Boolean register specifying which corresponding qubit in `qubits` should be operated on


### qubits : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

Quantum register on which to selectively apply the specified Pauli operator



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Example

The following applies an X operation on qubits 0 and 2, and a Z operation on qubits 1 and 3.```qsharpuse qubits = Qubit[4];let bits = [true, false, true, false];// Apply when index in `bits` is `true`.ApplyPauliFromBitString(PauliX, true, bits, qubits);// Apply when index in `bits` is `false`.ApplyPauliFromBitString(PauliZ, false, bits, qubits);```

## Remarks

The Boolean array and the quantum register must be of equal length.