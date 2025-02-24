---
uid: Microsoft.Quantum.Intrinsic.Ry
title: Ry operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Intrinsic
qsharp.name: Ry
qsharp.summary: Applies a rotation about the $y$-axis by a given angle.
---

# Ry operation

Namespace: [Microsoft.Quantum.Intrinsic](xref:Microsoft.Quantum.Intrinsic)

Package: [Microsoft.Quantum.QSharp.Core](https://nuget.org/packages/Microsoft.Quantum.QSharp.Core)


Applies a rotation about the $y$-axis by a given angle.

```qsharp
operation Ry (theta : Double, qubit : Qubit) : Unit is Adj + Ctl
```


## Description

\begin{align}R_y(\theta) \mathrel{:=}e^{-i \theta \sigma_y / 2} =\begin{bmatrix}\cos \frac{\theta}{2} & -\sin \frac{\theta}{2}  \\\\\sin \frac{\theta}{2} & \cos \frac{\theta}{2}\end{bmatrix}.\end{align}

## Input

### theta : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

Angle in radians about which the qubit is to be rotated.


### qubit : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Qubit to which the gate should be applied.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Remarks

Equivalent to:```qsharpR(PauliY, theta, qubit);```