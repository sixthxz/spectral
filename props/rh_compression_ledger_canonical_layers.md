# RH Compression Ledger — Stage 3 + Analytic-Structure Layer

## Status

Working research note.  
This document does not claim a proof of the Riemann Hypothesis.

It separates four layers:

```text
Layer 0: analytic-structure constraint
Layer 1: historical/formal transformations
Layer 2: coordinate-status shifts
Layer 3: reading-orientation interpretation
Layer 4: decompression check of xi(s)=xi(1-s)
```

The current focus is Layer 3, but Layer 0 must be recorded because it sits below the historical ledger: one-complex-variable analyticity constrains the local relation between the real and imaginary components of the completed function before any completion-step interpretation is applied.

---

## Status Separation Guardrail

This document must keep three levels separate:

```text
Theorem-level:
    xi(s)=xi(1-s)
    symmetry under the involution s -> 1-s
    derivative relation xi'(s) = -xi'(1-s)

Ledger-level:
    this project interprets the completed symmetry as reading/access reversal
    of the completed object

RH-level:
    no zero-location conclusion follows from the theorem-level or ledger-level
    statements alone
```

The phrase "reading orientation" is ledger-level vocabulary. It is not a standard theorem-level statement in complex analysis.

When this document says that completion changes the role of `s`, that must be read as:

```text
completion changes how this ledger interprets the role of s
```

not as:

```text
the complex coordinate s literally stops being the input variable
```


## Core Guardrail

Do not treat the zero-status of `s` and `1-s` as unrelated once the completed functional equation has been imposed.

Also do not say that `s` and `1-s` are literally the same complex point.

The careful statement is:

```text
After completion, the equality `xi(s)=xi(1-s)` may be interpreted in this ledger as relating opposite reading/access labels of the completed analytic object.
```

This is not object-unification.  
It is not two things becoming one.  
It is a change in how this ledger interprets the role of the coordinate after completion.

---

## Layer 0: Analytic-Structure Constraint

Before the historical compression ledger even begins, there is a structural fact:

```text
xi is a function of one complex variable.
```

If:

```text
xi(s) = u(x,y) + i v(x,y)
```

with:

```text
s = x + iy
```

then holomorphicity ties `u` and `v` through the Cauchy-Riemann equations:

```text
u_x = v_y
u_y = -v_x
```

This means the partial derivatives of the real and imaginary components cannot be prescribed independently.

However, this must not be overstated.

Cauchy-Riemann does not by itself prove RH. A holomorphic function of one complex variable can have zeros off any chosen vertical line. So CR does not eliminate off-line zeros by itself.

What CR does establish is narrower:

```text
The transverse coordinate is a legitimate coordinate parameter, but the function's local behavior in that direction is constrained by holomorphicity.
```

This layer is important because it prevents us from treating variation in `a` in:

```text
s = 1/2 + a + it
```

as analytically unconstrained merely because it is written as a separate real coordinate. It is a coordinate direction inside one holomorphic variable.

---

## Decompression Check: What does `xi(s)=xi(1-s)` unpack into?

The functional equation for the completed object is:

```text
xi(s) = xi(1-s)
```

This section is not a derivative-proof attempt.  
It is a decompression check: unpack the compressed identity and track what it says about reading orientation.

The compressed identity says:

```text
the completed object is invariant under the involution `s -> 1-s`, which this ledger interprets as reversal of reading orientation
```

with opposite reading labels:

```text
s
```

and:

```text
1-s
```

This should not be read first as:

```text
an accidental equality of values at two unrelated domain points
```

It should be read as:

```text
the completed object has equal values at involution-related inputs `s` and `1-s`, which this ledger interprets as opposite reading labels
```

### Diagnostic consequence under differentiation

If one differentiates the identity with respect to `s`, one obtains:

```text
xi'(s) = -xi'(1-s)
```

This does not prove RH.  
It gives the chain-rule relation `xi'(s) = -xi'(1-s)`, which this ledger interprets as sign reversal under the involution.

At the fixed point of the involution:

```text
s = 1-s
```

that is:

```text
s = 1/2
```

the derivative relation gives:

```text
xi'(1/2) = 0
```

But along the critical line:

```text
s = 1/2 + it
```

the relation gives:

```text
xi'(1/2 + it) = -xi'(1/2 - it)
```

not:

```text
xi'(1/2 + it) = 0 for all t
```

In the centered real-line notation:

```text
Xi(t) = xi(1/2 + it)
```

the symmetry becomes:

```text
Xi(t) = Xi(-t)
```

so:

```text
Xi'(t) = -Xi'(-t)
```

which forces:

```text
Xi'(0) = 0
```

not:

```text
Xi'(t) = 0 for all t
```

### Role in the ledger

The derivative calculation stays only as a guardrail.

The real purpose of this section is the decompression:

```text
xi(s)=xi(1-s)
```

unpacks to:

```text
completed-object invariance under reading reversal
```

and not to:

```text
a proof that every point on the critical line has zero derivative
```

So this layer remains in the ledger, but as a decompression check rather than a derivative approach.

---

## Corrected Stage 3

### Theorem-level versus ledger-level wording

The theorem-level statement is:

```text
xi(s)=xi(1-s)
```

or equivalently symmetry under the involution:

```text
s -> 1-s
```

