---
uid: Microsoft.Quantum.Canon.ApplyWithA
title: ApplyWithA operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: ApplyWithA
qsharp.summary: Given two operations, applies one as conjugated with the other.
---

# ApplyWithA operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Given two operations, applies one as conjugated with the other.

```qsharp
operation ApplyWithA<'T> (outerOperation : ('T => Unit is Adj), innerOperation : ('T => Unit is Adj), target : 'T) : Unit is Adj
```


## Description

Given two operations, respectively described by unitary operators $U$and $V$, applies them in the sequence $U^{\dagger} V U$. That is,this operation implements the unitary operator given by $V$ conjugatedwith $U$.

## Input

### outerOperation : 'T => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj

The operation $U$ that should be used to conjugate $V$. Note that theouter operation $U$ needs to be adjointable, but does notneed to be controllable.


### innerOperation : 'T => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj

The operation $V$ being conjugated.


### target : 'T

The input to be provided to the outer and inner operations.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Type Parameters

### 'T

The target on which each of the inner and outer operations act.

## Remarks

The outer operation is always assumed to be adjointable, but does notneed to be controllable in order for the combined operation to becontrollable.

## See Also

- [Microsoft.Quantum.Canon.ApplyWith](xref:Microsoft.Quantum.Canon.ApplyWith)
- [Microsoft.Quantum.Canon.ApplyWithC](xref:Microsoft.Quantum.Canon.ApplyWithC)
- [Microsoft.Quantum.Canon.ApplyWithCA](xref:Microsoft.Quantum.Canon.ApplyWithCA)