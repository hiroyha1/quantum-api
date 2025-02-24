---
uid: Microsoft.Quantum.Simulation.QuantumProcessor.Extensions.ApplyIfElseIntrinsicCA
title: ApplyIfElseIntrinsicCA operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Simulation.QuantumProcessor.Extensions
qsharp.name: ApplyIfElseIntrinsicCA
qsharp.summary: >+
  > [!WARNING]

  > ApplyIfElseIntrinsicCA has been deprecated. Please use <xref:Microsoft.Quantum.ClassicalControl.ApplyIfElseIntrinsicCA> instead.

---

# ApplyIfElseIntrinsicCA operation

Namespace: [Microsoft.Quantum.Simulation.QuantumProcessor.Extensions](xref:Microsoft.Quantum.Simulation.QuantumProcessor.Extensions)

Package: [Microsoft.Quantum.QSharp.Foundation](https://nuget.org/packages/Microsoft.Quantum.QSharp.Foundation)


> [!WARNING]
> ApplyIfElseIntrinsicCA has been deprecated. Please use <xref:Microsoft.Quantum.ClassicalControl.ApplyIfElseIntrinsicCA> instead.



```qsharp
operation ApplyIfElseIntrinsicCA (measurementResult : Result, onResultZeroOp : (Unit => Unit is Ctl + Adj), onResultOneOp : (Unit => Unit is Ctl + Adj)) : Unit is Adj + Ctl
```


## Input

### measurementResult : [Result](xref:microsoft.quantum.qsharp.valueliterals#result-literal)




### onResultZeroOp : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal) => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj + Ctl




### onResultOneOp : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal) => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj + Ctl





## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)