The reading-orientation language is this ledger's interpretive overlay. It must not be presented as standard theorem-level content.



### Stage 3: Completion changes how the ledger interprets the role of `s`

### Object

```text
xi(s) = 1/2 · s(s-1) · pi^(-s/2) · Gamma(s/2) · zeta(s)
```

with:

```text
xi(s) = xi(1-s)
```

and the centered convention:

```text
Xi(t) = xi(1/2 + it)
```

### Reading-orientation interpretation

Before completion, `s` can be treated as a domain coordinate for `zeta(s)`.

After completion, `s` remains the complex input variable, but this ledger additionally interprets its relation to `1-s` as a reading-orientation relation of the completed object.

The identity:

```text
xi(s) = xi(1-s)
```

should not be read first as:

```text
two independent points have equal output
```

It should be read as:

```text
the completed object has equal values at involution-related inputs `s` and `1-s`, which this ledger interprets as opposite reading labels
```

This does not make `s` and `1-s` the same complex point.

It changes what the coordinate is doing.

---

## Rewritten Ledger Rows

### Functional equation

Object:

```text
Lambda(s) = pi^(-s/2) Gamma(s/2) zeta(s)
```

with:

```text
Lambda(s) = Lambda(1-s)
```

Role of `s`:

```text
The completed zeta expression satisfies a symmetry relating the inputs `s` and `1-s`; this ledger interprets those related inputs as opposite access orientations.
```

What changed:

```text
After completion, `s` is the input of the completed object rather than only of raw `zeta(s)`; this ledger interprets the relation between `s` and `1-s` as a reversed reading orientation.
```

Guardrail:

```text
This does not make s and 1-s the same complex point.
```

Older reading that might incorrectly persist:

```text
s as merely the original exponent/convergence variable of sum n^(-s),
or s as an isolated input without dependence on completed normalization.
```

Ambiguity created for RH:

```text
Later RH interpretation can confuse equality of completed readings
with equality of raw zeta-values, or mistake orientation symmetry
for a zero-location theorem.
```

---

### Riemann xi / completed zeta

Object:

```text
xi(s) = 1/2 · s(s-1) · pi^(-s/2) · Gamma(s/2) · zeta(s)
```

with:

```text
xi(s) = xi(1-s)
```

and:

```text
Xi(t) = xi(1/2 + it)
```

Role of `s`:

```text
`s` is the complex coordinate of the pole-removed, entire, completed object; this ledger interprets its symmetry relation with `1-s` in reading-coordinate terms.
```

What changed:

```text
Completion changes the object under study from meromorphic `zeta(s)` to an entire normalized object expressed in the same complex coordinate `s`.

The central convention s = 1/2 + it then rewrites the reading
around the symmetry axis, with t as the vertical ordinate.
```

Older reading that might incorrectly persist:

```text
xi(s) as merely zeta(s) under a new name,
or s = 1/2 + it as already justified for every nontrivial zero.
```

Ambiguity created for RH:

```text
Later RH interpretation can blur three distinct layers:

1. raw zeta(s)
2. completed xi(s)
3. centered ordinate form Xi(t)

The completed symmetry makes the centered coordinate convention natural,
but does not by itself assert that all nontrivial zeros occupy that line.
```

---

## What the Simulations Contributed

The simulations are not the proof layer. They were diagnostic.

### Toy model result

The GCD/Fredholm toy had the zero rule:

```text
z_j(theta) = exp(-exp(i theta) log(lambda_j))
```

which implies:

```text
log |z_j(theta)| = -cos(theta) log(lambda_j)
```

At:

```text
theta = 90° or 270°
```

the radial term vanishes:

```text
cos(theta) = 0
```

so all toy zeros lock to:

```text
|z| = 1
```

This gave a toy-model example in which the chosen phase forces `|z|=1` at the specified angles.

### Zeta-side numerical result

For:

```text
s = 1/2 + a + it
```

the scans showed:

```text
a = 0
```

as the dominant spike behavior in the tested region.

The spike was:

```text
spike = -log |xi(s)|
```

Wide scans did not detect an independent off-line spike in the tested range.

Off-line-only scans appeared to show features attributable to nearby center-line spikes, rather than clearly separated off-line minima, within the tested resolution.

Interpretation of the simulations:

```text
They gave a direction and vocabulary.
They did not prove RH.
```

---

## Current Form of the Research Question

Do not ask:

```text
Where do the zeros occur?
```

Do not ask first:

```text
Why can there not be an off-center pair?
```

Instead ask:

```text
How can inherited coordinate language obscure the distinction between what completion symmetry constrains and what remains unresolved about off-center zero-status?
```

And below that:

```text
How does one-complex-variable analyticity constrain the apparent transverse direction
before any historical compression step is interpreted?
```

---

## Next Work

The next task is to build a two-level annotation over the historical ledger:

```text
1. Analytic-structure layer:
   What is already constrained by holomorphic one-variable structure?

2. Reading-orientation layer:
   Where does the ledger add a reading-coordinate interpretation to the standard role of `s` as the complex input of the completed object?
```

Differentiation can be used only as a diagnostic consequence inside the decompression check.

The Cauchy-Riemann approach is more foundational, but it must be kept precise:

```text
CR constrains the local partial-derivative relations of the real and imaginary parts.
CR does not by itself eliminate off-line zeros.
```
