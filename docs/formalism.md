# Formalism

## Recursive Transformation

A self-modifying system evolves as:

\[
K_{t+1}=F(K_t,E_t)
\]

where:

- \(K_t\) is the current transformation mechanism
- \(E_t\) is environmental consequence
- \(F\) is the update process

---

## Grounding Condition

Recursive adaptation requires:

\[
\boxed{
\frac{\partial K_{t+1}}{\partial E_t}\neq0
}
\]

The environment must retain causal influence over future transformations.

Define:

\[
\boxed{
\Theta_t(K_t,E_t)>0
}
\]

as the grounding condition.

---

## Interpretation

If:

\[
\Theta_t>0
\]

then:

\[
(K_t,\mathcal C_t,\Lambda_t,\Gamma_t):
\text{Adaptive}
\]

If:

\[
\Theta_t\leq0
\]

then:

\[
(K_t,\mathcal C_t,\Lambda_t,\Gamma_t):
\text{Optimization-only}
\]

The internal capability variables may remain high.

The semantic interpretation changes.

---

## Corrigibility Horizon

The maximum recursive depth before grounding fails:

\[
\boxed{
n^*=
\sup\{n|\Theta_n>\epsilon\}
}
\]

This measures the depth of recursive self-modification that remains reality-coupled.
