# Measures (2)

The **median** is the centre value in data, the **mean** is an average value of the data and the **mode** is the **most common** value!

<aside>
⚠️ Be very careful not to mistake the mode for the **highest value** - it is the **most common** value!

</aside>

A **quartile** is data at quarter positions. There’s the **lower quartile** ($Q_1$), the **median** ($Q_2$) and the **upper quartile** ($Q_3$). You can find the lower and upper quartile by multiplying the number of items by $\frac{1}4$ and $\frac{3}4$ respectively.

A **percentile**, is a percentage-based positions. E.g. $P_{36}$.

The **variance** is a measure of how far each point deviates from the mean. It’s measured in the unit *squared*, so gives a rough idea. This is represented with the symbol $\sigma^2$.

The **standard deviation** is just the variance *rooted,* so it’s actually measured in the units of the data. This is represented with the symbol $\sigma$.

# Simple Data

**Mean**

You can find the mean easily with the regular equation:

$$
\overline{x} = \frac{\sum x}n
$$

**Quartiles**

When you find quartiles, you need to **+ 1** to your number of items before doing any sort of division on it because that way if you have 11 items, you’ll get a value like $12/2$, telling you to get the 6th item - which would be correct. If you have a decimal result (e.g. it was an even number of items) - you can find the value exactly *between* the two pieces of data.

You can find the **median** value by taking the number of items, **adding one to it**, and then dividing by 2.

You can find the **lower and upper quartile** by taking the number of items, **adding one to it**, and then dividing by 4 (and multiplying by 3 for upper). Then, if your number is a decimal... You have to get the value exactly between, otherwise take that item.

<aside>
💡 You need the **+ 1**

</aside>

**Variance**

You can calculate the variance of this data using this equation:

$$
\sigma^2 = \frac{\sum x^2}n - \overline{x}^2
$$

# Frequency Data

**Mean**

You can find the mean in frequency data easily with the equation:

$$
\overline{x} = \frac{\sum fx}{\sum f}
$$

**Quartiles**

You can find the quartiles using the **cumulative frequency**. You don’t need to add one in this situation. Simply add the cumulative frequency and then divide by 2 or 4. 

**Variance**

You can calculate the variance of this data using this equation:

$$
\sigma^2 = \frac{\sum fx^2}{\sum f} - \overline{x}^2
$$

# Grouped data

**Estimated Mean & Variance**

You can calculate the mean/variance for grouped data the same way you do for frequency, just use the *midpoint* of the class intervals as the $x$.

<aside>
↔️ If your class width is an *odd number*, use the context to determine where to place the midpoint. E.g. if it’s ages you might need to round down.

</aside>

**Quartiles**

To find the quartiles, use cumulative frequency to find the position, and then use **interpolation** to find the value at that position.

# Interpolation

Interpolation is a technique you can use for estimating values *within* data at a certain point - it is similar to extrapolation.

<aside>
⚠️ You cannot perform interpolation on discrete data - just keep an eye on the marks a question needs and use your best judgement there.

</aside>

One way you can do it is using a **graph**. However, there is a mathematical way of doing it as well - and you need to know how to do that. It’s quite a simple and logical process:

1. Determine between **which groups** what you’re trying to find will go, and draw a graph like this representing it:
    
    ![Interpolation.png](Measures%20(2)%2059854ccad0cd4c9bb5395fbfeca2b1f0/Interpolation.png)
    
    *(where the $C$ values are the cumulative frequencies and the $V$values are the values around each group)*
    
2. Then, we need to figure out proportionally *how far* between the two the $C$ is, just some simple subtraction and division.
3. And finally, we can multiply the distance between the top two by this proportional amount.

Ez.

# Coding

Coding is when you simplify your data down by a given formula. You usually code values using a formula like this:

$$
y = \frac{x - a}{b}
$$

When you code values, you can still find the original mean and standard deviation using some very simple facts.

With the **mean**, the *divide by b* **and** the translation *both* affect the value, so to find the mean after coding, it’s $\overline{y} = \frac{\overline{x} - a}b$.

With the **standard deviation**, the translation actually doesn’t affect the spread at all, since everyone just moves up/down, so it’s only really affected by the division, so $\sigma y = \frac{\sigma x}b$.