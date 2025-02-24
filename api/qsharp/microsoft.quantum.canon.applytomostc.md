---
uid: Microsoft.Quantum.Canon.ApplyToMostC
title: ApplyToMostC operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: ApplyToMostC
qsharp.summary: Applies an operation to all but the last element of an array.
---

# ApplyToMostC operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Applies an operation to all but the last element of an array.

```qsharp
operation ApplyToMostC<'T> (op : ('T[] => Unit is Ctl), targets : 'T[]) : Unit is Ctl
```


## Description

Given an operation `op` and an array of targets `targets`,applies `op(Most(targets))`.

## Input

### op : 'T[] => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Ctl

An operation to be applied.


### targets : 'T[]

An array of targets, of which all but the last will be applied to `op`.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Type Parameters

### 'T

The input type of the operation to be applied.

## See Also

- [Microsoft.Quantum.Canon.ApplyToMost](xref:Microsoft.Quantum.Canon.ApplyToMost)
- [Microsoft.Quantum.Canon.ApplyToMostA](xref:Microsoft.Quantum.Canon.ApplyToMostA)
- [Microsoft.Quantum.Canon.ApplyToMostCA](xref:Microsoft.Quantum.Canon.ApplyToMostCA)