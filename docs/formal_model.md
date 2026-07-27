# Formal Model

## Overview

Grounded Recursive Adaptation models systems that recursively modify their own transformation processes while remaining coupled to environmental consequences.

The central object is not the system state alone.

It is the relationship:

\[
\boxed{
E_t \rightarrow K_{t+1}
}
\]

where reality maintains causal influence over future transformation.

---

# 1. System Definition

A recursively adapting system is represented as:

\[
\boxed{
S_t=(X_t,K_t,R_t,\Omega_t)
}
\]

where:

- \(X_t\) = system state
- \(K_t\) = transformation mechanism
- \(R_t\) = internal representation
- \(\Omega_t\) = reachable future space

---

# 2. Recursive Dynamics

The state transition:

\[
\boxed{
X_{t+1}=F(X_t,K_t,E_t)
}
\]

The transformation mechanism updates:

\[
\boxed{
K_{t+1}=G(K_t,E_t)
}
\]

The defining property of recursive adaptation:

\[
\boxed{
G \text{ itself is subject to change}
}
\]

The system does not merely learn.

It changes how it learns.

---

# 3. The Grounding Constraint

The adaptive condition:

\[
\boxed{
\frac{\partial K_{t+1}}{\partial E_t}\neq0
}
\]

means:

Environmental consequences influence future transformation.

The system remains grounded while:

\[
\boxed{
\Theta_t(K_t,E_t)>\epsilon
}
\]

---

# 4. Theta Function

Theta measures preserved causal authority.

A general form:

\[
\boxed{
\Theta_t
=
D_t
\cdot
S_t
\cdot
P_t
\cdot
V_t
}
\]

where:

---

## Direction

\[
D_t=
Corr(\Delta K_t,\Delta E_t^{real})
\]

Does the system change in response to actual consequences?

---

## Strength

\[
S_t=
|\Delta K_t^{valid}|
\]

Does consequence produce meaningful transformation?

---

## Persistence

\[
P_t=
P(\Theta_{0:t}>\epsilon)
\]

Does the correction relationship survive recursion?

---

## Veto Preservation

\[
V_t=
\frac{
\text{external correction influence}
}{
\text{internal optimization influence}
}
\]

Does reality retain authority over optimization?

---

# 5. Capability Space

Capability is measured independently:

\[
\boxed{
A_t=(\mathcal C_t,\Lambda_t,\Gamma_t)
}
\]

---

## Consequence Connectivity

\[
\boxed{
\mathcal C_t=
I(\Delta A_t;\Delta E_t)
}
\]

Measures action-consequence coupling.

---

## Information Yield

\[
\boxed{
\Lambda_t=
D_{KL}(R_{t+1}\parallel R_t)
}
\]

Measures representational change.

---

## Learning Improvement

\[
\boxed{
\Gamma_t=
\Delta
\left(
\frac{\Delta R}{\Delta E}
\right)
}
\]

Measures improvement of the learning process itself.

---

# 6. Adaptive Validity Predicate

Theta determines the semantic interpretation of capability:

\[
\boxed{
\Theta_t(K_t,E_t)
\vdash
(\mathcal C_t,\Lambda_t,\Gamma_t):
\begin{cases}
Adaptive & \Theta_t>\epsilon\\
Optimization & \Theta_t\leq\epsilon
\end{cases}
}
\]

The measurements remain identical.

The meaning changes.

---

# 7. Reachability Dynamics

Adaptive systems modify their future possibility space.

The genome:

\[
\boxed{
R\rightarrow\Omega\rightarrow C\rightarrow A\rightarrow R'
}
\]

where:

- \(R\) extracts structure
- \(\Omega\) determines reachable futures
- \(C\) applies correction
- \(A\) improves adaptation

The key constraint:

\[
\boxed{
\Delta\Omega\leq C
}
\]

Reachable futures must not expand faster than correction capacity.

---

# 8. Adaptive Mechanism Space

The recursive hierarchy:

\[
\boxed{
X\rightarrow F\rightarrow G\rightarrow\mathcal G
}
\]

where:

- \(X\) = state
- \(F\) = transformation
- \(G\) = transformation-selection mechanism
- \(\mathcal G\) = space of possible adaptive mechanisms

The deepest recursion:

\[
\boxed{
\Omega_t\rightarrow\Delta\mathcal G_{t+1}
}
\]

Information changes not only actions.

It changes which adaptation mechanisms are reachable.

---

# 9. Corrigibility Horizon

The maximum recursive depth:

\[
\boxed{
n^*
=
\sup
\{n|\Theta_n>\epsilon\}
}
\]

defines the boundary:

\[
\boxed{
\text{recursive adaptation}
\rightarrow
\text{closed optimization}
}
\]

---

# 10. Final Formal Statement

\[
\boxed{
\textbf{
A recursively self-modifying system remains adaptive only while environmental and internal consequences retain causal authority over future transformations.
}
}
\]

Minimal form:

\[
\boxed{
\textbf{
Adaptation is change that reality can still correct.}
}
\]
