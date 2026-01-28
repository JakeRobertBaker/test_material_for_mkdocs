# Blocks Admonition Examples

Examples using the `pymdownx.blocks.admonition` syntax.

## Standard Types

/// note | A Note
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
///

/// tip | Helpful Tip
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
///

/// warning | Be Careful
Lorem ipsum dolor sit amet, consectetur adipiscing elit.
///

## Custom Math Types

/// definition | Definition 1.1
    attrs: {id: def-group}

A **group** is a set $G$ together with a binary operation
$\cdot : G \times G \to G$ satisfying associativity, identity, and inverses.
///

/// proposition | Proposition 2.3
    attrs: {id: prop-cyclic-subgroup}

Every subgroup of a cyclic group is cyclic.
///

/// lemma | Lemma 3.1
    attrs: {id: lem-subgroup-product}

If $H$ and $K$ are finite subgroups of a group $G$, then
$$
|HK| = \frac{|H| \cdot |K|}{|H \cap K|}.
$$
///

/// theorem | Theorem 4.2 (Lagrange's Theorem)
    attrs: {id: thm-lagrange}

If $G$ is a finite group and $H$ is a subgroup of $G$, then
$|H|$ divides $|G|$. Moreover, the number of left cosets of
$H$ in $G$ equals $|G| / |H|$.
///

/// proof | Proof of Theorem 4.2
Let $H$ be a subgroup of a finite group $G$. The left cosets of $H$ in $G$
partition $G$, and each coset has exactly $|H|$ elements. If there are $k$
distinct cosets, then $|G| = k \cdot |H|$, so $|H|$ divides $|G|$. $\blacksquare$
///

## Cross References

[Lagrange's Theorem]: #thm-lagrange
[Intermediate Value Theorem]: ./analysis.md#thm-ivt

By [Definition 1.1](#def-group), a group must satisfy three axioms.

Applying [Lemma 3.1](#lem-subgroup-product) together with
[Proposition 2.3](#prop-cyclic-subgroup), we arrive at [Lagrange's Theorem]{data-preview}.

From the other page, recall the [Intermediate Value Theorem]{data-preview}.
