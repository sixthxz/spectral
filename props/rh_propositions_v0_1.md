# RH Compression Ledger — Propositions v0.1

## Purpose

This document begins the proposition layer after the controlled vocabulary.

The propositions are deliberately conservative. They separate:

```text
theorem-level statements
ledger-level interpretations
RH-level claims
```

No proposition below proves the Riemann Hypothesis.

---

## Proposition 1 — Involution Invariance Is Not Critical-Line Occupancy

### Theorem-level statement

The completed xi function satisfies:

```text
xi(s) = xi(1-s)
```

Equivalently, if:

```text
I(s) = 1-s
```

then:

```text
xi(I(s)) = xi(s)
```

So `xi` is invariant under the involution:

```text
s -> 1-s
```

### Consequence

If:

```text
xi(s) = 0
```

then:

```text
xi(1-s) = 0
```

Thus the zero set is invariant under the involution.

### Important distinction

The involution:

```text
I(s)=1-s
```

has only one fixed point:

```text
s = 1/2
```

The critical line:

```text
Re(s)=1/2
```

is not pointwise fixed. It is setwise invariant, since:

```text
I(1/2+it)=1/2-it
```

### What this does not imply

It does not imply:

```text
Re(s) = 1/2
```

for every nontrivial zero.

It does not imply that every zero is a fixed point of the involution.

### Ledger-level annotation

The ledger may annotate the involution:

```text
s -> 1-s
```

as reading reversal of the completed object.

### Guardrail

Reading reversal is not the same as critical-line occupancy.

An involution-invariant zero set may contain zeros on the setwise invariant critical line and/or off-line zeros appearing in involution-related pairs.

RH requires that the nontrivial zero set be contained in:

```text
Re(s)=1/2
```

not that every zero be a fixed point of the involution.

---

## Proposition 2 — Centering Makes the Involution Visible

### Theorem-level statement

Introduce the centered coordinate:

```text
s = 1/2 + w
```

Then:

```text
1-s = 1 - (1/2 + w) = 1/2 - w
```

So the involution becomes:

```text
w -> -w
```

### Consequence

The completed symmetry becomes:

```text
xi(1/2 + w) = xi(1/2 - w)
```

This shows that, in the centered coordinate, the completed object is invariant under `w -> -w`.

### What this does not imply

It does not imply that zeros must have:

```text
w = it
```

or:

```text
Re(w) = 0
```

It only shows that the coordinate system centered at `1/2` is natural for the involution.

### Ledger-level annotation

The centered coordinate is the coordinate in which reading reversal becomes explicit:

```text
w -> -w
```

### Guardrail

A natural centered coordinate is not a zero-location theorem.

---

## Proposition 3 — Critical-Line Form Is a Restricted Reading, Not a General Zero Parametrization

### Theorem-level statement

On the critical line, one writes:

```text
s = 1/2 + it
```

and defines:

```text
Xi(t) = xi(1/2 + it)
```

The symmetry:

```text
xi(s) = xi(1-s)
```

implies:

```text
Xi(t) = Xi(-t)
```

### Consequence

`Xi(t)` is an even function of the real variable `t`.

### What this does not imply

It does not imply that every nontrivial zero can be written as:

```text
1/2 + it
```

unless RH is assumed or proved.

For a general nontrivial zero, the safe notation remains:

```text
rho = beta + i gamma
```

with:

```text
0 < beta < 1
```

### Ledger-level annotation

The `t`-coordinate is a centered reading coordinate restricted to the critical line.

### Guardrail

Critical-line notation must not silently encode RH.

---

## Proposition 4 — Differentiation Gives Antisymmetry, Not Line-Wide Vanishing

### Theorem-level statement

From:

```text
xi(s) = xi(1-s)
```

differentiate with respect to `s`:

```text
xi'(s) = -xi'(1-s)
```

### Consequence at the fixed point

At:

```text
s = 1/2
```

we have:

```text
1-s = s
```

so:

```text
xi'(1/2) = -xi'(1/2)
```

and therefore:

```text
xi'(1/2) = 0
```

### Consequence on the critical line

At:

```text
s = 1/2 + it
```

the derivative relation is:

```text
xi'(1/2 + it) = -xi'(1/2 - it)
```

### What this does not imply

It does not imply:

```text
xi'(1/2 + it) = 0
```

for all `t`.

Equivalently, from:

```text
Xi(t) = Xi(-t)
```

we get:

```text
Xi'(t) = -Xi'(-t)
```

which forces only:

```text
Xi'(0) = 0
```

not:

```text
Xi'(t) = 0
```

for all `t`.

### Ledger-level annotation

Differentiation is a decompression diagnostic. It shows how rates transform under the involution.

