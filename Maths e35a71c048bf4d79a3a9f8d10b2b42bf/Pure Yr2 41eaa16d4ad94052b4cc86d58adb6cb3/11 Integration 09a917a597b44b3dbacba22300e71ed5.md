# 11. Integration

When you write out the final form of an integral, make sure you represent $\ln(x)$ as $\ln|x|$, this will make it easier to evaluate the final value.

Since integration is the reverse of differentiation, we have a technique to replicate pretty much everything you can do in differentiation.

- **Chain rule** $\rarr$ By recognition
- **Product rule** $\rarr$ By parts
- **Parametric Differentiation** $\rarr$ Parametric Integration
- **Implicit differentiation** $\rarr$ Separating variables under “solving differential equations”

Below are the three techniques we can apply to integrate things.

# By recognition

This is all about **recognising** when you have a differentiated form of something, and then reversing it. The way we do this is we **ignore** all the constants and specific details of what we’re integrating, and just look at any key pieces that we might know where they come from. And then we just *test* out what that’ll give and make any tweaks necessary to it. This is the exact process:

1. **Test** the form you’ve recognised the equation may have come from by differentiating
2. Determine what **adjustments** need to be made to it to get the same constants as what we have
3. Apply that adjustment to what we tested and finish.

<aside>
💡 The easiest way of applying that adjustment is to do a fraction with the *old number* on the bottom to cancel away and the *new number* on the top to fill it back in.

</aside>

Example #1: $\int 4e^{3x} dx$, test $y = e^{3x}, \frac{dy}{dx} = 3e^{3x}$, adjust x $\frac{4}3$.

Example #2: $\int \frac{4x}{x^2} dx$, test $y = \ln{x^2}, \frac{dy}{dx} = \frac{2x}{x^2}$, adjust x $2$.

## Reverse chain rule

One thing you should look out for is a position where **chain rule** may have been applied. If you see something in the form $u'u^n$, then you know you can test out $u^\bold{n+1}$ and go from there.

<aside>
⚠️ Do not forget to test with the number **increased**!

</aside>

## Trigonometry

There’s a few things you need to remember with trig that you’ve slipped up on in the past with trigonometry:

1. Things like $\sec x \tan x$ are one-step to integrate with the three circles!
2. You should try reverse chain rule if something isn’t directly recognisable - be careful, sometimes the **left** differentiates ****to the thing on the right and it is reverse chain!
3. **Only** try to rewrite with identities if you can’t recognise or reverse chain something - and when you do, remember that you can use the **RHS** of the double-angle formulas often. E.g. if you have a $\cos^2 x$ , you can rearrange $\cos2x \equiv 2\cos^2x - 1$.

# By parts

Integration by parts is kind of the equivalent to product rule in differentiation. If you have two functions in terms of `x` next to each other, and you cannot apply reverse chain rule, you can then use integration by parts.

This is the formula for integration by parts:

$$
\int uv' \text{dx} = uv - \int u'v \text{dx}
$$

<aside>
💡 The $v'$ on the left side of the equation doesn’t mean “differentiate v”, it actually means “*treat the v we have like it’s already differentiated”.*

</aside>

To use this formula, here’s what you need to do:

**1 - Choose $u$ and $v$**

Which way around you treat the $u$ and $v$ does matter, because what you *really* want is for the $u'$ over the right to get closer and closer to a constant with each iteration. There’s an acronym to make sure it always works out, but trial-and-error can get you there. The acronym is: $\text{LogAlgebraTrigExponential}$.

<aside>
🧠 It’s easy to forget that A is algebra and T is trig

</aside>

**2 - Lay out your $u$ and $v$ values you have**

The neatest way of doing it is to start off the normal text, then fill in the red text from there:

