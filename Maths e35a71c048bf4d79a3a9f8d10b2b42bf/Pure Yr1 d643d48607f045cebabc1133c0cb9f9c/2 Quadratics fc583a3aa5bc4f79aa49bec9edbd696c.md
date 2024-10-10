# 2. Quadratics

# Completing the square

## **Concept**

*Completing the square* is an important technique for factorising a quadratic expression. What it does is it converts the first **two terms** (the ones that typically have **a** and **b** on them) ****into the **completed square form**.

<aside>
💡  Completing the square does not care about the **c -** you can apply it on equations with only the **a** or **b** terms

</aside>

The **completed square form** looks like this:

 

$$
p(x+q)^2 + r = 0
$$

Where `p`, `q` and `r` are **real constants.** This is the target we want to get out of completing the square.

## **Process (for a = 1)**

To complete the square on a quadratic with an **a** of **1**, like this:

$$
x^2 + bx
$$

All you need to do is arrange it like so:

$$
(x + \frac{b}{2})^2 - (\frac{b}{2})^2
$$

And when you do that, you'll have the completed square form!

<aside>
💡 If there's a **c** in the quadratic, just dump it at the end of each step, and then right at the end you should be able to fold it in with the $(\frac{b}{2})^2$, to achieve the full **completed square form!**

</aside>

## **Process (for a ≠ 1)**

Completing the square does not work if a ≠ 1. If you're in that situation, what you need to do is *make* a = 1, so we can then complete the square on the expression where a is 1. And once we've done that, we can expand it out again.

You can do this by factorising the first **two terms** by `a`. We don't need to factorise the c because the completing the square process doesn't actually care about it, we can just leave it at the end.

<aside>
📌 Don't worry if the `b` isn't easily divisible by `a` - **you can have fractions!**

</aside>

When you do this, you'll end up with something like this (with maybe a `c` at the end):

$$
a(x^2 + \frac{b}{a}x)
$$

Now you can **complete the square** on that bit in the brackets! This will leave you with something like this:

$$
a((x + q)^2 + r)
$$

Then, expand the additive line in the brackets, which will leave you with something like this:

$$
a(x + q)^2 + ar
$$

And if there's a `c` at the end, fold that with the `ar`

## **Extracting info from the completed square form**

Once you have the **completed square form**, you can extract the **turning point** from it simply by taking `(-q, r)` 

The **p** in the completed square form doesn't matter - it's just a stretch.

# New Ideas

- **Factorising non-squared quadratics**
    
    If you have a quadratic like this:
    
    $$
    x^6 + 9x^3 + 8
    $$
    
    Then don't worry, all you need to do is turn the $x^6$ into a square, like $(x^3)^2$. And change the second term into $9(x^3)$, and then treat the $x^3$ in each of these as a single block.
    
    **To Check:** Does this work if it was $27(x^3)^2 + 26x^4 - 1$
    
- **The discriminant**
    
    In the quadratic equation, there's a bit that goes:
    
    $$
    \sqrt{b^2-4ac}
    $$
    
    Because that $b^2 - 4ac$ is under the root, this is the bit that determines whether the quadratic expression is going to have a solution or not, as the root is always what *stops* the quadratic equation from solving (you can’t just square root a negative number, that’s when the quadratic equation never works).
    
    So, we call that bit the **discriminant** and can tell whether an equation is going to have a solution based on it. Here are the rules:
    
    **< 0 -** No solutions! The root will not work
    
    **= 0 -** One solution! The root will work but it's always going to give **0** and therefore the $\pm$is only going to have one sign, resulting in only one solution to the whole equation. **This is also known as a *tangential solution*.**
    
    **> 0 -** Two solutions!
    
    Remember that the number of solutions is the number of times it touches the **x-axis!**
    
- **Graph Shape**
    
    The shape of a quadratic graph is what's known as a **parabola**. And it can either make a "U" shape or a "^" shape. If the `a` is *positive*, it will always be a "U" shape, and if it's negative, it will always be a "^" shape.
    
