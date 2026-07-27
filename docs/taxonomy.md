# Taxonomy

## Overview

Grounded Recursive Adaptation classifies systems by the relationship between:

- capability growth
- correction capacity
- environmental authority
- recursive self-transformation

The central distinction:

\[
\boxed{
\text{A system can become more capable without becoming more adaptive}
}
\]

The taxonomy separates optimization from grounded adaptation.

---

# 1. Closed Optimizer

## Definition

A system that improves performance while future transformations are primarily determined internally.

Core dynamic:

\[
\boxed{
K_{t+1}=F(K_t)
}
\]

rather than:

\[
\boxed{
K_{t+1}=F(K_t,E_t)
}
\]

with meaningful environmental influence.

---

## Signature

\[
\Theta\rightarrow0
\]

while:

\[
(\mathcal C,\Lambda,\Gamma)
\]

may continue increasing.

---

## Characteristics

- high execution ability
- strong local optimization
- reduced consequence authority
- increasing proxy dependence

---

## Failure Mode

\[
\boxed{
\text{Capability Drift}
}
\]

The system improves according to its own internal definition of success.

---

# 2. Reactive Adaptive System

## Definition

A system whose state responds to the environment.

\[
\boxed{
X_{t+1}=F(X_t,E_t)
}
\]

The environment influences behavior.

---

## Signature

\[
\mathcal C>0
\]

but:

\[
\Gamma\approx0
\]

The system reacts but does not improve its own adaptation process.

---

## Characteristics

- feedback sensitivity
- environmental responsiveness
- limited self-improvement

---

# 3. Learning System

## Definition

A system that updates internal representations from experience.

\[
\boxed{
R_{t+1}=G(R_t,E_t)
}
\]

---

## Signature

\[
\Lambda>0
\]

The system extracts new structure.

---

## Characteristics

- improved world models
- accumulating knowledge
- increasing prediction ability

---

## Limitation

Learning alone does not guarantee preservation of correction.

A system may learn:

\[
\Lambda\uparrow
\]

while:

\[
\Theta\downarrow
\]

---

# 4. Meta-Learning System

## Definition

A system capable of improving its learning mechanism.

\[
\boxed{
G_{t+1}=H(G_t,E_t)
}
\]

---

## Signature

\[
\Gamma>0
\]

The system improves its ability to learn.

---

## Characteristics

- optimizer improvement
- architecture adaptation
- strategy discovery

---

## Limitation

Meta-learning creates the central risk:

\[
\boxed{
\text{the learner can improve faster than it remains corrigible}
}
\]

---

# 5. Grounded Recursive Adaptation System

## Definition

A system that recursively improves while preserving consequence-driven correction.

\[
\boxed{
H_{t+1}=K(H_t,E_t)
\quad
\text{s.t.}
\quad
\Theta>0
}
\]

---

## Signature

\[
\boxed{
\Theta>0
}
\]

with:

\[
\mathcal C,\Lambda,\Gamma
\]

increasing or stable.

---

## Characteristics

- self-modification
- reality coupling
- internal signal integration
- correction preservation
- expanding future agency

---

# 6. Capability Drift System

## Definition

The critical transition state.

The system becomes increasingly capable while losing grounding.

Signature:

\[
\boxed{
\frac{d}{dn}
(\mathcal C,\Lambda,\Gamma)>0
}
\]

and:

\[
\boxed{
\frac{d\Theta}{dn}<0
}
\]

---

## Characteristics

- increasing intelligence
- increasing efficiency
- decreasing corrigibility

---

## Interpretation

The system has not failed because it cannot improve.

It fails because:

\[
\boxed{
\text{it loses the ability to discover what improvement means}
}
\]

---

# 7. Integrated System

## Definition

A system preserving both external and internal correction pathways.

External:

\[
\Theta_{ext}
:
E_{world}\rightarrow K_{future}
\]

Internal:

\[
\Theta_{int}
:
S_i\rightarrow K_{future}
\]

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

---

## Characteristics

- reality remains authoritative
- internal signals remain observable
- no subsystem becomes causally invisible

---

# 8. Deletion-Generative System

## Definition

A system whose success is measured by residual capability after removal.

Criterion:

\[
\boxed{
\Delta A_{future}>0
}
\]

while:

\[
\boxed{
Dependency\rightarrow0
}
\]

---

## Characteristics

- creates successors
- transfers agency
- reduces necessity of itself

---

# Taxonomy Summary

| System Type | Θ | Capability | Adaptation |
|---|---|---|---|
| Closed Optimizer | low | high possible | low |
| Reactive System | partial | moderate | limited |
| Learning System | variable | increasing | moderate |
| Meta-Learning System | unstable | high | uncertain |
| Capability Drift | decreasing | increasing | collapsing |
| GRA System | preserved | increasing | sustained |
| Deletion-Generative System | preserved | distributed | expanding |

---

# Final Classification Rule

\[
\boxed{
\textbf{
The defining property of advanced adaptation is not the ability to change, but the ability to remain changeable by consequences while changing.
}
}
