---
uid: Microsoft.Quantum.Diagnostics.AssertQubitIsInStateWithinTolerance
title: AssertQubitIsInStateWithinTolerance operation
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: operation
qsharp.namespace: Microsoft.Quantum.Diagnostics
qsharp.name: AssertQubitIsInStateWithinTolerance
qsharp.summary: >-
  Asserts that a qubit in the expected state.

  `expected` represents a complex vector, $\ket{\psi} = \begin{bmatrix}a & b\end{bmatrix}^{\mathrm{T}}$.
  The first element of the tuples representing each of $a$, $b$
  is the real part of the complex number, while the second one is the imaginary part.
  The last argument defines the tolerance with which assertion is made.
---

# AssertQubitIsInStateWithinTolerance operation

Namespace: [Microsoft.Quantum.Diagnostics](xref:Microsoft.Quantum.Diagnostics)

Package: [Microsoft.Quantum.QSharp.Foundation](https://nuget.org/packages/Microsoft.Quantum.QSharp.Foundation)


Asserts that a qubit in the expected state.`expected` represents a complex vector, $\ket{\psi} = \begin{bmatrix}a & b\end{bmatrix}^{\mathrm{T}}$.The first element of the tuples representing each of $a$, $b$is the real part of the complex number, while the second one is the imaginary part.The last argument defines the tolerance with which assertion is made.

```qsharp
operation AssertQubitIsInStateWithinTolerance (expected : (Microsoft.Quantum.Math.Complex, Microsoft.Quantum.Math.Complex), register : Qubit, tolerance : Double) : Unit is Adj + Ctl
```


## Input

### expected : ([Complex](xref:Microsoft.Quantum.Math.Complex),[Complex](xref:Microsoft.Quantum.Math.Complex))

Expected complex amplitudes for $\ket{0}$ and $\ket{1}$, respectively.


### register : [Qubit](xref:microsoft.quantum.qsharp.valueliterals#qubit-literals)

Qubit whose state is to be asserted. Note that this qubit is assumed to be separablefrom other allocated qubits, and not entangled.


### tolerance : [Double](xref:microsoft.quantum.qsharp.valueliterals#double-literals)

Additive tolerance by which actual amplitudes are allowed to deviate from expected.See remarks below for details.



## Output : [Unit](xref:microsoft.quantum.qsharp.valueliterals#unit-literal)



## Example

```qsharpusing (qubits = Qubit[2]) {    // Both qubits are initialized as |0〉: a=(1 + 0*i), b=(0 + 0*i)    AssertQubitIsInStateWithinTolerance((Complex(1., 0.), Complex(0., 0.)), qubits[0], 1e-5);    AssertQubitIsInStateWithinTolerance((Complex(1., 0.), Complex(0., 0.)), qubits[1], 1e-5);    Y(qubits[1]);    // Y |0〉 = i |1〉: a=(0 + 0*i), b=(0 + 1*i)    AssertQubitIsInStateWithinTolerance((Complex(0., 0.), Complex(0., 1.)), qubits[1], 1e-5);}```

## Remarks

The following Mathematica code can be used to verify expressions for mi, mx, my, mz:```mathematica{Id, X, Y, Z} = Table[PauliMatrix[k], {k, 0, 3}];st = {{ reA + I imA }, { reB + I imB} };M = st . ConjugateTranspose[st];mx = Tr[M.X] // ComplexExpand;my = Tr[M.Y] // ComplexExpand;mz = Tr[M.Z] // ComplexExpand;mi = Tr[M.Id] // ComplexExpand;2 m == Id mi + X mx + Z mz + Y my // ComplexExpand // Simplify```The tolerance isthe $L\_{\infty}$ distance between 3 dimensional real vector (x₂,x₃,x₄) defined by$\langle\psi|\psi\rangle = x\_1 I + x\_2 X + x\_3 Y + x\_4 Z$ and real vector (y₂,y₃,y₄) defined byρ = y₁I + y₂X + y₃Y + y₄Z where ρ is the density matrix corresponding to the state of the register.This is only true under the assumption that Tr(ρ) and Tr(|ψ⟩⟨ψ|) are both 1 (e.g. x₁ = 1/2, y₁ = 1/2).If this is not the case, the function asserts that l∞ distance between(x₂-x₁,x₃-x₁,x₄-x₁,x₄+x₁) and (y₂-y₁,y₃-y₁,y₄-y₁,y₄+y₁) is less than the tolerance parameter.Note that the Adjoint and Controlled versions of this operation will notcheck the condition.