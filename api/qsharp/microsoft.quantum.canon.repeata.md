---
uid: Microsoft.Quantum.Canon.RepeatA
title: RepeatA operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Canon
qsharp.name: RepeatA
qsharp.summary: Repeats an operation a given number of times.
---

# RepeatA operation

Namespace: [Microsoft.Quantum.Canon](xref:Microsoft.Quantum.Canon)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Repeats an operation a given number of times.

```qsharp
operation RepeatA<'TInput> (op : ('TInput => Unit is Adj), nTimes : Int, input : 'TInput) : Unit is Adj
```


## Input

### op : 'TInput => [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)  is Adj

The operation to be called repeatedly.


### nTimes : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The number of times to call `op`.


### input : 'TInput

The input to be passed to `op`.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Type Parameters

### 'TInput



## Example

The following are equivalent:```qsharpRepeatA(U, 17, target);(BoundA(ConstantArray(17, U)))(target);```

## See Also

- [Microsoft.Quantum.Arrays.DrawMany](xref:Microsoft.Quantum.Arrays.DrawMany)
- [Microsoft.Quantum.Canon.Repeat](xref:Microsoft.Quantum.Canon.Repeat)
- [Microsoft.Quantum.Canon.RepeatC](xref:Microsoft.Quantum.Canon.RepeatC)
- [Microsoft.Quantum.Canon.RepeatCA](xref:Microsoft.Quantum.Canon.RepeatCA)