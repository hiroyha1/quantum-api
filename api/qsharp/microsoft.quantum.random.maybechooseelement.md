---
uid: Microsoft.Quantum.Random.MaybeChooseElement
title: MaybeChooseElement operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Random
qsharp.name: MaybeChooseElement
qsharp.summary: >-
  Given an array of data and an a distribution over its indices,
  attempts to choose an element at random.
---

# MaybeChooseElement operation

Namespace: [Microsoft.Quantum.Random](xref:Microsoft.Quantum.Random)

Package: [Microsoft.Quantum.QSharp.Foundation](https://nuget.org/packages/Microsoft.Quantum.QSharp.Foundation)


Given an array of data and an a distribution over its indices,attempts to choose an element at random.

```qsharp
operation MaybeChooseElement<'T> (data : 'T[], indexDistribution : Microsoft.Quantum.Random.DiscreteDistribution) : (Bool, 'T)
```


## Input

### data : 'T[]

The array from which an element should be chosen.


### indexDistribution : [DiscreteDistribution](xref:Microsoft.Quantum.Random.DiscreteDistribution)

A distribution over the indices of `data`.



## Output : ([Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals),'T)



## Type Parameters

### 'T



## Example

The following Q# snippet chooses an element at random from an array:```qsharplet (succeeded, element) = MaybeChooseElement(    data,    DiscreteUniformDistribution(0, Length(data) - 1));Fact(succeeded, "Index chosen by MaybeChooseElement was not valid.");```