$$
u = ... \\
\red{u' = ...}
$$

$$
\red{v = ...} \\
v' = ...
$$

<aside>
🖊️ We don’t need to put a $+ c$ on the $v=$ bit because our end result is going to have a $+\space c$ anyway and it’d just contribute to that $c$, so there’s no real point bothering.

</aside>

**3 - Use the equation!**

And now you have everything prepared to use the equation! Just put the correct values into the correct places. For some questions you have to use integration by parts *multiple times*, which is pretty funky!

## Looping Parts

Sometimes you’ll get a question where you have by parts **looping**, where you get the original equation from the subbed value. When this occurs, you’re expected to do this key thing:

1. Keep going until you get one cycle
2. Set the original equation to equal $I$.
3. Replace the LHS of our parts with $I$ and the loop on the right with $I$, and collect like terms to get $2I$.
4. Rearrange and we can get our answer.

# By substitution

If an equation is too difficult to integrate on its own, we can use *integration by substitution* to attempt to simplify it. Now, in reality you would probably never actually use this by yourself because there’s always better, easier ways of integrating difficult things. But, if you are *asked to use this* in an exam, you gotta do it, of course!

There’s two parts to doing this: One part is to replace all our $x$ terms with $u$ through the substitution. And the second part is to turn our $\text{dx}$ (which actually *is* a term in our integral) into $\text{du}$. This is the process I recommend you do:

1. Figure out what we’re going to turn the $\text{dx}$ into. Because replacing this often opens us up for cancelling terms inside the integral, you should do this first and see what you get left with.
2. Figure out all the terms you need to replace with $u$.
3. Perform the integration, and if necessary re-substitute our x back in through $u$.

## With Limits

If you have a definite integral, you can either perform the integration and turn it back into terms of $x$ before doing your limits, *or,* even better, you can **leave it** in terms of $u$ and turn your limits in values in terms of u through the equation. Best way is with a little table like this:

| x | u |
| --- | --- |
| 0 | 0 |
| 3 | 9 |

Outside of properly integrating, there’s some other concepts you also need to understand.

Two quick small things: 

**Tell me to integrate without telling me to integrate**

Sometimes you’ll get questions that ask you to find:

$$
\lim_{\delta x \to 0} \sum_{x=a}^b f(x) \delta x
$$

Literally all this means when you really look at it is “find the area under the curve”, so you’re just going to apply an integral.

**Swapping limits on integrals**

If you swap limits of an integral with each other, you’re just multiplying your integral’s value by -1 - which is pretty obvious when you visualize the definite integration process. 

# Parametric Integration

The equation to parametrically integrate is as follows:

$$
\int y \frac{dx}{dt} \text{dt}
$$

If you need to do this definitely, you need to find the $t$ value at each of the limits and use that as necessary. Make sure you don’t change the order of the limits when you do this!

# Trapezium Rule

**Trapezium Rule** is a trick we can use to estimate the value of a definite integral. The idea is very simple, if you take the area under a curve and break it up into equal strips, you can treat each strip like it’s a trapezium, which will be “mostly accurate”. By combining the area of these trapeziums, we get an estimate for the area under the curve, and therefore an estimate for the value of an integral!

When performing trapezium rule, we call the base width of each strip the $h$ and the values around each strip the $y_x$.

# Differential Equations

To “solve a differential equation” essentially just means “*to integrate it”*. 

<aside>
💡

</aside>

We use specific terminology to refer to this that’s introduced only in this section for some reason, so let’s explore it now. 

A **general solution** is an equation with $+ c$ in it. A sketch of the **family of solutions** is all the different values of c sketched out in a graph. A **particular solution** is a solution with the constant found - and we can *find* a constant through a **boundary condition**.

## Separating variables

We can use the **separating variables** technique to solve equations in the form $\frac{dy}{dx} = ...$ where the `...` either contains *both x and y* terms *or* just *y* terms. This technique is essentially the opposite of **implicit differentiation** (and the reverse $\frac{dy}{dx}$ trick)**.**

To perform this trick, you need to rearrange the equation so you get the $y$ terms over on the side of the $dy$ and the $x$ terms on the side of the $dx$. Then, you can take the integral of both sides. Once you solve the integrals, you only need to put the $+ c$  one one side as the constants from each side collect together.

<aside>
💡 If you have a question that ends in all $\ln$s, a quick trick you can use to make sure easier is to rewrite $c$ as $\ln k$.

</aside>

## Family of solutions

Because of the above technique of *separating variables* and the rearrangement that comes at the end of it, what can sometimes happen is your $c$ ends up not as a translation at the end of the equation, but as a multiplier of a function of x, so consider that when sketching the family of solutions. 

## Modelling with them

There are certain questions that are asking you to use the “solving differential equations” technique. These questions are *not* that obvious, but here’s essentially the criteria:

> If you have a differential equation and need to find an expression in terms of two variables involved in it - use the separating variables technique!
> 

<aside>
💡

Remember that ***all*** “solve” means is “get into the form `y = ...`” so… yeah, *solving a differential equation* is just integrating it.

</aside>

# Integral of the Day

### 07/12/2022

**Question:** Integrate $\int \ln^2x \text{ dx}$.

**Working**

$$
\text{Let u =} \ln x \\
\frac{du}{dx} = \frac{1}{x} \rarr dx = du\space x
$$

$$
\int u^2 \text{ du}x = \int u^2x \text{ du} \\
u = \ln x, \text{ So } x = e^u \\
\text{So } \int u^2e^u \text{du}

$$

$$
\text{Using } \int ab' \text{du} = ab - \int a'b \text{du} \text{ ...} \\
a = u^2, a' = 2u...\space b' = e^u, b = e^u \\
\text{So } \int u^2e^u \text{du} = u^2e^u - \red{\int 2ue^u \text{du}}
$$

$$
\red{\text{Using } \int ab' \text{du} = ab - \int a'b \text{du} \text{ again...} \\
a = 2u, a' = 2...\space b' = e^u, b = e^u} \\
\text{So } \int u^2e^u \text{du} = u^2e^u - \red{(2ue^u-\int2e^u\text{du})}
$$

$$
\int u^2e^u \text{du} = u^2e^u - 2ue^u + \int2e^u\text{du} + c
$$

$$
\int u^2e^u \text{du} = u^2e^u - 2ue^u + 2e^u + c
$$

$$
\int u^2e^u \text{du} = e^u(u^2 - 2u + 2) + c
$$

$$
\text{Since u = } \ln x, \int u^2e^u \text{du} = e^{\ln x}(\ln^2x - 2\ln x + 2) + c 
$$

$$
\text{So finally: } \int u^2e^u \text{du} = x(ln^2x - 2\ln x + 2) + c
$$

### 08/12/2022

$$
\int{\frac{x^2}{\sqrt{9-x^2}}}
$$

**Working**

### High Rearrangement Integral

$$
\int \sin x \cos 2x \text{ dx} \\
\int \sin x(1 - 2\sin^2 x) \text{ dx} \\
\int \sin x - 2\sin^3 x \text{ dx} \\
\int \sin x - 2\sin x \sin^2 x \text{ dx} \\
\int \sin x - 2\sin x (1- \cos^2x)\text{ dx} \\
\int \sin x - 2\sin x + 2\sin x \cos^2x \text{ dx} \\
\int -\sin x + 2\sin x \cos^2x \text{ dx} \\
\ \\
\text{Test} \\
f(x) = \cos^3 x \\ f'(x) = -3\sin x \cos^2x \\
\text{Off by x}\frac{2}3 \\
\ \\
\text{So } ... + \frac{2}3 \cos^3x
$$