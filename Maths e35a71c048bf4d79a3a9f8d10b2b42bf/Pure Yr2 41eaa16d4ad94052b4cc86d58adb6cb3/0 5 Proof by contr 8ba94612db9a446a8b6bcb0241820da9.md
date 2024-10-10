# 0.5. Proof by contr

**Proof by contradiction** is a technique you can use to prove statements. The way it works is you assume the *negation* of the statement is true, then show that doing that contradicts itself, and that therefore the original statement must be true.

The simplest example of this is “Prove there is no greatest odd integer”:

1. Assume there is a greatest odd integer, **`n`**
2. Consider `n + 2` 
    1. `n + 2` is odd 
    2. But `n + 2 > n` 
3. Therefore there is no greatest odd integer.

Some of the simpler proofs you can just come up with, like prove that if $n^2$ is even, that $n$ must also be even.

# Rational numbers

One very common thing you’ll find are proofs questioning the rationality of something. For these, you need to say that anything that’s rational can be rewritten as:

$$
n \equiv \frac{a}{b}
$$

With the following two conditions: 

1. `a` and `b` must be integers
2. `a` and `b` must share no common factors

You don’t always need to write both these conditions, and usually #2 is only useful for the root complex proofs below, but make sure you know the conditions are there.

# Complex proofs

Some of the more extreme proofs requires some serious creativity and aren’t something you can exactly come up with on the spot in the exam, so for those you really just have to remember the general process, there are three examples that come to mind that are a little out there:

1. Prove that $\sqrt{x}$ is irrational
2. Prove there are no integer solutions to $x^2-y^2=2$
3. Prove there are infinitely many primes

## Prove that $\sqrt{x}$ is irrational (g iven constant x)

Assume that $\sqrt{x}$  is rational number, $\frac{a}b$.

**Arrangement:**

1. Rearrange it into $\frac{a^2}{b^2} = x$.
2. Rearrange that into  $a^2 = xb^2$.
3. Determine that $a^2$ and by extension $a$ has the factor $x$ and use it to rewrite `a`
4. After rewriting it, determine that $b^2$ also has the factor $x$.

**Contradiction:**

They both share common factors, but $\frac{a}{b}$ cannot have common factors between the top and bottom variables.

## Prove there are no integer solutions to $x^2-y^2=2$

Assume there are integer solutions

**Arrangement:**

1. Use *difference of two squares* to simplify the LHS into two multiplications.
2. Figure out the different pairs of values each half of the multiplication can have to give 2
3. Show with simultaneous equations that in none of these scenarios both $x$ and $y$ integers.

**Contradiction:**

In no scenario are $x$ or $y$ integers, so there are no integer solutions.

## There are infinitely many primes

Assume *there is a finite number of primes*.

**Arrangement**:

1. Consider a list of every prime, $p_1, p_2...p_n$ 
2. **Then consider $N = (p_1*p_2...*p_n) + 1$**

**Contradiction:**

If you divide N by *any* of these prime numbers, it’ll always give a remainder of 1. This means it doesn’t have a single prime factor and therefore that it itself is prime. But $N$ is not in the list.