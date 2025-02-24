---
uid: Microsoft.Quantum.Canon.ApplyToRest
title: ApplyToRest operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: ApplyToRest
qsharp.summary: Applies an operation to all but the first element of an array.
---

# ApplyToRest operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Applies an operation to all but the first element of an array.

```qsharp
operation ApplyToRest<'T> (op : ('T[] => Unit), targets : 'T[]) : Unit
```


## Description

Given an operation `op` and an array of targets `targets`,applies `op(Rest(targets))`.

## Input

### op : 'T[] => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal) 

An operation to be applied.


### targets : 'T[]

An array of targets, of which all but the first will be applied to `op`.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Type Parameters

### 'T

The input type of the operation to be applied.

## Example

The following Q# snippets are equivalent:```qsharpApplyToRest(ApplyCNOTChain, register);ApplyCNOTChain(Rest(register));```

## See Also

- [Microsoft.Quantum.Canon.ApplyToRestA](xref:Microsoft.Quantum.Canon.ApplyToRestA)
- [Microsoft.Quantum.Canon.ApplyToRestC](xref:Microsoft.Quantum.Canon.ApplyToRestC)
- [Microsoft.Quantum.Canon.ApplyToRestCA](xref:Microsoft.Quantum.Canon.ApplyToRestCA)