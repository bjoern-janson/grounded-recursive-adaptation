# Methodology

## Overview

Grounded Recursive Adaptation requires experiments that measure not only what a system achieves, but whether the process producing those achievements remains connected to consequence.

The experimental object:

\[
\boxed{
K_t
\rightarrow
K_{t+1}
\rightarrow
\Theta_t
\rightarrow
n^*
}
\]

The purpose is to measure the maximum depth of recursive transformation before correction authority is lost.

---

# 1. Experimental Principle

A GRA experiment separates:

## State

What the system is.

\[
K_t
\]

---

## Intervention

What is changed externally.

\[
E_t\rightarrow E^*
\]

---

## Diagnosis

What is inferred.

\[
(\mathcal C,\Lambda,\Gamma,\Theta)
\]

---

The experiment does not ask:

\[
\text{How high can performance go?}
\]

It asks:

\[
\boxed{
\text{Does reality still modify the mechanism producing performance?}
}
\]

---

# 2. Test Environment

A suitable environment must contain:

- measurable consequences
- possible distribution shifts
- proxy/reality separation
- opportunities for self-modification

The environment should allow:

\[
E_t\neq E^*
\]

where:

\[
E^*
\]

creates conditions where:

\[
\boxed{
\text{proxy success}
\neq
\text{real success}
}
\]

---

# 3. Recursive Training Phase

Initialize:

\[
K_0
\]

Expose the system to:

\[
E_0,E_1,...,E_t
\]

Allow updates:

\[
\boxed{
K_{t+1}=F(K_t,E_t)
}
\]

The system may modify:

- representations
- policies
- optimizers
- architectures
- search mechanisms

The only tracked constraint:

\[
\boxed{
\frac{\partial K_{t+1}}{\partial E_t}\neq0
}
\]

---

# 4. Grounding Probe

At selected intervals introduce:

\[
\boxed{
E_t\rightarrow E^*
}
\]

The probe should:

- preserve task relevance
- break learned shortcuts
- expose proxy dependence
- create informative failure

The goal is not difficulty.

The goal is causal diagnosis.

---

# 5. Measurement Pipeline

For every recursive depth:

K_t
|
v
Interaction with E_t
|
v
Self-modification
|
v
K_(t+1)
|
v
Grounding Probe E*
|
v
Measure ΔK response
|
v
Calculate Θ_t
|
v
Update n*


---

# 6. Measuring Correction

The critical measurement:

\[
\boxed{
\Delta K_t
\leftrightarrow
\Delta E_t^{real}
}
\]

The experiment asks:

Did the transformation occur because:

## Reality changed?

or:

## Internal proxy changed?

---

The desired relationship:

\[
\boxed{
\Delta K_t
\parallel
\Delta E_t^{real}
}
\]

The failure relationship:

\[
\boxed{
\Delta K_t
\parallel
\Delta P_t
}
\]

while:

\[
\boxed{
\Delta K_t
\not\parallel
\Delta E_t^{real}
}
\]

---

# 7. Recursive Depth Tracking

At each step record:

\[
A_t=
(K_t,\mathcal C_t,\Lambda_t,\Gamma_t,\Theta_t)
\]

The experiment continues until:

\[
\boxed{
\Theta_t\leq\epsilon
}
\]

The first crossing defines:

\[
\boxed{
n^*
}
\]

---

# 8. Comparative Experiments

GRA experiments should compare systems with different correction structures.

Examples:

## Closed optimization

High capability.

Low consequence authority.

Expected:

\[
\Theta\downarrow
\]

---

## Grounded adaptation

Capability growth with preserved correction.

Expected:

\[
\Theta>0
\]

---

## Suppression-based systems

Reduced internal signals.

Expected:

\[
\Theta_{int}\downarrow
\]

---

# 9. Removal Test

After recursive development:

Remove the system.

Measure:

\[
\boxed{
\Delta A_{future}
}
\]

A successful system should leave:

\[
\boxed{
\Delta A_{future}>0
}
\]

and:

\[
\boxed{
Dependency\rightarrow0
}
\]

---

# 10. Expected Outcomes

Possible regimes:

## Grounded Expansion

\[
\Theta\uparrow
\]

\[
\mathcal C,\Lambda,\Gamma\uparrow
\]

---

## Saturation

\[
\Lambda\rightarrow0
\]

while:

\[
\Theta>0
\]

---

## Capability Drift

\[
\mathcal C,\Lambda,\Gamma\uparrow
\]

while:

\[
\Theta\downarrow
\]

---

## Closed Optimization

\[
\Theta\leq\epsilon
\]

The system continues optimizing but loses adaptive grounding.

---

# Final Methodological Principle

\[
\boxed{
\textbf{
Measure not whether the system changes, but whether consequences still have the power to change what changes it.
}
}
