---
uid: Microsoft.Quantum.Diagnostics.EqualityFactCP
title: EqualityFactCP function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Diagnostics
qsharp.name: EqualityFactCP
qsharp.summary: Asserts that a complex number has the expected value.
---

# EqualityFactCP function

Namespace: [Microsoft.Quantum.Diagnostics](xref:Microsoft.Quantum.Diagnostics)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Asserts that a complex number has the expected value.

```qsharp
function EqualityFactCP (actual : Microsoft.Quantum.Math.ComplexPolar, expected : Microsoft.Quantum.Math.ComplexPolar, message : String) : Unit
```


## Input

### actual : [ComplexPolar](xref:Microsoft.Quantum.Math.ComplexPolar)

The value to be checked.


### expected : [ComplexPolar](xref:Microsoft.Quantum.Math.ComplexPolar)

The expected value.


### message : [String](xref:microsoft.quantum.qsharp.valueliterals#string-literals)

Failure message string to be used when the assertion is triggered.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

