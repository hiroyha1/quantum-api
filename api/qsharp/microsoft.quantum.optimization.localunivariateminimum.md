---
uid: Microsoft.Quantum.Optimization.LocalUnivariateMinimum
title: LocalUnivariateMinimum function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Optimization
qsharp.name: LocalUnivariateMinimum
qsharp.summary: >-
  Returns some local minimum for a univariate function over a bounded interval,
  using a golden interval search.
---

# LocalUnivariateMinimum function

Namespace: [Microsoft.Quantum.Optimization](xref:Microsoft.Quantum.Optimization)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Returns some local minimum for a univariate function over a bounded interval,using a golden interval search.

```qsharp
function LocalUnivariateMinimum (fn : (Double -> Double), bounds : (Double, Double), tolerance : Double) : Microsoft.Quantum.Optimization.UnivariateOptimizationResult
```


## Input

### fn : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals) -> [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

The univariate function to be minimized.


### bounds : ([Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals),[Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals))

The interval in which the local minimum is to be found.


### tolerance : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

The accuracy in the function input to be tolerated.The search for local optima will continue until the interval issmaller in width than this tolerance.



## Output : [UnivariateOptimizationResult](xref:Microsoft.Quantum.Optimization.UnivariateOptimizationResult)

A local optima of the given function, located within the given bounds.