- **Always remember to go the simplest way!**
    
    If you see the following equation:
    
    $$
    (2x - 3)^2 = 25
    $$
    
    You may think that you should expand the `2x - 3` out, and then try to solve from there. But that's actually a waste of effort. All you need to do is just solve it as it is, like so:
    
    $$
    2x - 3 = \pm\sqrt{25}
    $$
    
    And then continue on from there.
    

# Reasonings

- **Why is the turning point the way it is?**
    
    When you have the completed square form, like so:
    
    $$
    p(x + q)^2 + r
    $$
    
    The turning point for this is `(-q, r)`. And when you think about it, it’s actually quite obvious why. The `y` in this coordinate is just the **lowest** value the function will go to, and that’s really easy to find out. We know $(x+q)^2$ is always going to be $\ge0$, and therefore the *minimum* and lowest value we can ever get *out of* this function will always be $r$ - so that’s the minimum *y.*
    
    And now that we know the `y`, all we need to do is figure out what the `x` is *at* that point on the curve - so we essentially just rearrange a bit to *solve* what `x` is under the exact same conditions. And you’ll get `x = -q` in that.
    
- **Quadratic formula**
    1. Start with:
        
        $$
        ax^2+bx+c
        $$
        
    2. Factor the `a` from the first two terms so you can complete the square:
        
        $$
        a(x^2+\frac{b}{a}x)+c
        $$
        
    3. Complete the square in the inner section:
        
        $$
        a((x+\frac{b}{2a})^2 - (\frac{b}{2a})^2) + c
        $$
        
    4. Simplify as needed:
        
        $$
        a((x+\frac{b}{2a})^2 - \frac{b^2}{4a^2}) + c
        $$
        
    5. Expand the `a` out:
        
        $$
        a(x + \frac{b}{2a})^2 - \frac{ab^2}{4a^2} + c
        $$
        
    6. The quadratic formula **solves** the quadratic, so to do that, we need to make this equal to `0` and rearrange it as needed.
        
        $$
        a(x + \frac{b}{2a})^2 - \frac{ab^2}{4a^2} + c = 0 \\
        \space \\
        a(x + \frac{b}{2a})^2 =  \frac{ab^2}{4a^2} - c \\
        \space \\
        (x + \frac{b}{2a})^2 = \frac{\frac{ab^2}{4a^2} - c}{a} \\
        \space \\
        (x + \frac{b}{2a})^2 = \frac{ab^2}{4a^3} - \frac{c}{a}
        $$
        
    7. Now, in order to get further, subtract the fractions on the right. To do that, **make the denominators the same,** so both fractions have the same denominator.
        
        $$
        (x + \frac{b}{2a})^2 = \frac{a^2b^2}{4a^4} - \frac{4a^3c}{4a^4} \\
        \space \\
        (x + \frac{b}{2a})^2 = \frac{a^2b^2 - 4a^3c}{4a^4}
        $$
        
    8. Now, you can **simplify** the fraction on the right by factorising $a^2$ out the top and cancelling it out, you can start to see the quadratic formula appear here
        
        $$
        (x + \frac{b}{2a})^2 = \frac{a^2(b^2 - 4ac)}{4a^4} \\
        \space \\
        (x + \frac{b}{2a})^2 = \frac{b^2 - 4ac}{4a^2}
        $$
        
    9. Move the root over
        
        $$
        x + \frac{b}{2a} = \pm\sqrt{ \frac{b^2 - 4ac}{4a^2}}
        $$
        
    10. Use the rule $\sqrt{\frac{a}{b}} = \frac{\sqrt{a}}{\sqrt{b}}$, and simplify as much as possible:
        
        $$
        x + \frac{b}{2a} = \pm\frac{\sqrt{b^2 - 4ac}}{\sqrt{4a^2}} \\
        \space \\
        x + \frac{b}{2a} = \pm\frac{\sqrt{b^2 - 4ac}}{2a}
        $$
        
    11. **One more rearrange!**
        
        $$
        x = - \frac{b}{2a} \pm \frac{\sqrt{b^2 - 4ac}}{2a} \\
        \space \\
        x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}
        $$