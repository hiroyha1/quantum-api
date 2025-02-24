---
uid: Microsoft.Quantum.Math.ExpModI
title: ExpModI function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Math
qsharp.name: ExpModI
qsharp.summary: >-
  Returns an integer raised to a given power, with respect to a given
  modulus.
---

# ExpModI function

Namespace: [Microsoft.Quantum.Math](xref:Microsoft.Quantum.Math)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Returns an integer raised to a given power, with respect to a givenmodulus.

```qsharp
function ExpModI (expBase : Int, power : Int, modulus : Int) : Int
```


## Description

Let us denote expBase by $x$, power by $p$ and modulus by $N$.The function returns $x^p \operatorname{mod} N$.We assume that $N$, $x$ are positive and power is non-negative.

## Input

### expBase : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)




### power : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)




### modulus : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)





## Output : [Int](xref:microsoft.quantum.qsharp.valueliterals#int-literals)



## Remarks

Takes time proportional to the number of bits in `power`, not the `power` itself.