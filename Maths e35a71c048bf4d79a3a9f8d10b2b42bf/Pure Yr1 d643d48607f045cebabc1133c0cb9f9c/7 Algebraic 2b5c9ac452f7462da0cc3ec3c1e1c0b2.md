# 7. Algebraic

# Polynomials

A **polynomial** is an expression made up of **multiple** terms and can contain constants, variables and **positive integer exponents**. Anything else will cause it to not be a polynomial. So you can't have fractional exponents.

<aside>
🖊️ **Poly** means "many" and **nomial** means terms. So it's literally "many-terms"!

</aside>

For example, this is a polynomial, nothing in it is outside of the allowing items:

$$
7x^2 + 3xy + 5
$$

But this is not a polynomial:

$$
\sqrt{x} + 3xy
$$

<aside>
💡 You can actually prove this by rewriting the $\sqrt{x}$ as $x^{\frac{1}{2}}$, which is not a positive integer exponent.

</aside>

> When you have a polynomial, the **highest index** is known as the **degree**.
> 

# Dividing Polynomials

The easiest way to divide polynomials is just by the cancellation. For example, if you have the following expression:

$$
\frac{x^2 + 3x - 4}{x - 1}
$$

You can factorise the top and cancel as needed. However, if you have a numerator that's a lot more complex, then you use a long division-like method.

It's quite a lengthy process but it follows a few simple steps.

1. Draw a "bus stop"-like shape, as you do for division, like so:
    
    $$
    \begin{array}{l} x-3\space \overline{\big)\,x^3+x^2-7x-15} \end{array}
    $$
    
2. Divide the first term by the `x` and place it above:
    
    $$
    \begin{array}{l} \phantom{x-3((} x^2 \\ x-3\space{\overline{\big)x^3+x^2-7x-15}} \end{array}
    $$
    
3. Now multiply our ***answer*** value from step #2 above by the denominator, like so:
    
    $$
    \begin{array}{l} \phantom{x-3((} \red{x^2} \\ \red{x-3}\space{\overline{\big)x^3+x^2-7x-15}} \\ \phantom{x-3((} \green{x^3 - 3x^2} \end{array}
    $$
    
4. Now, what we want to do is for our new expression to cancel out the expression above it, we can do it by subtracting it away, and simply evaluating that after.
    
    $$
    \begin{array}{l} \phantom{x-3((} x^2 \\ x-3\space{\overline{\big)x^3+x^2-7x-15}} \\ \phantom{x-} -\space\space x^3 - 3x^2 \\ \phantom{--} \overline{\phantom{---(} 4x^2} \end{array}
    $$
    
    <aside>
    ⚠️ **NOTE:** Be very careful when subtracting. You're doing $x^2--\space3x^2$, which makes $4x^2$
    
    </aside>
    
5. Bring the $7x$ down and add it after the $4x^2$
    
    $$
    \begin{array}{l} \phantom{x-3((} x^2 \\ x-3\space{\overline{\big)x^3+x^2-7x-15}} \\ \phantom{x-} -\space\space x^3 - 3x^2 \\ \phantom{--} \overline{\phantom{---(} \red{4x^2}} \red{- 7x} \end{array}
    $$
    
6. Repeat the process for the term in red, as if it was at the start.

In the end, you should get `0` when you subtract the very last two things. If you don't, that's the remainder of the expression.

One way to remember this process is to describe it as **Divide - Multiply - Subtract - Pull.** You **divide** the current term by the `x`, and use that as your answer on top, then you then you **multiply** the result from that by the denominator, then you **subtract** those two, and then you **pull** the next term in and repeat.

<aside>
🖊️ It spells out **DMSP,** and Beatrice likes "Dream SMP", so use that to remember it!

</aside>

You can also apply this method for $2x+1$. This isn't much different, you just need to divide each bit by `2x` now instead of just `x`.

When you're doing this process, **make sure** the powers of each term in the polynomial are all decreasing, it **won't work otherwise.** So, if you're asked to do:

$$
\frac{x^3+x+10}{x+2}
$$

You should add the $x^2$ in before trying to do long division.

## The Factor Theorem

The **factor theorem** says that if $f(p) = 0$, where $f(x)$ is a polynomial, then $(x-p)$ is a factor of said polynomial. Remember that it's a subtraction in there, and not an addition. You can remember it is because you tried once as if the rule was $(x+p)$ and it didn't work.

So, if you're asked to show that $(x-  2)$ is a factor of $f ( x) = x^3+ x^2 - 4x - 4$, substitute in `p`, which is `2`, and if it gives `0`, then it is a factor.

<aside>
🖊️ Make sure to write a **conclusion,** if you're asked to *show* that.

</aside>

### Factorising anything

You can use this, combined with factor theorem, to factorize **anything**. What you need to do is *brute-force* one of the terms via factor theorem. Then, once you’ve done that, you’ll *have* one of the possible terms, and you can then *divide* the whole equation by that.

# Proofs

A **proof** is an argument to show that a conjecture is true. A **conjecture** is an unproven statement, while a proven statement is known as a **theorem.** 

When creating proof, you should start with a*lready established facts*, and then use those through a series of logical steps. And at the end, you can **state** what's been proven.

## Proof by deduction

This is where you use *known facts* and use logical steps to reach the conclusion you're after.

- **Identities**
    
    If you're given an identity, you should get both sides *looking* the same, don't try to solve it!
    
- **Is multiple of**
    
    If you're asked to show that something is the multiple of another thing, you need to be able to rearrange the thing such that you can **factorise** by `20`, and that will prove it.
    

## Proof by exhaustion

This is where you break a conjecture into smaller cases and show each case separately. This can also be used to **disprove** a statement, just, well, give an example where it doesn't work.