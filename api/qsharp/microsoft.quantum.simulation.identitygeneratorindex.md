---
uid: Microsoft.Quantum.Simulation.IdentityGeneratorIndex
title: IdentityGeneratorIndex function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Simulation
qsharp.name: IdentityGeneratorIndex
qsharp.summary: >-
  Returns a generator index consistent with the zero
  Hamiltonian, `H = 0`, which corresponds to the identity evolution operation.
---

# IdentityGeneratorIndex function

Namespace: [Microsoft.Quantum.Simulation](xref:Microsoft.Quantum.Simulation)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Returns a generator index consistent with the zeroHamiltonian, `H = 0`, which corresponds to the identity evolution operation.

```qsharp
function IdentityGeneratorIndex (idxTerm : Int) : Microsoft.Quantum.Simulation.GeneratorIndex
```


## Input

### idxTerm : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

This input is ignored, and is defined for consistency with the<xref:Microsoft.Quantum.Simulation.GeneratorSystem> user-defined type.



## Output : [GeneratorIndex](xref:Microsoft.Quantum.Simulation.GeneratorIndex)

A generator index representing evolution under the Hamiltonian$H = 0$.