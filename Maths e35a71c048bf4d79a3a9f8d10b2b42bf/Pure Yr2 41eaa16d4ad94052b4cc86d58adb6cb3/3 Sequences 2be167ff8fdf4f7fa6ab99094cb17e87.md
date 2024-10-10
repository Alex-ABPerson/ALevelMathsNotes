# 3. Sequences

A **sequence** is a list of terms (e.g. `2, 5, 7`). A **series** is the sum of a list of terms (e.g. `2 + 5 + 7`).

When you have a sequence of items, the variable used to represent an index in it is $n$ and the value of a term at index $n$ is given as $u_n$.

A sequence is considered to be **strictly increasing** if it only ever increases, and **strictly decreasing** if it only ever decreases. A **periodic sequence** is one where terms repeats in a cycle (a *recurrence relation* sequence below) - these sequences have what’s known as an **order**, which is how many terms there are in each loop (for some reason).

# Arithmetic

An **arithmetic sequence** is a sequence where each term goes up or down and the same pace. Now, in GCSE, when we had sequences, we came up with the equation for it just by looking at it (rate of increase), but in A Level we have to take it a bit more “first principles” than that. For A Level we use this equation to come up with an equation for a sequence (which you must remember):

$$
u_n = a + (n-1)d
$$

The reason we have this equation is it lets us algebraically find the equation for a sequence from all kinds of situations, no “guessing” involved. 

When you have a question with arithmetic sequences, it will usually involve only one of two things:

1. Using the fact that the difference is the same between items (e.g. “For what values of $x$ is $-8, x^2, 17x$ an arithmetic sequence?”)
2. Using the equation (in both normal form and with inequalities)

## Series

There’s also an equation that finds the *sum* of the first $n$ items of a sequence. That might sound kind of impossible to have an equation for, but it’s actually really simple! The way it works is it’s all centred around the simple fact that in an arithmetic sequence `first + last`, `second + second-to-last`, `third + third-to-last` etc. items will *always* give us the exact same total. E.g. With `3, 6, 9, 12` `3 + 12 = 15`, `6 + 9 = 15` etc.

So, built around this idea of taking $\frac{n}2$ items from the beginning and $\frac{n}2$ items from the end and adding them to give the same total, you get this (which is given to you in the exam):

$$
S_n = \frac{n}2(2a + (n-1)d)
$$

### Proof

You need to be able to prove it in the exam. 

**Step 1 - Write two series**

To do that, you write two algebraic arithmetic series: One representing the start items, and one representing the end items. They look like this:

$$
\begin{matrix} a \\ a+(n-1)d\end{matrix}\space + \begin{matrix} a+d \\ a+a(n-2)d\end{matrix}\space +\begin{matrix} a+2d \\ a+a(n-3)d\end{matrix}\space + ... + \begin{matrix} a+(n-1)d \\ a\end{matrix}
$$

**Step 2 - Add the two series**

Add each term vertically, which will give you the $2S_n$ (because we’ve got the series twice now):

$$
2S_n = 2a+(n-1)d+2a+(n-1)d+2a+(n-1)d+...+2a+(n-1)d
$$

**Step 3 - Simplify**

And since this is happening *n* times, we’ve got:

$$
2S_n = n(2a + (n-1)d) \\
S_n = \frac{n}2(2a + (n-1)d)
$$

# Geometric

A **geometric sequence** is a sequence where each term goes increases of decreases by a common ratio, `r`. You can find this ratio by taking one item and dividing it by the previous item (e.g. if you had $8, 16$ , you can do $\frac{16}8$ to get the common ratio).

If the `r` is negative, you have what’s known as an **alternating sequence**, as the sign alternates back and forth between positive and negative between the terms.

The formula for geometric sequences is:

$$
u_n = ar^{n-1}
$$

You can literally see this the case by just writing out a sequence and what happens to it: $a, ar^1,ar^2, ar^3...$ - might be worth just doing that when you need to remember the formula!

