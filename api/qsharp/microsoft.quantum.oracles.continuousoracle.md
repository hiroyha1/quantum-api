---
uid: Microsoft.Quantum.Oracles.ContinuousOracle
title: ContinuousOracle user defined type
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: udt
qsharp.namespace: Microsoft.Quantum.Oracles
qsharp.name: ContinuousOracle
qsharp.summary: Represents a continuous-time oracle.
---

# ContinuousOracle user defined type

Namespace: [Microsoft.Quantum.Oracles](xref:Microsoft.Quantum.Oracles)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Represents a continuous-time oracle.

```qsharp

newtype ContinuousOracle = (((Double, Qubit[]) => Unit is Adj + Ctl));
```



## Description

This is an oracle that implements$U(\delta t) : \ket{\psi(t)} \mapsto \ket{\psi(t + \delta t)}$for all times $t$, where $U$ is a fixed operation, and where$\delta t$ is a non-negative real number.