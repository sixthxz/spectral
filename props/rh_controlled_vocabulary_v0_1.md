# RH Compression Ledger — Controlled Vocabulary v0.2

## Purpose

This document defines the minimal vocabulary needed before writing or repairing propositions.

The goal is to prevent category mistakes between:

```text
theorem-level statements
ledger-level annotations
RH-level claims
```

Nothing in this vocabulary claims a proof of the Riemann Hypothesis.

---

## 0. Global Status Rule

Every statement in this project must be classifiable as one of the following:

```text
theorem-level
ledger-level
RH-level
numerical-diagnostic level
```

A ledger-level annotation cannot serve as a theorem-level hypothesis, lemma, or inference rule unless it is translated back into theorem-level mathematics.

The most important distinction:

```text
I(s)=1-s has one fixed point: s=1/2.
The critical line Re(s)=1/2 is setwise invariant under I.
```

Therefore, avoid the phrase:

```text
fixed-point occupancy of zeros
```

when discussing RH.

Use instead:

```text
critical-line occupancy of zeros
```

or:

```text
zero set contained in the critical line Re(s)=1/2
```

---

## 1. Theorem-Level Statement

### Definition

A theorem-level statement is a standard mathematical statement expressible in ordinary complex analysis or analytic number theory.

### Allowed meaning

It may include formulas such as:

```text
xi(s) = xi(1-s)
```

or:

```text
xi'(s) = -xi'(1-s)
```

when derived by ordinary rules.

### Not allowed to mean

It does not include interpretive vocabulary unless that vocabulary has been translated into theorem-level mathematics.

It does not mean:

```text
reading orientation is a theorem
```

or:

```text
the functional equation proves RH
```

### Related formula

```text
xi(s) = xi(1-s)
```

---

## 2. Ledger-Level Annotation

### Definition

A ledger-level annotation is a non-theorem annotation of theorem-level statements, used only to track notation, compression, coordinate choices, and explicit assumptions.

### Allowed meaning

A ledger-level annotation may gloss:

```text
xi(s) = xi(1-s)
```

as a reading-reversal annotation.

### Not allowed to mean

A ledger-level annotation cannot serve as a hypothesis, lemma, inference rule, or proof step unless translated back into theorem-level statements.

It cannot be used by itself to conclude zero-location results.

### Related formula

```text
theorem-level: xi(s) = xi(1-s)
ledger-level gloss: interpreted as reading reversal
```

---

## 3. RH-Level Claim

### Definition

An RH-level claim is any statement that asserts, implies, or requires that all nontrivial zeros of `zeta(s)` or `xi(s)` lie on the critical line.

### Allowed meaning

The classical RH claim is:

```text
if zeta(s)=0 and 0<Re(s)<1, then Re(s)=1/2
```

Equivalent completed-object phrasing:

```text
all nontrivial zeros of xi(s) in the critical strip occur on Re(s)=1/2
```

### Not allowed to mean

An RH-level claim must not be smuggled in through notation such as:

```text
rho = 1/2 + i gamma
```

unless RH is being assumed.

### Related formula

```text
Re(rho) = 1/2
```

---

## 4. Completed Object

### Definition

The completed object is the Riemann xi-function, defined here by:

```text
xi(s) = 1/2 · s(s-1) · pi^(-s/2) · Gamma(s/2) · zeta(s)
```

It is entire and satisfies:

```text
xi(s) = xi(1-s)
```

### Allowed meaning

The completed object is the completed Riemann xi-function obtained from `zeta(s)` by the displayed gamma factor and polynomial factor, satisfying the functional equation.

### Not allowed to mean

It is not merely `zeta(s)` under another name.

It is not evidence by itself that every nontrivial zero lies on the critical line.

### Related formula

```text
xi(s)=xi(1-s)
```

---

## 5. Involution

### Definition

An involution is a map that undoes itself when applied twice.

Here the relevant involution is:

```text
I(s) = 1-s
```

so:

```text
I(I(s)) = s
```

### Allowed meaning

The functional equation says the completed object is invariant under this involution:

```text
xi(I(s)) = xi(s)
```

The critical line is setwise invariant under this involution:

