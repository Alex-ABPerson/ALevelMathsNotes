# 11. Vectors

A **vector** has both a magnitude and a direction. They can be represented as $\overrightarrow{AB}$ or as a little number, like $a$ (which is typically written as $\underline{a}$ in handwriting). They are comprised of two **components** in 2D, the x component and the y component.

You can visually represent a vector on a diagram using a line with a little arrow in the middle representing the direction it follows.

# Basics

If two vectors are equal, that means they are **parallel** and have **equal length**. So if $\overrightarrow{AB} = \overrightarrow{CD}$, then they parallel and have the length. 

You can add a **scalar** to a vector, represented with the symbol **lambda** $\lambda$, which will change the *magnitude* but not the direction, and therefore it will still be **parallel**. An example is $\frac{1}2\overrightarrow{CD}$, this is parallel but not the same length.

If your scalar is *negative*, then you’ll be going in the reverse direction - and $\overrightarrow{AB} = -\overrightarrow{BA}$, because if you add opposite vectors like these you have to get exactly **0** as you’ve moved nowhere.

You can find a vector by ”following” existing lines you’ve already found.

# Representation

You can describe a vector as the **displacement** relative to the x and y axis using the **column vector** form. This looks like so: $\begin{pmatrix}x \\ y \end{pmatrix}$.

You can add column vectors $\begin{pmatrix}a \\ b \end{pmatrix} + \begin{pmatrix}c \\ d \end{pmatrix} = \begin{pmatrix}a+c \\ b+d\end{pmatrix}$, and you can add scalars to them, $\lambda\begin{pmatrix}a \\ b \end{pmatrix} = \begin{pmatrix}\lambda a \\ \lambda b \end{pmatrix}$.

# Magnitude

The magnitude is essentially the total distance needed to travel across the vector. If the x or you of the vector as 0 it’s very easy to find the magnitude - it’s just the non-zero one. E.g. a vector of $\begin{pmatrix}3 \\ 0 \end{pmatrix}$ just has a magnitude of 3.

However, if it gets more complex you can find the magnitude of $\bold{a} = \begin{pmatrix}x \\ y \end{pmatrix}$ using $\bold{|a|} = \sqrt{x^2+y^2}$ - which is just derived from Pythagorus’ theorem, and really easy to find.

# Unit Vectors

A **unit vector** is a vector of length **1**. There are only two ways you can make a vector that does this and it either goes *up* one or *right* one. And what we *do* is we *call* them $\bold{i}$ and $\bold{j}$ respectively. And then we can *use* these two core vectors to describe more complex ones.

You can represent any vector with the form $p\bold{i} + q\bold{j}$ (or in handwriting terms, $p\underline{i} + q\underline{j}$), as this communicates the “width” and “height” of the vector in one equation.

In addition, one thing you can do is find a unit vector in the same **direction** as another vector - the *magnitude* is just one because it’s a unit vector, but it has the same direction. This is typically represented with the symbol $\hat{a}$ and you can find this using vector using the equation $\hat{a} = \frac{a}{\bold{|a|}}$ . This equation just comes from some common sense - if our line is **5** long, then dividing its size by, well, *5* will bring its size down to 1.

# Position vectors

A **position vector** is a vector describing a point relative to the origin. So if you’re asked for the position vector of $A$, it likely means $\overrightarrow{OA}$ - where $O$ is the origin.