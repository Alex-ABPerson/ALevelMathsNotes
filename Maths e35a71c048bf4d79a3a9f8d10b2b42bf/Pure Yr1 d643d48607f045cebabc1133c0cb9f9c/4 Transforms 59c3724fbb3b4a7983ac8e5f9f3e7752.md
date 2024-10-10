# 4. Transforms

TO IMPROVE: Sketching cubics!

# Sketching

When you want to *sketch* graphs, there are three things you need:

1. **The roots -** Make sure you find out where it cross the x-axis by factorising, and setting each outer term equal to `0`.
2. **The y-intercept -** Make sure you find out where it cross the y-axis. 

You can find this by substituting the `x` in whatever equation you have (unexpanded or not) by `0` and seeing what you get. You substitute it by `0`  because that's where the y-intercept always is on the y-axis. 
    
    <aside>
    🚄 When you have the form `x^2 + bx + c` - the y-intercept will always just end up being `c` as the rest gets removed by the `0` term. This is why it’s *called* c in $y = mx+c$. Actually pretty clever ;)
    
    Similarly, when you have the factorised form, such as `(x+4)(x-3)`, when expanded those last terms just become the $c$ so you can just multiply them and there’s your y-intercept.
    
    </aside>
    
3. **The shape** - If needed, pick a point somewhere to find out what direction it goes in.

As long as it follows these rules, you will have an accurate enough sketch and get the marks.

# **Reciprocal graphs**

Reciprocal graphs are graphs represented as one of the following:

$$
y = \frac{k}{x},\space y = \frac{k}{x^2}
$$

These graphs are made up of **asymptotes**, which are lines that go *towards* a point but never actually hit it. In this case, the lines are **always** heading towards an `x` of `0`, but can never get there because `k/0` is *undefined*. In addition, the lines are **also** always heading towards a `y` of 0, but never hit it, because if you rearrange the first one you'll get:

$$
x = \frac{k}{y}
$$

And `k/0` is still undefined.

<aside>
🖊️ It's very helpful to remember that they're always heading towards **x = 0** *and* **y = 0**, to make sure you draw them right.

</aside>

When it comes to *drawing* reciprocal graphs having an $x$ and an $x^2$ are a little different, although the lines themselves remain mostly the same. 

- **Non-squared**
    
    In these graphs, lines are on alternate sides of the x-axis.
    
    **When `k` is positive**
    
    `x` being positive is going to cause `positive / positive`, so that side will have a positive y.
    
    `x` being negative is going to cause `positive / negative`, so that side will have a negative y.
    
    **When `k` is negative**
    
    `x` being positive is going to cause `negative / positive`, so that side will have a negative y.
    
    `x` being negative is going to cause `negative / negative`, so that side will have a positive y.
    
- **Squared**
    
    With an $x^2$, because the square forces the $x$ to always be positive, the `x` can never affect the sign on the `y` - this means both sides, regardless of whether the x is actually negative or not, are going to always have the *same sign*. It's all left down to the `k`, so whatever sign the `k` is, is the side the line goes on. If `k` is positive, they go above `y` and if `k` is negative, they'll both go below `y`.
    

A higher value of `k` pushes the lines out more.

# Polynomial Graphs

There is one very interesting pattern that applies to these. Each time you up the number of powers in these graphs, the direction the first line starts in changes each time. So, **quadratic graphs** start with the line descending down at the beginning, and then **cubic graphs** have it ascending, and then **quartic graphs** have it descending etc.

## **Quadratic graphs**

If you just have the following structure in your equation:

$$
x^2+a
$$

That represents a **quadratic graph.** These graphs have a shape known as a **parabola.** They cross the x-axis **two or less** times. ****You can see what it looks like below:

![Quadratic.png](4%20Transforms%2059c3724fbb3b4a7983ac8e5f9f3e7752/Quadratic.png)

The reason it's shaped like this is that the power causes the negative `x`s to end up becoming positive, resulting in an upwards value on both the left and the right.

The shape above is a **positive parabola,** if you add a `-` before the squared term, it will flip the other way. The value before term with `x` it will grow or shrink the graph by certain amounts.

<aside>
🙋 You can remember this as the **positive parabola** is the one where it's happy (positive), and the negative parabola is the one where it's not.

</aside>

<aside>
🖊️ When drawing a quadratic graph, remember that they're symmetrical, so the min-point will always be exactly between the two roots.

</aside>

## **Cubic graphs**

Cubic graphs are equations that follow the form:

$$
x^3 + bx^2 + cx + d
$$

These can cross the x-axis **three times or below**. Here's what a **positive cubic graph** looks like:

![Cubic.png](4%20Transforms%2059c3724fbb3b4a7983ac8e5f9f3e7752/Cubic.png)

With a **positive cubic graph**, the line always starts *upwards (to positive)*. 

With a **negative cubic graph**, the line always starts *downwards (to negative)*. 

## **Quartic graphs**

Quartic graphs have equations that follow the form:

$$
ax^4 + bx^3+cx^2+dx+e
$$

These have **four or fewer** roots, as the name suggests.

With a **positive quartic graph**, the line always starts *downwards (to negative).*

And then there's one more type of graph (besides linear graphs), called **reciprocal graphs**. These are also known as **asymptote graphs**.

# Transforming Graphs

There are a number of operations you can apply to graphs, and they affect the graph in certain ways. 

In the below examples, $f(x)$ is a function that gives back the `y` position from a given `x` position of a graph.

## **Translation**

You can translate a graph **up** by $a$ using $y = f(x) + a$. This can be described as $\begin{pmatrix}0 \\ a \end{pmatrix}$

You can translate a graph **left** by $a$ using $y = f(x +a)$. This can be described as$\begin{pmatrix}-a \\ 0 \end{pmatrix}$

<aside>
💡 Don't forget that translating left or up will affect the y-intercept.

</aside>

## **Stretching**

You can stretch a graph **vertically** by the scale factor of $a$ using $y = af(x)$.

You can stretch a graph **horizontally** by the scale factor of $\frac{1}{a}$ using $y = f(ax)$.

<aside>
👀 This explains why in the *completed square form* the a in $p(x + q)^2 + r$ is just *part of* a scale because the way that $p$ was achieved was by multiplying *everything* by it.

</aside>

## **Reflecting**

You can reflect a graph on the **x-axis** with $y = -f(x)$.

You can reflect a graph on the **y-axis** with $y = f(-x)$.