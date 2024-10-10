# 12. Differentiation

**Differentiation** is a tool you can use to *create a function* that finds the gradient of a **tangent** of a curve at any $x$ position, from just the line function and a point. It's part of **calculus**, which is one of the most powerful tools in maths.

There are two ways of *naming* this function to find the gradient. One thing you can call it is $\frac{dy}{dx}$(or, to be exact, $\frac{\delta x}{\delta y}$), because $\frac{dy}{dx}$ is the gradient of the line at a point, and the other is $f'(x)$. You can write either of these as you want, I prefer $f'(x)$ though since it's clearer to visualize it as just a function like that. 

But, essentially:

$\frac{dy}{dx} = ..., y = ..., f'(x) = ...$

You can sometimes see the `y` and `x` in $\frac{dy}{dx}$ replaced with something else. Just remember that the `x` is what we're putting *into* the function and the `y` is what we're getting out, and you'll be fine.

# The idea

Differentiation comes down to the idea that if you have point $A$ and point $B$, and you draw a line between them, the gradient of that line will be *closer* to the gradient of the tangent of $A$ the *closer $B$* is.

So if you make the Y of $A$ just plain old $f(x)$ and we start *shifting $B$ 's* X and Y **ahead by $h$ (so the y is $f(x+h)$), the smaller $h$ is, the closer the gradient between the two points is going to get to actually *being the gradient of the tangent*.