### Guardrail

Differentiation does not supply an RH-level claim.

---

## Proposition 5 — Cauchy-Riemann Constrains Local Analytic Behavior, Not Zero Location by Itself

### Theorem-level statement

Let:

```text
xi(s) = u(x,y) + i v(x,y)
```

with:

```text
s = x + iy
```

Since `xi` is holomorphic, the Cauchy-Riemann equations hold:

```text
u_x = v_y
u_y = -v_x
```

### Consequence

The local partial derivatives of `u` and `v` cannot be prescribed independently.

### What this does not imply

It does not imply that the coordinate directions `x` and `y` are not valid independent real coordinates.

It does not imply that off-line zeros are impossible.

It does not imply RH.

### Ledger-level annotation

The CR equations warn against treating variation in:

```text
a
```

from:

```text
s = 1/2 + a + it
```

as analytically unconstrained merely because it appears as a separate real coordinate.

### Guardrail

CR is a local analytic-structure constraint, not a global zero-location theorem.

---

## Proposition 6 — Numerical Spike Detection Is Diagnostic, Not Proof

### Theorem-level statement

For numerical visualization, define the log-modulus diagnostic for `xi(s) != 0`:

```text
L(s) = -log |xi(s)|
```

At zeros, one may regard `L(s)=+infinity` in the extended-real visualization sense.

### Consequence

A large finite value of `L(s)` can indicate small computed modulus.

### What this does not imply

A large value of `L(s)` is not automatically a rigorously verified zero.

A scan that does not detect off-line spikes does not prove that no off-line zeros exist.

### Ledger-level annotation

The simulations helped identify useful vocabulary:

```text
center-line log-modulus behavior
off-line displacement
boundary features
```

### Guardrail

Simulation results guide interpretation but do not establish RH.

---

## Proposition 7 — The Ledger Identifies a Framing Gap, Not a Missing Theorem

### Theorem-level statement

The formal historical chain includes:

```text
Euler series/product
analytic continuation
functional equation
completed xi
critical strip
critical line
zero-set formulations
```

### Ledger-level claim

The ledger tracks how the meaning and use of `s` shifts across this chain:

```text
exponent
convergence parameter
complex coordinate
involution-related coordinate
completed-object coordinate
centered ordinate
zero-location label
```

### Consequence

Some RH confusion may arise when these roles are collapsed into one undifferentiated use of `s`.

### What this does not imply

It does not imply that RH is solved by clarifying notation.

It does not imply that off-center zeros are impossible.

### Guardrail

The ledger identifies a framing gap. A proof would still require a theorem-level argument excluding off-center nontrivial zeros.

---

## Proposition 8 — The Core Unresolved Step

### Theorem-level situation

The completed zero set is invariant under:

```text
s -> 1-s
```

So if an off-center zero existed at:

```text
rho = beta + i gamma
```

with:

```text
0 < beta < 1
```

and:

```text
beta != 1/2
```

then the involution symmetry would require a corresponding zero at:

```text
1-rho
```

With conjugation symmetry included, this belongs to the usual symmetric orbit of related zeros.

### Ledger-level annotation

The ledger annotates this as the distinction between:

```text
involution-invariant zero set
```

and:

```text
zero set contained in the setwise invariant critical line
```

### What remains unresolved

RH requires moving from:

```text
zero set invariant under the involution
```

to:

```text
all nontrivial zeros lie on the critical line Re(s)=1/2
```

### Guardrail

This move is not supplied by:

```text
the functional equation alone
Cauchy-Riemann alone
the derivative relation alone
numerical scans alone
reading-reversal language alone
```

This is the precise remaining theorem-level gap.

---

## Proposition 9 — Safe Statement of the Project’s Current Result

### Claim

The project has not proved RH.

It has produced a controlled framework for separating:

```text
1. theorem-level symmetries of xi
2. ledger-level interpretation of compression and reading reversal
3. RH-level zero-location claims
```

### Consequence

The framework can clarify which statements are safe and which would require proof.

### Safe summary

```text
The completed xi function is invariant under s -> 1-s.
The ledger interprets that involution as reading reversal of the completed object.
This interpretation helps audit inherited coordinate assumptions.
It does not by itself prove that all nontrivial zeros lie on the critical line.
```

---

## Next Question After These Propositions

The next theorem-level question is:

```text
What additional structure, beyond involution invariance and holomorphicity,
could force an involution-invariant zero set to be contained in the critical line?
```

In classical terms, this points toward structures such as:

```text
positivity
self-adjointness
Hilbert-Polya type spectral realization
de Branges-type Hilbert spaces
explicit formula constraints
```

But those are future tracks. They should not be imported into the current propositions without separate review.
