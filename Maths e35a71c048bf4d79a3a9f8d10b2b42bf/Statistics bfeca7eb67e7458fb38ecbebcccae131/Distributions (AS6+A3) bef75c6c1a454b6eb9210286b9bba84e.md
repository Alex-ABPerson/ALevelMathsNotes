# Distributions (AS6+A3)

You can say that a variable **follows a distribution** using the symbol $\sim$
. A **discrete uniform distribution** is where all possibilities have an equal probability.

# Binomial

This is represented with the function $B(n, p)$.

You cannot binomially distribute something that doesn’t meet these requirements. If you’re asked about it, use these and apply them to the question:

1. Only **two outcomes**
2. Only a **fixed number of trials and chance of success**
3. Only **independent** events

## Definition

Below is the exact formula for a binomial distribution - just make sure you know it exists:

$$
P(X=r) = \binom{n}{r}p^r(1-p)^{n-r}
$$

## Calculations

We can calculate the value of $P(X = x)$ and $P(X \le x)$ using the calculator. $P(X > x)$ can be done by finding $1 - P(X < x)$.

<aside>
⚠️ It’s $\bold{\le}$ and not $<$!!

</aside>

## Inverse

The calculator isn’t able to offer **inverse binomial** like normal because binomial is discrete and it simply wouldn’t work. If you need to find the right value for a $P(X\le x_1)$, say to find the critical region in binomial, you need to **brute force** your way through. The cool thing is the calculator has a table mode for doing this at least.

## When to use

Most of the time the need for binomial is really obvious but *sometimes* you will get a **sneaky binomial question** where you need to form your own definition. For instance, you might be asked what the probability is of something happening 3 times out of a certain number of situations - this is binomial!!

# Normal

This is represented as $N(\mu, \red{\sigma^2})$. 

<aside>
💡 The bit in red is the **variance**, as standard deviation is the non-squared thing.

</aside>

## Sketching

We can represent a normal distribution through a bell-curve. This bell curve has:

- The **mean** in the middle
- The area between $\mu \pm \sigma$ and $\mu$ *on both sides* is **0.68**
- The area between $\mu \pm 2\sigma$ and $\mu$ *on both sides* is **0.95**
- The area between $\mu \pm 3\sigma$ and $\mu$ *on both sides* is **0.997**

For many questions it is a very good idea to sketch it so you know what they’re really asking you to do. When doing this, while it’s not the end of the world if you mess it up, you should use the logic above as much as possible to try and get it right.

## Calculations

We can flawlessly calculate $P(X > a)$, $P(X < a)$ and $P(a < X < b)$ all with our calculator, as it allows ranges.

<aside>
🧮 Do keep in mind that the mean and standard deviation values on the calculator are reverse of what you’d expect!!

</aside>

## Continuousness

Unlike binomial, normal is **continuous.** This means that unlike binomial where $P(X \lt a) \ne P(X \le a)$, in normal we can use $<$ and $\le$ interchangeably as there’s 0.000000001 of a difference.

## Inverse

If we have $P(X \lt a) = b$ or similar, we can find the value of $a$ through our calculator. For $P(X > a)$ this can be applied with some rearrangement and for $P(46 < X < b) =c$ we must perform a sketch.

<aside>
⚠️ The inverse normal function on the calculator **specifically does** $P(X<a)$, not $P(X = a)$.

</aside>

You can be asked some very bizarre questions like what the interquartile range of a graph is. This is just an inverse normal range question in disguise, where you have **0.25** on each side of the Qs!

# Standard Normal

$\mathcal{Z}$ is a variable that’s normally distributed by $N(0, 1^2)$, and we can *turn any* complex normal distributions into this normal distribution by simply coding it a bit. It’s really simple and logical, you want the mean to be at 0 instead of wherever it is, so we **subtract $\mu$,** and we want to make sure the *scale* keeps us a standard distribution of 1, so we just say the following. 

$$
P(X < 5) = P(\mathcal{Z} < \frac{5 - \mu}{\sigma})
$$

<aside>
🖊️ The default settings on the calculator is the standard normal ones.

</aside>

The ***most common*** use of this technique, and the one you’ll see in the exam, is when you have an unknown in the normal and need to find it.

# Estimating Binomial with Normal

We can use the normal distribution to estimate the value of a binomial distribution. This is **necessary** to do this if $n > 50$ because we don’t have any tables for values above this, and can only be done if $p$ is *near to* 0.5.

**Changing the definition**

Apply the formula $X \sim B(n,p) \rarr Y \sim N(np, np(1-p))$.

**Changing the use**

We need to apply **continuity correction** to the usage. Since binomial is discrete and normal is continuous, we need to *round* what we’re considering to the correct near 0.5 value. The best way to do this is as follows:

1. Turn the LHS into having an *equal to* on it.
2. Extend the range of values included by 0.5.