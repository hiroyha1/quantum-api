---
uid: Microsoft.Quantum.AmplitudeAmplification.FixedPointReflectionPhases
title: FixedPointReflectionPhases function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.AmplitudeAmplification
qsharp.name: FixedPointReflectionPhases
qsharp.summary: >-
  Computes partial reflection phases for fixed-point amplitude
  amplification.
---

# FixedPointReflectionPhases function

Namespace: [Microsoft.Quantum.AmplitudeAmplification](xref:Microsoft.Quantum.AmplitudeAmplification)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Computes partial reflection phases for fixed-point amplitudeamplification.

```qsharp
function FixedPointReflectionPhases (nQueries : Int, successMin : Double) : Microsoft.Quantum.AmplitudeAmplification.ReflectionPhases
```


## Input

### nQueries : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

Number of queries to the state preparation oracle. Must be an oddinteger.


### successMin : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

Target minimum success probability.



## Output : [ReflectionPhases](xref:Microsoft.Quantum.AmplitudeAmplification.ReflectionPhases)

Array of phases that can be used in fixed-point amplitude amplificationquantum algorithm implementation.

## References

We use the phases in "Fixed-Point Amplitude Amplification withan Optimal Number of Queries"- [YoderLowChuang2014](https://arxiv.org/abs/1409.3305)  See also "Methodology of composite quantum gates"- [LowYoderChuang2016](https://arxiv.org/abs/1603.03996)  for phases in the `RotationPhases` format.