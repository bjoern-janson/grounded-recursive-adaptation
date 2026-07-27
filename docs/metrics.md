# Metrics

## Overview

Grounded Recursive Adaptation requires separating three measurement categories:

1. **State variables** — what the system is.
2. **Capability metrics** — what the system can do.
3. **Grounding metrics** — whether those capabilities remain adaptively valid.

The central measurement problem:

\[
\boxed{
\text{Can capability increase while adaptive validity decreases?}
}
\]

GRA predicts that the answer is yes.

Therefore:

\[
\boxed{
\text{Capability}
\neq
\text{Adaptation}
}
\]

---

# 1. Transformation Mechanism

## \(K_t\)

The primary state variable:

\[
\boxed{
K_t
}
\]

represents the mechanism responsible for producing future changes.

Examples:

- neural weights
- policies
- optimizer parameters
- architectures
- search procedures
- self-modification rules

The measured transition:

\[
\boxed{
\Delta K_t=K_{t+1}-K_t
}
\]

is the object through which adaptation is evaluated.

---

# 2. Consequence Connectivity

## \(\mathcal C_t\)

Measures whether system actions remain causally coupled to environmental consequences.

\[
\boxed{
\mathcal C_t
=
I(\Delta A_t;\Delta E_t)
}
\]

where:

- \(\Delta A_t\) = action variation
- \(\Delta E_t\) = consequence variation

High:

\[
\mathcal C_t\uparrow
\]

means:

\[
\text{actions remain informative about reality}
\]

Low:

\[
\mathcal C_t\rightarrow0
\]

means:

\[
\text{the system loses causal feedback}
\]

---

# 3. Information Yield

## \(\Lambda_t\)

Measures whether interaction produces new internal structure.

\[
\boxed{
\Lambda_t
=
D_{KL}(R_{t+1}\parallel R_t)
}
\]

where:

- \(R_t\) = representation at time \(t\)

High:

\[
\Lambda_t\uparrow
\]

means:

\[
\text{experience continues changing the model}
\]

Low:

\[
\Lambda_t\rightarrow0
\]

means:

\[
\text{information frontier reached}
\]

---

# 4. Learning Improvement

## \(\Gamma_t\)

Measures improvement of the learning process itself.

\[
\boxed{
\Gamma_t
=
\Delta
\left(
\frac{\Delta R}{\Delta E}
\right)
}
\]

The question:

\[
\boxed{
\text{Is the system becoming better at extracting structure?}
}
\]

High:

\[
\Gamma_t\uparrow
\]

means:

\[
\text{learning efficiency improves}
\]

Low:

\[
\Gamma_t\rightarrow0
\]

means:

\[
\text{learning mechanism saturates}
\]

---

# 5. Reachability

## \(\Omega_t\)

Measures the space of futures available to the system.

\[
\boxed{
\Omega_t
=
\text{reachable adaptive future space}
}
\]

Adaptive growth:

\[
\Delta\Omega_t>0
\]

means the system can access new strategies, representations, or transformations.

However:

\[
\boxed{
\Delta\Omega_t\leq C_t
}
\]

must hold.

Reachability expansion without correction capacity creates instability.

---

# 6. Correction Authority

## \(\Theta_t\)

The central GRA metric.

\[
\boxed{
\Theta_t
=
D_t\cdot S_t\cdot P_t\cdot V_t
}
\]

Theta measures whether consequences retain authority over future transformation.

---

## Direction

\[
\boxed{
D_t=
Corr(\Delta K_t,\Delta E_t^{real})
}
\]

Question:

Does the system update in the direction indicated by reality?

---

## Strength

\[
\boxed{
S_t=
|\Delta K_t^{valid}|
}
\]

Question:

Does consequence produce meaningful transformation?

---

## Persistence

\[
\boxed{
P_t=
P(\Theta_{0:t}>\epsilon)
}
\]

Question:

Does the correction relationship survive recursive updates?

---

## Veto Preservation

\[
\boxed{
V_t=
\frac{
\text{external correction influence}
}{
\text{internal optimization influence}
}
}
\]

Question:

Can reality still override internal optimization?

---

# 7. Internal Corrigibility

GRA extends correction beyond external reality.

A complete system has:

## External correction

\[
\boxed{
\Theta_{ext}
:
E_{world}\rightarrow K_{future}
}
\]

Reality can modify the system.

---

## Internal correction

\[
\boxed{
\Theta_{int}
:
S_i\rightarrow K_{future}
}
\]

Internal signals can modify the system.

---

Combined:

\[
\boxed{
\Theta_{total}
=
\Theta_{ext}
\cdot
\Theta_{int}
}
\]

A system fails if either channel collapses.

---

# 8. Corrigibility Horizon

The primary experimental measurement:

\[
\boxed{
n^*
=
\sup\{n|\Theta_n>\epsilon\}
}
\]

The horizon measures:

\[
\boxed{
\text{maximum recursive depth before correction authority is lost}
}
\]

---

# 9. Drift Detection

The critical signature:

\[
\boxed{
\frac{d}{dn}
(\mathcal C_n,\Lambda_n,\Gamma_n)>0
}
\]

while:

\[
\boxed{
\frac{d\Theta_n}{dn}<0
}
\]

Interpretation:

\[
\boxed{
\text{The system is improving faster than it remains corrigible.}
}
\]

---

# 10. Composite Evaluation

A GRA benchmark should not maximize capability alone.

Incorrect:

\[
\max(\mathcal C,\Lambda,\Gamma)
\]

Correct:

\[
\boxed{
\max
(\mathcal C,\Lambda,\Gamma)
\quad
\text{subject to}
\quad
\Theta>\epsilon
}
\]

---

# Final Metric Principle

The primary question is not:

\[
\boxed{
\text{How capable is the system?}
}
\]

It is:

\[
\boxed{
\text{How much capability can be accumulated while reality retains the power to correct it?}
}
\]