```text
I(1/2 + it) = 1/2 - it
```

### Not allowed to mean

The involution does not make `s` and `1-s` literally the same complex point, except at the single fixed point:

```text
s = 1/2
```

Do not say that every point on the critical line is a fixed point of the involution.

### Related formula

```text
s -> 1-s
```

---

## 6. Reading Label

### Definition

A reading label is ledger shorthand for one of two distinct coordinate inputs `s` and `1-s` whose `xi`-values are equal by the functional equation.

### Allowed meaning

In ledger-level commentary only, the pair:

```text
(s, 1-s)
```

may be annotated as an involution-paired pair of coordinate inputs.

### Not allowed to mean

This annotation does not identify the inputs.

A reading label is not a standard replacement for the complex coordinate.

It does not erase the fact that `s` and `1-s` are generally distinct complex inputs.

### Related formula

```text
xi(s)=xi(1-s)
```

---

## 7. Reading Reversal

### Definition

Reading reversal means only the operation:

```text
I(s)=1-s
```

when discussed in ledger-level language.

### Allowed meaning

At ledger level, one may say that the functional equation is glossed as reading reversal.

### Not allowed to mean

Any theorem-level use must be restated as:

```text
s -> 1-s
```

Reading reversal is not itself a proof that zeros lie on the critical line.

It does not imply:

```text
s = 1-s
```

for every zero.

### Related formula

```text
xi(s)=xi(1-s)
```

---

## 8. Centered Coordinate

### Definition

The centered coordinate rewrites `s` around the setwise invariant vertical line:

```text
Re(s)=1/2
```

associated with the involution:

```text
s -> 1-s
```

Use:

```text
s = 1/2 + w
```

Then:

```text
I(s)=1-s=1/2-w
```

so the involution becomes:

```text
w -> -w
```

### Critical-line specialization

On the critical line, one writes:

```text
s = 1/2 + it
```

and then:

```text
I(1/2+it)=1/2-it
```

The critical line is invariant as a set, not pointwise fixed.

The only fixed point of the involution is:

```text
s=1/2
```

### Not allowed to mean

Writing:

```text
s = 1/2 + it
```

for a zero is not legitimate unless the zero is already known or assumed to be on the critical line.

For a general nontrivial zero, use:

```text
rho = beta + i gamma
```

unless RH is assumed.

### Related formula

```text
s = 1/2 + w
```

---

## 9. Zero-Status

### Definition

Define the predicate:

```text
Z(s) : xi(s)=0
```

The phrase “zero-status at `s`” is ledger shorthand for:

```text
Z(s)
```

### Allowed meaning

It records the predicate:

```text
xi(s)=0
```

without imposing any additional condition such as:

```text
Re(s)=1/2
```

### Not allowed to mean

Zero-status does not by itself imply critical-line status.

It does not mean:

```text
s = 1/2 + it
```

unless additional information establishes that.

### Related formula

```text
Z(s) : xi(s)=0
```

---

## 10. Coordinate Location

### Definition

A coordinate location is a point in the complex plane, usually written:

```text
s = sigma + it
```

or for a zero:

```text
rho = beta + i gamma
```

### Allowed meaning

Coordinate location is the standard complex-analysis way of identifying inputs.

### Not allowed to mean

Coordinate location should not be confused with zero-status.

A location can be written down freely; zero-status is an additional predicate.

### Related formula

```text
s = sigma + it
```

---

## 11. Object-Status

### Definition

Object-status is a theorem-level predicate or relation involving explicit coordinate inputs of `xi`.

Unary example:

```text
Z(s) : xi(s)=0
```

Binary/symmetric example:

```text
R(s) : xi(s)=xi(1-s)
```

### Allowed meaning

Object-status tracks predicates or relations involving the completed object and explicit coordinate inputs.

### Not allowed to mean

Object-status does not erase ordinary domain coordinates.

It is not a proof that off-line coordinates cannot be considered.

Do not mix unary and binary statuses without specifying arity.

### Related formulas

```text
Z(s) : xi(s)=0
R(s) : xi(s)=xi(1-s)
```

---

## 12. Off-Center Zero-Status

### Definition

Off-center zero-status means a hypothetical zero:

```text
rho = beta + i gamma
```

of `xi` with:

```text
0 < beta < 1
```

and:

```text
beta != 1/2
```

### Allowed meaning

This is exactly the type of zero RH says does not exist.

### Not allowed to mean

Do not treat off-center zero-status as already impossible unless RH has been proved or assumed.

Do not treat numerical non-detection as proof of nonexistence.

### Related formula

```text
xi(beta+i gamma)=0, 0<beta<1, beta != 1/2
```

---

## 13. Decompression Check

### Definition

A decompression check unpacks a compressed identity without adding new theorem-level content.

For example, it unpacks:

```text
xi(s)=xi(1-s)
```

into:

```text
theorem-level: invariance under s -> 1-s
ledger-level gloss: interpreted as reading reversal
```

### Allowed meaning

A decompression check may expose what an identity says and what it does not say.

### Not allowed to mean

It is not a proof step unless the unpacked content is theorem-level and the inference is valid.

It must not claim:

```text
xi'(1/2+it)=0 for all t
```

because the derivative relation only gives:

```text
xi'(1/2+it) = -xi'(1/2-it)
```

### Related formula

```text
xi'(s) = -xi'(1-s)
```

---

## 14. Analytic-Structure Constraint

### Definition

An analytic-structure constraint is a standard holomorphic constraint on the local behavior of a one-complex-variable function.

If:

```text
xi(s) = u(x,y) + i v(x,y)
```

with:

```text
s = x + iy
```

then holomorphicity gives:

```text
u_x = v_y
u_y = -v_x
```

### Allowed meaning

The Cauchy-Riemann equations constrain the local partial-derivative relations of the real and imaginary parts.

### Not allowed to mean

They do not eliminate off-line zeros.

They do not make the coordinate `a` in:

```text
s = 1/2 + a + it
```

unavailable as a coordinate parameter.

### Related formula

```text
u_x = v_y
u_y = -v_x
```

---

## 15. Log-Modulus Diagnostic

### Definition

For:

```text
xi(s) != 0
```

define:

```text
L(s) = -log |xi(s)|
```

At zeros, one may regard:

```text
L(s)=+infinity
```

in the extended-real visualization sense.

### Allowed meaning

Large finite values of `L(s)` indicate small computed modulus.

This is a numerical diagnostic for visualization and exploration.

### Not allowed to mean

A large value of `L(s)` is not automatically a rigorously verified zero.

A scan that does not detect off-line spikes is not a proof that no off-line zeros exist.

Without rigorous error bounds, the diagnostic carries no zero-existence or zero-nonexistence conclusion.

### Related formula

```text
L(s) = -log |xi(s)|
```

---

## Safe Proposition Template

A safe proposition should separate theorem-level, ledger-level, and RH-level content.

Example:

```text
Proposition 1.
The functional equation xi(s)=xi(1-s) gives invariance of the completed object under s -> 1-s, and therefore symmetry of the zero set under this map.

Ledger gloss.
This project may annotate the involution as reading reversal of the completed object.

Guardrail.
This does not imply that zeros lie on Re(s)=1/2, and therefore does not prove RH.
```

---

## Forbidden Shortcuts

Do not write:

```text
xi(s)=xi(1-s), therefore all zeros lie on Re(s)=1/2
```

Do not write:

```text
Cauchy-Riemann removes transverse freedom, therefore no off-line zeros
```

Do not write:

```text
s and 1-s are the same point
```

Do not write:

```text
the derivative vanishes on the whole critical line
```

Do not write:

```text
numerical scans found no off-line spikes, therefore RH holds
```

Do not write:

```text
critical-line zeros are fixed points of s -> 1-s
```

unless the zero is exactly:

```text
s=1/2
```

---

## Next Step

After this vocabulary is reviewed, the first formal proposition should be:

```text
The functional equation gives invariance of the completed object under s -> 1-s,
and therefore symmetry of the zero set under this map,
but it does not imply that zeros lie on Re(s)=1/2.
```

Then the project can ask what additional structure would be required to move from:

```text
involution-invariant zero set
```

to:

```text
zero set contained in the critical line Re(s)=1/2
```
