# More Motion (8)

This chapter is all about inserting *vectors* into all the concepts we’ve covered. We introduce a new letter, $r$, which tells us about the **displacement** of an object.

# Constant Velocity Trick

If you have constant velocity happening anywhere, you can always represent that movement through this equation:

$$
r = r_0 + vt
$$

I’m sure I don’t need to spell out how this equation works.

# SUVAT with vectors

We can use the SUVAT equations with vectors, simply by putting bars above everything but time. This results in **four** out of **five** of our SUVAT equations being usable with vectors, with the only equation not usable being $v^2=u^2+at$ as that’s squaring a vector and we can’t do that in A-level (hmmm).

# Projectiles

When you’re asked about projectiles *with motion* you can ***either*** do them by analysing vertical/horizontal separately, *or* you can use the vector formula. 

# Calculus on Vectors

**Differentiation**

You can differentiate vectors by just differentiating the top and bottom ($\frac{dr}{dt} = \dot{r} = \dot{x}\bold{i} + \dot{y}\bold{j}$).

<aside>
🖊️ Saying $\dot{x}$ is shorthand for “differentiate with respect to time”.

</aside>

**Integration**

Integrating vectors has some interesting behaviours. To integrate a vector in the format $a\bold{i} + b\bold{j}$, we just integrate it as one keeping the $\bold{i}$ and $\bold{j}$ intact. Then, you add a $+ c$ to the end (of course), and this constant is a ***vector*** in itself! 

Now from here, we can use boundary conditions to find c. Remember that if you integrated velocity, you’ve formed an equation for $r$. So, you might be given a boundary condition which uses that, in which case you can sub in there and find the value of c. Once you’ve found c, you can collect like terms with everything.