So, if we can get $h$ as *low as possible* (we can't literally just make it zero, but make it *as low as physically possible*), and then find the gradient between points $A$ and $B$, we have the gradient of the tangent there!

<aside>
🖊️ In differentiation this $h$ value can often also be written as $\delta x$.

</aside>

# Limits

A **limit** is something you can add to an equation, and it's critical for calculus and integrals. 

You can write it in the following form:

$$
a = \lim_{b \to c}d
$$

This essentially means

> **As b gets closer to c, d gets closer to a**
> 

# First principle

Differentiation’s **first principle** is the equation, because it’s the basic idea the process is built on.

The gradient of a line is, as we know $\frac{\triangle y}{\triangle x}$. Now, as we discussed before, we're going to make point $B$ the same `x` as $A$, just with a `+ h` slapped on it, just so it's ahead of point $A$ by a really tiny amount. So, if we want to get the gradient between these two things, we're going to get this:

$$
\frac{y_2 - y_1}{x_2 - x_1} \\
\space
\\
\frac{f(x + h) - f(x)}{x - x + h} \\
\space
\\
\frac{f(x + h) - f(x)}{h}

$$

Now, all we need to do is **indicate** that the `h` is always heading really close *to 0*, and we have the equation!

We can indicate this using a **limit** on $h$. We can limit $h$ to always be towards zero, like so:

$$
\lim_{h \to 0}
$$

So, altogether you get:

$$
f'(x) = \lim_{h \to 0}\frac{f(x + h) - f(x)}{h}
$$

And that is the equation for differentiating. (You don't need to recall this but I guess you will now)

## Using the equation

Now, to actually *solve the equation*, what you need to do is **leave** the $lim$ on the equation and simplify it down *as much as physically possible.* And only right at the very end, after simplifying it, can you then remove the $lim$ and treat $h$ like it's $0$.

The reason we do this is if you set $h$ to `0` straight away - the fraction would become $\frac{f(x)-f(x)}{0}$, and you can't really divide by 0.

Even if you treated this fraction's value as $\infin$, this is also the same as $\frac{0}0$, which should be `1` - so we're getting conflicting answers and therefore this is in **indeterminate form**. We can't get a valid answer out of it when it's in this form.

However, after expansion and simplification, we can get it in a form that does make sense and is evaluable.

## In practice

Now, the *solid equation* is nice and you can technically do absolutely any differentiation you want with it. But it's very time-consuming to do all the expansion and such needed, so instead of doing all of that, there is a *trick* you can use that has the *same effect* as the equation.

> If you have a $x^a$ in your line's equation, you can *transform* that into $ax^{a - 1}$.
> 

<aside>
⚠️ You can remember this order based on the fact that differentiating has **diff** in the name - meaning it’s about *subtracting*. And you typically do $a - b$ so the subtraction occurs *second.*

</aside>

And that's it! That replicates a lot of what the equation does. And if you have a **polynomial,** just do this on *each term* in the polynomial.

$$
f(x) = x^3 + 2x^5 \\
\space \\
f'(x) = 3x^2 + 10x^4
$$

<aside>
💡 If you have anything in your polynomial without an $x$ - **ignore it!** Because all that's doing is *translating* the line, and that's not going to affect the gradient, that's just... Well, moving it about, so it's irrelevant to us.

If you actually think about it, if you treated this constant like it was $cx^0$, and you differentiate it and multiply $c$ by $0$ - it disappears! So this really does work.

</aside>

## Rate of change

You can **differentiate** a *second time* to find $f''(x)$ or $\frac{d^2y}{dx^2}$ - and this is known as the **second-order derivative**. This will tell you the **rate of change** for the gradient at a particular point - i.e. how *quickly* the gradient is changing at a point. This value is very useful for identifying **stationary points**, when you compare them to the original function.

## Stationary points

A **stationary point** is a point where the *gradient* is `0`. When the gradient is zero, it's always going to be either the **maximum,** the **minimum** or a **point of inflection** for the graph. You can **find** stationary points by setting $f'(x)$ to zero and you can figure out what a stationary point means using $f''(x)$.

You can check which one of these it is using 

- **Local maximum** - This means this point is the *highest point* for the part of the graph we're currently looking at (the "local" part).
    
    The $f''(x)$ **at** a maximum point will always be $<0$.
    

![LocalMaximum.png](12%20Differentiation%20c85e6b7e84f34b4e91d0eb6931f5133a/LocalMaximum.png)

- **Local minimum** - This means this point is the *lowest* for the part of the graph we're currently looking at
    
    The $f''(x)$ **at** a minimum point will always be $> 0$. 
    

![LocalMinimum.png](12%20Differentiation%20c85e6b7e84f34b4e91d0eb6931f5133a/LocalMinimum.png)

- **Point of inflection** - This is where the line is *temporarily* stopping but is going to continue on soon
    
    The $f''(x)$ at a point of inflection will always be $= 0$.
    

![Untitled](12%20Differentiation%20c85e6b7e84f34b4e91d0eb6931f5133a/Untitled.png)

<aside>
🍷 One way you can remember what a given $f''(x)$ represents is by thinking of the original $f(x)$  as a wine glass. 

When $f''(x) > 0$, your glass is **upright,** like above, it has a *positive* (above 0) amount of wine in it, and *therefore* this point is the minimum of the graph.

When $f''(x) < 0$, your glass is **upside-down,** like above, and has no wine in it as it's all spilt everywhere, and *therefore* this point is the maximum.

And, my favourite one, when $f''(x) = 0$, your glass is just shattered and a mess and it's all over the place

</aside>

## Graphing $f(x)$, $f'(x)$ and $f''(x)$

One thing you need to be able to do is sketch $f'(x)$ in a graph without differentiating. It's actually really easy to do. Just make sure your line is **above 0** when there's an upwards gradient, make sure it's **below 0** when there's a downwards gradient, and make sure it's **at 0** when the line goes flat. Here's an example:

(Red is $f(x)$, **black is $f'(x)$** )

![Untitled](12%20Differentiation%20c85e6b7e84f34b4e91d0eb6931f5133a/Untitled%201.png)

<aside>
💡 One very interesting pattern you might notice is $f(x)$ was a cubic graph, while $f'(x)$ was a quadratic graph - that's what happens when you differentiate, the degree goes down!

</aside>

Also, you don't need to be able to do this, but it is interesting to see what happens when you sketch all of them *together.* You'll notice there are some patterns between all of them:

![Untitled](12%20Differentiation%20c85e6b7e84f34b4e91d0eb6931f5133a/Untitled%202.png)

## Mechanics with differentiation

$\frac{dy}{dx}$ is essentially represented as