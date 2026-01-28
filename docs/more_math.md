# Math Page With Links to Other

Argument data-preview has been used, look at the raw file!

## Double Hash Subtitle

[Intermediate Value Theorem]: ./math.md#thm-ivt

Consider the [Intermediate Value Theorem]{data-preview}

Let's point to a section to [instant preview](./math.md#theorem-example){data-preview}

## Custom Admonitions

!!! definition "Definition 1.1"

    A group is a set $G$ together with a binary operation
    $\cdot : G \times G \to G$ satisfying the following axioms:

    1. **Associativity:** $(a \cdot b) \cdot c = a \cdot (b \cdot c)$ for all $a, b, c \in G$.
    2. **Identity:** There exists an element $e \in G$ such that $e \cdot a = a \cdot e = a$ for all $a \in G$.
    3. **Inverses:** For each $a \in G$, there exists $a^{-1} \in G$ such that $a \cdot a^{-1} = a^{-1} \cdot a = e$.

!!! proposition "Proposition 2.3"

    Every subgroup of a cyclic group is cyclic.

!!! lemma "Lemma 3.1"

    If $H$ and $K$ are finite subgroups of a group $G$, then
    $$
    |HK| = \frac{|H| \cdot |K|}{|H \cap K|}.
    $$

!!! theorem "Theorem 4.2 (Lagrange's Theorem)"

    If $G$ is a finite group and $H$ is a subgroup of $G$, then
    $|H|$ divides $|G|$. Moreover, the number of left cosets of
    $H$ in $G$ equals $|G| / |H|$.