## Series

For geometric sequences, we can get an equation to find the sum of the first $n$ items. This equation is formed from the fact that the difference between a series and a series of all the next terms always cancels down to two terms.

$$
S_n = \frac{a(1-r^n)}{1-r},r\ne1
$$

### Proof

**Step 1 - Write two series**

Make two variants of the series: One is normal, and the other where each term is the sequence one term ahead (a.k.a. multiplied by `r`).

$$
S_n = a+ar+ar^2 +...+ar^{n-2}+ar^{n-1} \\
rS_n = \phantom{a} ar + ar ^2 + ... + ar^{n-1} + ar^{n}
$$

**Step 2 - Subtract them from each other**

Subtract the two sequences from each other, and you can see by looking at the layout above, that pretty much *everything* is going to cancel out, except the first $a$ and the negated $ar^n$ at the end:

$$
S_n - rS_n = a - ar^n
$$

**Step 3 - Simplify**

Now, we can just simplify this as necessary to get the given equation:

$$
S_n(1-r) = a(1-r^n) \\
S_n = \frac{a(1-r^n)}{1-r}
$$

## Series to infinity

If you do $S_{\infin}$, then as you’d expect, you’re gonna get $\infin$… *Unless $|r| < 1$.* When $|r|<1$, it’s known as a **convergent series** and in this situation, something special happens where it *doesn’t* infinitely go up, but rather converges on one very specific small value.

This happens because if you look closely at the geometric series formula, the only thing in it that changes as you move along the series, is the $r^n$ piece. And when $|r| < 1$, this value actually gets **smaller** instead of bigger! This makes it such that there is a finite value and we have a dedicated formula for finding it (which, well, I’m sure you can see where it’s come from):

$$
S_{\infin} = \frac{a}{1-r}
$$

<aside>
❕ When $\{ r: r > 1 \} \cup \{ r: r < 1 \}$, that’s known as a **divergent series**.

</aside>

## Recurring decimals

When you have a question about decimals like $0.\dot{2}\dot{3}$, these are actually series questions *in disguise*. In reality, this is really a geometric series that goes: $\frac{23}{100} + \frac{23}{10000} + ...$. So, if you’re asked to find the exact value of this, what you really need to do is:

1. Find out what `r` is, by doing `2nd / 1st`
2. Use $S_{\infin}$ to find its value.

The technique we used in GCSE wasn’t really practical.

# Sigma

**Sigma** *(the capital S is important because with Greek it matters)* is literally a “for loop” applied to series. It allows you create a series comprised of a given thing repeated a given number of times, with a number changing each time. The notation is below: On the top is the end index, on the bottom is the start index, and in the middle is your term.

$$
\sum_{n=\text{min}}^\text{max}(nx) = x + 2x + ...
$$

You can perform all the same operations on this as you would any other series, you usually need to expand it out a bit to figure out what kind of sequence it is, though.

<aside>
❕ Be careful, sigma is a $\le$ loop, so the number of iterations is always $+1$  the $\text{max} - \text{min}$.

</aside>

# Recurrence Relations

A **recurrence relation** sequence is one where each term depends on the term that came before it. They’re usually given as $x_1 = ..., x_{n+1} = ...$.

Many recurrence relations will start to ***loop*** after a certain point and repeat themselves. For example, you might get $x_1 = 3, x_2 = 7, x_3  = 12, x_4 = 3$, and because the $x_4$ is $3$, it’ll loop here as the terms after will just go through the same process again - it’s just like our sequential logic systems in Electronics!

So, if you’re asked to find the sum of any of these sequences, usually they’re expecting you to go through a few terms and find the loop, then use that to do the sum.

# Modelling

Modelling with sequences is generally quite simple - one thing that can catch you out though and you have to keep an eye out for is when a modelling question has an initial state you need to include. I.e. if you wanted to find the height of a piece of A4 paper after folding it 4 times, you have to find the sum of the first **5** terms because the unfolded state counts!