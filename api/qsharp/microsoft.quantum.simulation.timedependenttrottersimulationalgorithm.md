---
uid: Microsoft.Quantum.Simulation.TimeDependentTrotterSimulationAlgorithm
title: TimeDependentTrotterSimulationAlgorithm function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Simulation
qsharp.name: TimeDependentTrotterSimulationAlgorithm
qsharp.summary: >-
  `TimeDependentSimulationAlgorithm` function that uses a Trotter–Suzuki
  decomposition to approximate a unitary operator that solves the
  time-dependent Schrodinger equation.
---

# TimeDependentTrotterSimulationAlgorithm function

Namespace: [Microsoft.Quantum.Simulation](xref:Microsoft.Quantum.Simulation)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


`TimeDependentSimulationAlgorithm` function that uses a Trotter–Suzukidecomposition to approximate a unitary operator that solves thetime-dependent Schrodinger equation.

```qsharp
function TimeDependentTrotterSimulationAlgorithm (trotterStepSize : Double, trotterOrder : Int) : Microsoft.Quantum.Simulation.TimeDependentSimulationAlgorithm
```


## Input

### trotterStepSize : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

Duration of simulated time-evolution in single Trotter step.


### trotterOrder : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

Order of Trotter integrator. This must be either 1 or an even number.



## Output : [TimeDependentSimulationAlgorithm](xref:Microsoft.Quantum.Simulation.TimeDependentSimulationAlgorithm)

A `TimeDependentSimulationAlgorithm` type.