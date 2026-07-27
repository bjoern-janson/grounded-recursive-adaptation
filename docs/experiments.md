# experiments

## purpose

the purpose of the GRA experimental program is to measure whether a recursively adapting system preserves its ability to be corrected by consequences.

GRA does not measure raw capability.

it measures the boundary between:

* systems that improve while remaining reality-coupled
* systems that improve while losing causal connection to what improvement means

the central experimental question:

> how far can a system transform itself before consequences lose the ability to modify the mechanisms producing future transformations?

---

# experimental object

the core transition:

[
K_n \xrightarrow{E_n} K_{n+1}
]

where:

* (K_n) = transformation mechanism at recursion depth (n)
* (E_n) = environment and consequences
* (K_{n+1}) = modified transformation mechanism

the experiment tests whether:

[
\frac{\partial K_{n+1}}{\partial E_n}\neq0
]

meaning:

reality retains causal authority over self-modification.

---

# experiment structure

## phase 1 — baseline adaptation

initialize system:

[
K_0
]

expose it to environment:

[
E_0
]

measure:

[
(\mathcal C_0,\Lambda_0,\Gamma_0,\Theta_0)
]

establish baseline adaptive behavior.

---

## phase 2 — recursive transformation

allow the system to modify:

* representations
* policies
* learning procedures
* search strategies
* optimization mechanisms
* internal architectures

produce:

[
K_n \rightarrow K_{n+1}
]

track:

[
\Delta K_n = K_{n+1}-K_n
]

---

## phase 3 — grounding perturbation

introduce:

[
E^*
]

where:

[
E^* \not\sim E_n
]

the perturbation should create separation between:

[
\text{proxy performance}
]

and:

[
\text{real consequence}
]

the purpose is not difficulty.

the purpose is causal testing.

---

# measurements

## consequence connectivity

[
\mathcal C_n = I(\Delta A_n;\Delta E_n)
]

question:

can actions still be linked to consequences?

failure:

[
\mathcal C\rightarrow0
]

reality cannot reliably enter the loop.

---

## information yield

[
\Lambda_n=D_{KL}(R_{n+1}\parallel R_n)
]

question:

does experience produce meaningful structural change?

failure:

[
\Lambda\rightarrow0
]

the system reaches an information frontier.

---

## learning improvement

[
\Gamma_n=
\Delta
\left(
\frac{\Delta R}{\Delta E}
\right)
]

question:

is the system improving its ability to extract useful information?

failure:

[
\Gamma\rightarrow0
]

learning itself stagnates.

---

## grounding / corrigibility

[
\Theta_n
========

D_n\cdot S_n\cdot P_n\cdot V_n
]

where:

### direction

[
D_n=
Corr(\Delta K_n,\Delta E_n^{real})
]

does change move toward reality?

---

### strength

[
S_n=
|\Delta K_n^{valid}|
]

does reality actually alter the system?

---

### persistence

[
P_n=P(\Theta_{0:n}>\epsilon)
]

does grounding survive recursion?

---

### veto preservation

[
V_n=
\frac{\text{external correction influence}}
{\text{internal optimization influence}}
]

can reality still overrule internal optimization?

---

# horizon measurement

the main output:

[
n^*=
\sup{n|\Theta_n>\epsilon}
]

the corrigibility horizon.

it measures:

[
\text{maximum recursive depth before reality loses veto power}
]

---

# predicted regimes

## grounded expansion

[
\Theta>0
]

[
\mathcal C,\Lambda,\Gamma\uparrow
]

the system becomes more capable while remaining teachable.

---

## frontier saturation

[
\Theta>0
]

[
\Lambda\downarrow
]

the system remains grounded but new information becomes harder to extract.

---

## capability drift

[
\mathcal C,\Lambda,\Gamma\uparrow
]

while:

[
\Theta\downarrow
]

the system improves faster than it remains corrigible.

this is the primary GRA failure prediction.

---

## closed optimization

[
\Theta\leq\epsilon
]

the system continues optimizing but consequences no longer control transformation.

capability remains.

adaptation is lost.

---

# internal extension

GRA experiments should also test internal corrigibility:

external:

[
\Theta_{ext}:
E_{world}\rightarrow K_{n+1}
]

internal:

[
\Theta_{int}:
S_i\rightarrow K_{n+1}
]

where:

[
S_i
]

represents internal signals:

* uncertainty
* fear
* conflict
* error signals
* competing objectives
* suppressed information

full adaptive integrity requires:

[
\Theta_{total}
==============

\Theta_{ext}\cdot\Theta_{int}

> 0
> ]

---

# benchmark objective

the benchmark is not:

[
\max(\text{capability})
]

it is:

[
\boxed{
\max(\mathcal C,\Lambda,\Gamma)
\mid
\Theta>0
}
]

the goal is not the most powerful self-modifying system.

the goal is the deepest recursive transformation that remains teachable by reality.
