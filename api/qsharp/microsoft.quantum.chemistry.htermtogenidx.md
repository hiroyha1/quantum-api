---
uid: Microsoft.Quantum.Chemistry.HTermToGenIdx
title: HTermToGenIdx function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Chemistry
qsharp.name: HTermToGenIdx
qsharp.summary: Converts a Hamiltonian term in `HTerm` data format to a GeneratorIndex.
---

# HTermToGenIdx function

Namespace: [Microsoft.Quantum.Chemistry](xref:Microsoft.Quantum.Chemistry)

Package: [Microsoft.Quantum.Chemistry](https://nuget.org/packages/Microsoft.Quantum.Chemistry)


Converts a Hamiltonian term in `HTerm` data format to a GeneratorIndex.

```qsharp
function HTermToGenIdx (term : Microsoft.Quantum.Chemistry.HTerm, termType : Int[]) : Microsoft.Quantum.Simulation.GeneratorIndex
```


## Input

### term : [HTerm](xref:Microsoft.Quantum.Chemistry.HTerm)

Input data in `HTerm` format.


### termType : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)[]

Additional information added to GeneratorIndex.



## Output : [GeneratorIndex](xref:Microsoft.Quantum.Simulation.GeneratorIndex)

A GeneratorIndex representing a Hamiltonian term represented by `term`,together with additional information added by `termType`.