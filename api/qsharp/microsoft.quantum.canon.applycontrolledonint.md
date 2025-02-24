---
uid: Microsoft.Quantum.Canon.ApplyControlledOnInt
title: ApplyControlledOnInt operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: ApplyControlledOnInt
qsharp.summary: >-
  Applies a unitary operation on the target register if the control
  register state corresponds to a specified nonnegative integer.
---

# ApplyControlledOnInt operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Applies a unitary operation on the target register if the controlregister state corresponds to a specified nonnegative integer.

```qsharp
operation ApplyControlledOnInt<'T> (numberState : Int, oracle : ('T => Unit is Adj + Ctl), controlRegister : Qubit[], targetRegister : 'T) : Unit is Adj + Ctl
```


## Input

### numberState : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

A nonnegative integer on which the operation `oracle` should becontrolled.


### oracle : 'T => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj + Ctl

A unitary operation to be controlled.


### controlRegister : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)[]

A quantum register that controls application of `oracle`.


### targetRegister : 'T

A register on which to apply `oracle`.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Type Parameters

### 'T



## Remarks

The value of `numberState` is interpreted using a little-endian encoding.`numberState` must be at most $2^\texttt{Length(controlRegister)} - 1$.For example, `numberState = 537` means that `oracle`is applied if and only if `controlRegister` is in the state $\ket{537}$.