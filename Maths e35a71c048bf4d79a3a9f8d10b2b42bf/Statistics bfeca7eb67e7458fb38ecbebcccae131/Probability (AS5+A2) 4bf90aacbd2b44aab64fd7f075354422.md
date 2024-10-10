# Probability (AS5+A2)

The entire Year 1 and Year 2 probability sections can be simplified down to more or less just **three** key points:

1. **Mutually exclusive** - Mutually exclusive means two events can’t happen at the same time, so $P(A \cap B) = 0$.
2. **Independence** - If two events are independent of each other, that means they follow the tree diagrams perfectly, so we can say that:
    1. The probabilities follow the tree diagrams that we’ve used since GCSE, so we know immediately that $P(A \cap B) = P(A) * P(B)$.
    2. We can find the probability of **both** happening by taking the probability of both and subtracting the intersection to get rid of duplicate counting. As seen in the equation: $P(A \cup B) = P(A) + P(B) - P(A \cap B)$.
3. **Conditional probability** - If you see the format $P(A | B) = ...$, that means you’re finding the probability of A given that B has happened. This is essentially **dependent probability**. In this scenario, we can say two things about this situation:
    1. We use the equation $P(A \cup B) = \frac{P(A \cap B)}{P(B)}$. This is also **really obvious** if you just think about something like a two-way table.

(Mr Khalid explains this as 4 because he counts the addition formulae in #2 as their own thing but eh)

# Extra understanding

While the three points above are the key ones, there is some extra concepts you’re expected to be comfortable with, usually underlying questions.

## Shading Venn Diagrams

You definitely need to be able to shade relevant regions of Venn diagrams and you already can, so there’s not *too much* to talk about here! Only thing is Mr Khalid did give us a really good technique: To draw strips going in different directions for *each side* of an operator, then looking at the intersections/whatever of them.

## Two-way tables

The good old GCSE two-way tables where you have “Total” shared across the rows and columns “could” come up hypothetically, allbeit unlikely. The biggest point you mess up with this is ***making them***, but it’s really easy. You just do “A”, “A’” on the rows and “B”, “B’” on the columns.

In this case we know when we have conditional probability and whatnot, we just pay attention to a certain row/column.

## Extra notation

As covered in AS6, you can represent all the outcomes of probability using this notation:

$$
p(x) = \begin{cases}x & \text{For x = 1,2} \\ y & \text{For x = 3,4} \\ 0\end{cases}
$$

This says that for **1 and 2** the probability is $x$, for **3 and 4** the probability is $y$ and for anything else it’s $0$.