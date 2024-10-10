# Hypothesis Testing

*(as seen in AS7, A1, A3 etc.)*

**Hypothesis testing** is a method of testing if something has changed. It works by assuming one scenario (known as $H_0$) is true and checks through a distribution if the results we got from a trial are likely if it is.

We use hypothesis testing when we think something may have changed, and take a test to evaluate if it has.

There are many different types of hypothesis testing: Binomial, normal, one/two tailed, correlation coefficient etc. This is how they all connect.

![Untitled](Hypothesis%20Testing%20fca5792aee2d4d3ba9dab90056a1b037/Untitled.png)

And if we expand all that out:

![Untitled](Hypothesis%20Testing%20fca5792aee2d4d3ba9dab90056a1b037/Untitled%201.png)

The start of hypothesis testing question is *cheap* (not free, but *cheap*) *marks*, you literally just **follow some patterns**.

# The Ends

**$H_0$ and $H_1$**

The start of any hypothesis test answer is the $H_0$ and $H_1$ values. The $H_0$ is our initial scenario that we’re going to be testing under the assumption of, while $H_1$ is the scenario we’re “looking for” that we assume if we see any change.

**Conclusion**

At the end of each question, we need to **reject** $H_0$ if our distribution didn’t work out, because that means it’s probably not falling under $H_0$.

# Binomial/normal testing

For trial-based testing, the $H_0$ will always be $p = ...$ and the $H_1$ will always be $p < ...$ or $p > ...$ or $p \ne ...$.

## Setting Up

![Untitled](Hypothesis%20Testing%20fca5792aee2d4d3ba9dab90056a1b037/Untitled%202.png)

### Let X

State that everytime say “X”, we are referring to the result of our trial. 

### Assuming H0 is true, X ~ …

Here we state what we’re assuming X is distributed on if H0 is true, as per the first sentence. If we later find that it’s really unlikely the trial would turn out the way it did under this, then we give up on H0 and go to H1.

<aside>
💡 You may be asked to view the distribution

</aside>

### If two-tailed, half significance level

For two-tailed tests, you must make sure you half the significance level. This is just a consequence of what the term *significance level* means, it’s not to do with how the distributions and whatnot work.

## Testing $H_0$

From here, there are now *two ways* we can test if our trial seems to fit under $H_0$ or not. One way is the **critical region** path, the other is the **p-value** path. The p-value path is the way I did it all throughout Yr12 and half of Yr13, and it is shorter, but the critical region path is in some way a “nicer way”, and works in more cases. You **do** need to know both though.

### P-value Method

An alternate method to performing hypothesis testing is to **get** the probability of values falling into the test data range and seeing if that’s within 5%.

### Critical Region Method

To test $H_0$ under the critical region method, we just need to find the two **critical values**, then see if the data falls into those regions or not.

**Relevant Critical graph**

For binomial testing, we can use a number line to represent the critical data values.

![BinomialNumLine.png](Hypothesis%20Testing%20fca5792aee2d4d3ba9dab90056a1b037/BinomialNumLine.png)

For normal distribution, we should draw a bell-shaped curve like so:

![NormalDistributionGraph.png](Hypothesis%20Testing%20fca5792aee2d4d3ba9dab90056a1b037/NormalDistributionGraph.png)

**Find the critical value(s)**

For **binomial**, we can get those critical value(s) from the value tables, and for **normal** we can use our calculator in inverse mode to obtain them.

**Check if trial data fits in**

Finally, just check if the trial result lies in these regions.

![Untitled](Hypothesis%20Testing%20fca5792aee2d4d3ba9dab90056a1b037/Untitled%203.png)

# Coefficient testing

Coefficient testing is all about taking a coefficient correlation value, $r$, and finding if the whole population is likely to have a linear correlation. Here the $H_0:\rho = 0$ and $H_1: \rho \ne 0$.

There’s only one method for this, which is as follows.

![Untitled](Hypothesis%20Testing%20fca5792aee2d4d3ba9dab90056a1b037/Untitled%204.png)

<aside>
⚠️ Be careful with the conclusion here we are *looking for a correlation*, don’t talk, in any way, about positive and negative types of correlation, just say there is or isn’t one.

</aside>

# Cumulative Distribution

If you need to find $P(X \ge x)$, just find $1 - P(X \le x)$. 

<aside>
⚠️ If you’re asked to find the **actual significance level**, just add up the probability of each side.

</aside>