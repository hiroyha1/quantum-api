---
uid: Microsoft.Quantum.Random.NormalDistribution
title: NormalDistribution function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Random
qsharp.name: NormalDistribution
qsharp.summary: Returns a normal distribution with a given mean and variance.
---

# NormalDistribution function

Namespace: [Microsoft.Quantum.Random](xref:Microsoft.Quantum.Random)

Package: [Microsoft.Quantum.QSharp.Foundation](https://nuget.org/packages/Microsoft.Quantum.QSharp.Foundation)


Returns a normal distribution with a given mean and variance.

```qsharp
function NormalDistribution (mean : Double, variance : Double) : Microsoft.Quantum.Random.ContinuousDistribution
```


## Input

### mean : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)




### variance : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)





## Output : [ContinuousDistribution](xref:Microsoft.Quantum.Random.ContinuousDistribution)



## Example

The following draws 10 samples from the normal distribution with mean2 and standard deviation 0.1:```qsharplet samples = DrawMany(    (NormalDistribution(2.0, PowD(0.1, 2.0)))::Sample,    10, ());```

## See Also

- [Microsoft.Quantum.Random.StandardNormalDistribution](xref:Microsoft.Quantum.Random.StandardNormalDistribution)