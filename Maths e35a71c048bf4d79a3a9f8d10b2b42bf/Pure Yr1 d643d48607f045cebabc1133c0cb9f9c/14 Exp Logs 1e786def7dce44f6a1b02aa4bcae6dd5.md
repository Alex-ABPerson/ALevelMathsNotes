# 14. Exp/Logs

# Exponentials

An exponential is a curve with the form $y = n^x$, where $n$ is a constant. The x-axis is always an **asymptote** for an exponential - even negative numbers will just be fractions and can never really hit 0.

**Euler’s number**, represented as $e$, is a constant number, that when used as the base of an exponential graph will create a “perfect” exponential graph. In this graph, the gradient at any point will always be the *same* as $x$. So the gradient at $e^3$ will always be $3$, the gradient at $e^4$ will be $4$ etc.

## Differentiating

If you have a graph with euler’s number as the base, due to its unique property, differentiating it will always result in the graph function as the output. So if you have a graph of $y = e^x$, the differentiated form of that is just $e^x$.

However, if you have a graph with the form $e^{kx}$, this will always differentiate into $ke^{kx}$.

<aside>
💡 If you have a term like $e^{2x+1}$, you can break it apart into $e^1e^{2x}$

</aside>

# Logarithms

A **logarithm** is the opposite of index numbers - it will tell you the **index**, given a **base** and **value**. The *base* of the logarithm is the same as the base on the power. And the value *inside* the log is the evaluated result - so this lets you find the power. So essentially:

$$
x^y = z \\ \log_xz = y
$$

There are three different forms of writing it:

$\log_ny$ - This is a logarithm with the given base and the given value.

$\log y$ - This is a logarithm with the base of **10**. 

$\ln y$ - This is a logarithm with the base of *e***.**

## Log of both sides

One technique you can use in algebra when working with logs is to **take a log of both sides**. This is where you log both sides by a log with the same base number - this can be very helpful for a number of things.

## Log Laws

There a number of laws relating to logarithms that you need to know - these are all just “the opposites” of certain index laws. 

**Additive laws**

If you’re adding two same-base logarithms, you can simplify that multiplying the values within each:

$$
\log_nx + \log_ny = log_n{xy}
$$

In addition, when you subtract logarithms you end up *dividing* the two values, for the same reason as above.

$$
\log_nx - \log_ny = \log_n{\frac{x}{y}}
$$

If you think about it, this makes sense - if you look at $n^x * n^y = n^{x+y}$. Because the the *value* you get from the log is the power, so adding together the powers is just like doing this, where on the other side you’re multiplying.

**Coefficient linking**

The coefficient of the logarithm can be moved into a power in the log’s parameter. Like so:

$$
\log_ax^n = n\log_ax
$$

This happens because of the index law $(a^m)^n$. Because here you’re multiplying the index (what the log represents) by the value $n$, creating this.

**Special values**

Same base and value - $\log_aa = 1$, because $a^1 = a$.

Value of 1 - $\log_a1 = 0$, because $a^0 = 1$.

Reciprocal - $\log_a\frac{1}a = -1$, because $a^{-1} = \frac{1}{a}$

# Modelling

You can sometimes get models with exponentials in them, asking about a given thing. 

When you get questions like this, sometimes you’ll be asked to get a formula to find the **rate of change** at a given point. To get this, just **differentiate it!**

# Graphing

You can estimate values in an exponential-based model using a **graph.** What you do is take a log of both sides to try and get your equation into something of the form $y = mx+c$, then plot it and use it to find the $m$ and $c$.

For example:

$$
y = ax^n \\
\log y = \log ax^n \\
\log y = \log a + \log x^n \\
\log y = n\log x + \log a
$$

Here the *gradient* is $n$ and the y-intercept is $\log a$, so now you just need to pick a bunch of values for x and y and find the $\log x$ and $\log y$

Often if you have the equation $y = ax^n$, it becomes $\log y = n \log x + \log a$.

And if you have the equation $y = ab^x$, it often becomes $\log y = \log a + x\log b$