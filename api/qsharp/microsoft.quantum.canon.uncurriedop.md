---
uid: Microsoft.Quantum.Canon.UncurriedOp
title: UncurriedOp function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: UncurriedOp
qsharp.summary: >-
  Given a function which returns operations,
  returns a new operation which takes both inputs
  as a tuple.
---

# UncurriedOp function

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Given a function which returns operations,returns a new operation which takes both inputsas a tuple.

```qsharp
function UncurriedOp<'T, 'U> (curriedOp : ('T -> ('U => Unit))) : (('T, 'U) => Unit)
```


## Input

### curriedOp : 'T -> 'U => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal) 

A function which returns operations.



## Output : ('T,'U) => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal) 

A new operation `op` such that `op(t, u)` is equivalentto `(curriedOp(t))(u)`.

## Type Parameters

### 'T

The type of the first input to a curried operation.
### 'U

The type of the second input to a curried operation.

## See Also

- [Microsoft.Quantum.Canon.UncurriedOpC](xref:Microsoft.Quantum.Canon.UncurriedOpC)
- [Microsoft.Quantum.Canon.UncurriedOpA](xref:Microsoft.Quantum.Canon.UncurriedOpA)
- [Microsoft.Quantum.Canon.UncurriedOpCA](xref:Microsoft.Quantum.Canon.UncurriedOpCA)