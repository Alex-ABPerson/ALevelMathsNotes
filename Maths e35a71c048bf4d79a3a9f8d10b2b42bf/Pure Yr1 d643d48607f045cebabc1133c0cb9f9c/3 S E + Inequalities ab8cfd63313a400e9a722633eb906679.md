# 3. S.E. + Inequalities

# Simultaneous equations

<aside>
⚠️

**NOTE: Don't forget to solve *both* `x` and `y` and not just one - this is something you always forget to do!**

</aside>

In preparation for more complex simultaneous equations, there is a certain way you should structure your working out. **Number** each of the equations (usually with a number in a circle). And then describe the operations you're performing on each one. Anytime you come up with a new equation, you should *re-number* that one.

Also, always make sure to **write a conclusion!** For example, say "so" then write **co-ordinate** at the end like `(x, y)` or write `x = ...; y = ...`

With that said, there are **two ways** to solve simultaneous equations - by **elimination** or by **substitution!**

## **Elimination**

Elimination is the same you already know, just make sure you number the equations and *describe* what operations you're performing. E.g. write `(2) - (1)` if you're subtracting equation 2 from equation 1.

## **Substitution**

Substitution is another technique you can use to solve simultaneous equations. To do this, you just need to *place* one equation into another. For example, if you have the following two simultaneous equations (**numbered** 1 and 2 respectively):

$$
x + 3y = 11 
$$

$$
4x - 7y = 6
$$

You can rearrange equation **1** into $x = 11 - 3y$, and then replace $x$ with $11 - 3y$ in the second equation. Once you've done this, with some expanding and rearrangement you should find the solution to `y`. *Which you can then use to get `x`*

<aside>
🔑 Don't forget that it's **also valid** to substitute a variable on the more empty side of the `=`. For example, if you have $y = 2x - 4$ and $x^2 + 3x = y$ - you *can* make this into $x^2 + 3x = 2x - 4$, which with some rearrangement should help you solve it.

*This might even be necessary when you have some quadratic simultaneous equations going on.*

</aside>

# Inequalities

Solving inequalities is quite easy. Just treat the sign like it's a `=` - the **only** special thing you have to keep in mind is if you **divide** or **multiply** by a negative number, you must flip the sign!

This actually does present one **very important thing** you didn’t realize all the way until near the end of Year 1! If you have this $\frac{6}{x + 5} < 2$, you **can’t** turn this into $6 < 2(x+5)$, because we don’t know if this will require sign flipping. Instead, you need to multiply by $(x+5)^2$, which you *know* won’t be 

# Sets

You may need to represent your answers to inequalities to certain questions in **set notation.**

To represent a **new set**, you first need to wrap your answer in curly braces:

$$
\{ \space \}
$$

Now, you can describe **x** within this new set. If you have `x < 3` as your answer, and you need to write it in set notation, this is how you do it:

$$
\{ x: \space x < 3\}
$$

If you have two answers, such as `x > -2` **and** `x ≤ 4` - there are two ways you could represent this. 

The simplest way is to make one set with `x > -2` and another set with `x ≤ 4` and *merge* them as a **union**. Like so:

$$
\{x: x > -2 \} \space \cup \space \{ x: x \le 4 \}
$$

However, you can also represent it in just one set, like so:

$$
\{ x : -2 < x \le 4 \}
$$

## Combining Sets

There are **two ways** you can combine sets. One is called a **union,** and the other is called an **intersection**. 

- **Union:**
    
    A **union** is like this:
    
    $$
    \cup
    $$
    
    This combines the items in the first set and second set, so if you had `{1, 3}` and `{2, 4}`, you're going to get `{1, 2, 3, 4}`.
    
    You just think of it as an **OR**. It's simply merging both sets.
    

- **Intersection:**
    
    An **intersection** is like this:
    
    $$
    \cap
    $$
    
    This combines only the items shared in *both sets*.
    
    Think of this like an **AND.**
    

## Common Sets

There are a few common sets that we always see: The two most common ones being $\R$ (all Real numbers) and $\Z$ (all *natural numbers* - positive integers).

The symbol $\in$ means “is in” so if you see $x \in \R$, that means $x$ is any real value.

# Quadratic inequalities

You may get questions where you're asked to find the set of values `x` for which `... > 0` - `...` is typically something that gives us a curve when plotted, so this is really asking us any values of `x` where the line of the curve is going to be above `0`.

An example question might be to find the set of `x` values where $x^2 - 11x + 24 > 0$. What you can do is **solve** that quadratic (just treat the `>` as a `=`), and then use the solutions you get to put together an inequality for all the positions that go above the axis. **You MUST do this** 

For example, consider the following graph:

![Untitled](3%20S%20E%20+%20Inequalities%20ab8cfd63313a400e9a722633eb906679/Untitled.png)

If we're asked to find values where `... > 0` we just need to select the parts of the graphs where the x goes above 0. In this case, that's always going to be the things from the left of point "1" and the right point "2", anything between those would start to go negative.