---
uid: Microsoft.Quantum.Arithmetic.MultiplyByModularInteger
title: MultiplyByModularInteger operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Arithmetic
qsharp.name: MultiplyByModularInteger
qsharp.summary: Performs modular multiplication by an integer constant on a qubit register.
---

# MultiplyByModularInteger operation

Namespace: [Microsoft.Quantum.Arithmetic](xref:Microsoft.Quantum.Arithmetic)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Performs modular multiplication by an integer constant on a qubit register.

```qsharp
operation MultiplyByModularInteger (constMultiplier : Int, modulus : Int, multiplicand : Microsoft.Quantum.Arithmetic.LittleEndian) : Unit is Adj + Ctl
```


## Description

Let us denote `modulus` by $N$ and `constMultiplier` by $a$.Then this operation implements a unitary operation defined by the following map on thecomputational basis:$$\begin{align}\ket{y} \mapsto \ket{(a \cdot y) \operatorname{mod} N}\end{align}$$for all $y$ between $0$ and $N - 1$.

## Input

### constMultiplier : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

Constant by which multiplicand is being multiplied. Must be co-prime to modulus.


### modulus : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)

The multiplication operation is performed modulo `modulus`.


### multiplicand : [LittleEndian](xref:Microsoft.Quantum.Arithmetic.LittleEndian)

The number being multiplied by a constant.This is an array of qubits encoding an integer in little-endian format.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Remarks

- For the circuit diagram and explanation see Figure 7 on [Page 8  of arXiv:quant-ph/0205095v3](https://arxiv.org/pdf/quant-ph/0205095v3.pdf#page=8)- This operation corresponds to Uₐ in  [arXiv:quant-ph/0205095v3](https://arxiv.org/pdf/quant-ph/0205095v3.pdf)