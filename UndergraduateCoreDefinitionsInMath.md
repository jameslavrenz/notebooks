
# Undergraduate Core Definitions in Analysis, Topology, and Algebra

---

# 1. Real Analysis

## Limits of Sequences

A sequence $(a_n)$ converges to $L \in \mathbb{R}$ if

$$
\forall \varepsilon > 0,\ \exists N \in \mathbb{N} \text{ such that } n \ge N \Rightarrow |a_n - L| < \varepsilon.
$$

---

## Limits of Functions

$$
\lim_{x \to a} f(x) = L
$$

if

$$
\forall \varepsilon > 0,\ \exists \delta > 0 \text{ such that } 0 < |x-a| < \delta \Rightarrow |f(x)-L| < \varepsilon.
$$

---

## Continuity

A function $f: \mathbb{R} \to \mathbb{R}$ is continuous at $a$ if

$$
\lim_{x \to a} f(x) = f(a).
$$

---

## Uniform Continuity

$f$ is uniformly continuous on $A$ if

$$
\forall \varepsilon > 0,\ \exists \delta > 0 \text{ such that } |x-y| < \delta \Rightarrow |f(x)-f(y)| < \varepsilon \quad \forall x,y \in A.
$$

---

## Cauchy Sequence

A sequence $(a_n)$ is Cauchy if

$$
\forall \varepsilon > 0,\ \exists N \text{ such that } m,n \ge N \Rightarrow |a_n - a_m| < \varepsilon.
$$

---

## Completeness

A metric space is complete if every Cauchy sequence converges in the space.

---

## Supremum

$s = \sup A$ if:

- $a \le s$ for all $a \in A$
- $\forall \varepsilon > 0,\ \exists a \in A$ such that $s - \varepsilon < a$

---

## Differentiability

$f$ is differentiable at $a$ if

$$
f'(a) = \lim_{h \to 0} \frac{f(a+h)-f(a)}{h}
$$

exists.

---

# 2. Topology

## Topological Space

A pair $(X,\tau)$ where $\tau \subseteq \mathcal{P}(X)$ such that:

1. $\emptyset, X \in \tau$
2. Arbitrary unions of elements of $\tau$ are in $\tau$
3. Finite intersections of elements of $\tau$ are in $\tau$

---

## Interior

$$
\operatorname{int}(A) = \bigcup \{U \subseteq A : U \text{ open}\}
$$

---

## Closure

$$
\overline{A} = \bigcap \{F \supseteq A : F \text{ closed}\}
$$

---

## Boundary

$$
\partial A = \overline{A} \setminus \operatorname{int}(A)
$$

---

## Basis

A collection $\mathcal{B}$ is a basis if:

- Every $x \in X$ lies in some $B \in \mathcal{B}$
- If $x \in B_1 \cap B_2$, then $\exists B_3 \subseteq B_1 \cap B_2$ with $x \in B_3$

---

## Continuity

$f: X \to Y$ is continuous if

$$
f^{-1}(U) \text{ is open in } X \text{ for all open } U \subseteq Y.
$$

---

## Homeomorphism

A bijection $f: X \to Y$ such that both $f$ and $f^{-1}$ are continuous.

---

## Compactness

Every open cover has a finite subcover.

---

## Connectedness

Cannot be written as union of two disjoint nonempty open sets.

---

# 3. Abstract Algebra

## Group

A set $G$ with operation $\cdot$ such that:

- $(ab)c = a(bc)$
- $\exists e \in G$ such that $ae = ea = a$
- $\forall a \in G,\ \exists a^{-1}$
- Closure: $ab \in G$

---

## Abelian Group

$$
ab = ba \quad \forall a,b \in G
$$

---

## Subgroup

$H \le G$ if $H \subseteq G$ and $H$ is a group.

---

## Cyclic Group

$$
G = \langle g \rangle = \{g^n : n \in \mathbb{Z}\}
$$

---

## Homomorphism

$$
f(ab) = f(a)f(b)
$$

---

## Kernel

$$
\ker(f) = \{g \in G : f(g) = e_H\}
$$

---

## Ring

A set $R$ with $+$ and $\cdot$ such that:

- $(R,+)$ is an abelian group
- multiplication is associative
- distributive laws hold

---

## Field

A commutative ring where every nonzero element has an inverse.

---

## Vector Space

A set $V$ over field $F$ such that:

- $(V,+)$ is an abelian group
- scalar multiplication $F \times V \to V$ satisfies axioms

---

## Linear Independence

$$
\sum a_i v_i = 0 \Rightarrow a_i = 0
$$

---

## Basis

A linearly independent spanning set.

---

## Dimension

Number of vectors in a basis.

---

## Ideal

$I \subseteq R$ such that:

- additive subgroup
- $rI \subseteq I$

---

## Quotient

Equivalence classes under subgroup or ideal.

---

# End of File