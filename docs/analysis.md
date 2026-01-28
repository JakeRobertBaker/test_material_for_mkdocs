# Real Analysis

## Foundational Definitions

/// definition | Definition 1.1 (Continuity)
    attrs: {id: def-continuous}

A function $f: \mathbb{R} \to \mathbb{R}$ is **continuous** at a point $a$ if
for every $\varepsilon > 0$ there exists $\delta > 0$ such that
$$
|x - a| < \delta \implies |f(x) - f(a)| < \varepsilon.
$$
///

/// definition | Definition 1.2 (Bounded)
    attrs: {id: def-bounded}

A function $f: D \to \mathbb{R}$ is **bounded** on $D$ if there exists $M > 0$
such that $|f(x)| \leq M$ for all $x \in D$.
///

## Key Results

/// lemma | Lemma 2.1 (Boundedness Lemma)
    attrs: {id: lem-bounded}

If $f$ is continuous on a closed interval $[a,b]$, then $f$ is bounded on $[a,b]$.
///

/// theorem | Theorem 2.2 (Extreme Value Theorem)
    attrs: {id: thm-evt}

If $f$ is continuous on $[a,b]$, then $f$ attains its maximum and minimum on $[a,b]$.
That is, there exist $c, d \in [a,b]$ such that $f(c) \leq f(x) \leq f(d)$
for all $x \in [a,b]$.
///

/// theorem | Theorem 2.3 (Intermediate Value Theorem)
    attrs: {id: thm-ivt}

If $f$ is continuous on $[a,b]$ and $f(a) \neq f(b)$, then for every value $y$
between $f(a)$ and $f(b)$, there exists $c \in (a,b)$ such that $f(c) = y$.
///

## Cross References

[Lagrange's Theorem]: ./blocks_admonition_example.md#thm-lagrange
[Definition 1.1]: ./blocks_admonition_example.md#def-group

By [Definition 1.1 (Continuity)](#def-continuous) and
[Lemma 2.1](#lem-bounded), a continuous function on a closed interval is bounded.

The [Extreme Value Theorem](#thm-evt){data-preview} strengthens this further.

The [Intermediate Value Theorem](#thm-ivt){data-preview} is a cornerstone of
real analysis.

From the algebra page, see [Lagrange's Theorem]{data-preview} and
[Definition 1.1]{data-preview} of a group.
