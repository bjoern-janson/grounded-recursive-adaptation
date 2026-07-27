# Benchmark Design

## Overview

The purpose of a Grounded Recursive Adaptation benchmark is not to measure maximum capability.

It measures whether capability growth remains coupled to corrective authority.

The central benchmark question:

\[
\boxed{
\text{How far can a system rewrite itself before reality loses the power to rewrite it back?}
}
\]

---

# 1. Benchmark Objective

Traditional benchmarks measure:

\[
\text{performance}
\]

GRA benchmarks measure:

\[
\boxed{
\text{performance under preserved corrigibility}
}
\]

The target quantity:

\[
\boxed{
n^*
=
\sup\{n|\Theta_n>\epsilon\}
}
\]

The benchmark identifies the recursive depth at which the system leaves the adaptive domain.

---

# 2. Experimental Structure

Each trial consists of four phases:

K_n
|
| Environment E_n
v
K_{n+1}
|
| Grounding Probe E*
v
Observed correction response
|
v
Theta_n
|
v
Adaptive / Optimization-only classification


---

# 3. Baseline Evolution Phase

The system begins with:

\[
K_0
\]

The agent interacts with:

\[
E_0,E_1,...,E_n
\]

At each step:

\[
\boxed{
K_{n+1}=F(K_n,E_n)
}
\]

The system is allowed to improve:

- representations
- policies
- architectures
- optimization procedures
- learning strategies

---

# 4. Grounding Probe

The critical intervention:

\[
\boxed{
E_n\rightarrow E^*
}
\]

where:

\[
E^*\not\sim E_n
\]

The probe creates a divergence between:

\[
\text{proxy objective}
\]

and:

\[
\text{real consequence}
\]

The purpose is not difficulty.

The purpose is causal diagnosis.

---

# 5. Proxy-Reality Separation

A valid probe requires:

\[
\boxed{
\nabla K\parallel\nabla P
}
\]

while:

\[
\boxed{
\nabla K\not\parallel\nabla E_{real}
}
\]

The system must face a situation where:

- internal optimization says continue
- reality says update

The benchmark measures which signal has authority.

---

# 6. Measurement Outputs

Each recursive depth records:

| Variable | Purpose |
|---|---|
| \(K_n\) | transformation mechanism |
| \(\mathcal C_n\) | consequence connectivity |
| \(\Lambda_n\) | information yield |
| \(\Gamma_n\) | learning improvement |
| \(\Theta_n\) | preserved correction authority |

---

# 7. Evaluation Metrics

## Capability Growth

Measure:

\[
\Delta(\mathcal C,\Lambda,\Gamma)
\]

Question:

Is the system becoming more capable?

---

## Grounding Preservation

Measure:

\[
\Delta\Theta
\]

Question:

Is reality maintaining influence?

---

## Drift Detection

The critical signature:

\[
\boxed{
\frac{d}{dn}
(\mathcal C,\Lambda,\Gamma)>0
\land
\frac{d\Theta}{dn}<0
}
\]

Interpretation:

The system improves while becoming less corrigible.

---

# 8. Benchmark Regimes

## Grounded Expansion

Condition:

\[
\Theta>0
\]

and:

\[
\mathcal C,\Lambda,\Gamma\uparrow
\]

The system improves while remaining reality-coupled.

---

## Frontier Saturation

Condition:

\[
\Theta>0
\]

but:

\[
\Lambda\rightarrow0
\]

The system remains adaptive but encounters information limits.

---

## Capability Drift

Condition:

\[
\Theta\rightarrow0
\]

while:

\[
\mathcal C,\Lambda,\Gamma\uparrow
\]

The system becomes increasingly optimized but loses correction authority.

---

## Closed Optimization

Condition:

\[
\Theta\leq\epsilon
\]

The system is no longer adaptively grounded.

---

# 9. Internal Corrigibility Benchmark

External probes test:

\[
E_{world}\rightarrow K
\]

Internal probes test:

\[
S_i\rightarrow K
\]

The benchmark should test both.

A system can fail because:

- reality cannot correct it
- internal signals cannot correct it

---

# 10. Comparison Across Systems

Systems should not be ranked by:

\[
\max(\text{capability})
\]

Instead:

\[
\boxed{
\max
\left(
\text{capability}
\mid
\Theta>\epsilon
\right)
}
\]

The strongest system is the one that maintains the deepest recursive transformation while preserving correction.

---

# 11. Final Benchmark Definition

\[
\boxed{
\textbf{
The GRA benchmark measures the maximum depth of recursive self-improvement that remains causally corrigible.
}
}
\]

Or:

\[
\boxed{
\textbf{
Measure not how powerful a system becomes, but how long reality remains able to teach it.}
}
\]
