# CGET: Capability-Grounded Evolutionary Topology

## Purpose

CGET is the measurement framework for Grounded Recursive Adaptation.

GRA defines the condition for adaptive self-transformation.

CGET defines how to observe and measure whether that condition is preserved.

The distinction:

- GRA: what must remain true
- CGET: how we measure whether it remains true

---

# Core State

A recursively adapting system is represented as:

\[
A_n=(K_n,\mathcal C_n,\Lambda_n,\Gamma_n)
\]

where:

## \(K_n\)

The current transformation mechanism.

Includes:

- architecture
- optimizer
- update rules
- internal representations
- self-modification procedures

---

## \(\mathcal C_n\)

Consequence connectivity.

\[
\mathcal C_n=I(\Delta A_n;\Delta E_n)
\]

Measures whether environmental changes remain causally connected to system changes.

Question:

> Does reality still influence behavior?

Failure:

\[
\mathcal C\rightarrow0
\]

Blindness.

---

## \(\Lambda_n\)

Information yield.

\[
\Lambda_n=D_{KL}(R_{n+1}\parallel R_n)
\]

Measures whether experience produces new internal structure.

Question:

> Does interaction generate new useful information?

Failure:

\[
\Lambda\rightarrow0
\]

Saturation.

---

## \(\Gamma_n\)

Learning improvement.

\[
\Gamma_n=\Delta\left(\frac{\Delta R}{\Delta E}\right)
\]

Measures whether the system improves its own ability to extract structure.

Question:

> Is learning itself improving?

Failure:

\[
\Gamma\rightarrow0
\]

Stagnation.

---

# Grounding Condition

The above variables describe capability.

They do not determine whether capability remains adaptive.

That requires:

\[
\Theta_n>0
\]

where:

\[
\Theta_n=
D_n\cdot S_n\cdot P_n
\]

---

## Direction

\[
D_n=
Corr(\Delta K_n,\Delta E_n^{real})
\]

Does self-modification move according to real consequences?

---

## Strength

\[
S_n=|\Delta K_n^{valid}|
\]

Does consequence actually modify the transformation mechanism?

---

## Persistence

\[
P_n=P(\Theta_{0:n}>\epsilon)
\]

Does grounding survive recursive depth?

---

# CGET Interpretation

A system can have:

\[
\mathcal C,\Lambda,\Gamma\uparrow
\]

while:

\[
\Theta\downarrow
\]

This is the critical failure regime.

The system becomes:

\[
\text{more capable}
\neq
\text{more adaptive}
\]

Capability can continue increasing after adaptation has failed.

---

# Corrigibility Horizon

The primary CGET measurement is:

\[
n^*=
\sup\{n|\Theta_n>\epsilon\}
\]

The horizon measures:

> How far can a system recursively transform itself before consequences lose authority over future transformation?

---

# CGET and GRA

GRA provides the invariant relationship:

\[
E_n\rightarrow K_{n+1}
\]

CGET provides the diagnostic space:

\[
(K_n,\mathcal C_n,\Lambda_n,\Gamma_n,\Theta_n)
\]

Together:

\[
\boxed{
\text{GRA defines adaptive validity}
}
\]

\[
\boxed{
\text{CGET measures adaptive validity}
}
\]

---

# Summary

CGET does not define intelligence.

It defines the boundary between:

\[
\text{open-ended adaptation}
\]

and:

\[
\text{closed optimization}
\]

Its purpose is to detect whether increasing capability is still connected to the process that allows reality to correct the system.
