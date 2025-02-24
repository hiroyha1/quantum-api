---
uid: Microsoft.Quantum.Simulation.EvolutionGenerator
title: EvolutionGenerator user defined type
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: udt
qsharp.namespace: Microsoft.Quantum.Simulation
qsharp.name: EvolutionGenerator
qsharp.summary: >-
  Represents a dynamical generator as a set of simulatable gates and
  an expansion in terms of that basis.

  Last parameter for number of terms.
---

# EvolutionGenerator user defined type

Namespace: [Microsoft.Quantum.Simulation](xref:Microsoft.Quantum.Simulation)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Represents a dynamical generator as a set of simulatable gates andan expansion in terms of that basis.Last parameter for number of terms.

```qsharp

newtype EvolutionGenerator = (Microsoft.Quantum.Simulation.EvolutionSet, Microsoft.Quantum.Simulation.GeneratorSystem);
```

