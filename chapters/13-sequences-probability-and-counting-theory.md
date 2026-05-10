# Chapter 13 — Sequences, Probability, and Counting Theory

## 1. Chapter Opening

A bank account earns 5% interest, compounded annually, on an initial deposit of $\$1{,}000$. Year 1: $\$1{,}050$. Year 2: $\$1{,}102.50$. Year 3: $\$1{,}157.63$. Each year's balance is the previous year's multiplied by $1.05$. The list — $1000, 1050, 1102.50, 1157.63, \ldots$ — is a *sequence*. Specifically, a *geometric sequence*, where each term is a constant multiple of the one before. Sequences and series — sums of sequences — describe everything from compound interest to population dynamics to mathematical physics.

This final chapter covers sequences and series, the binomial theorem, counting principles (permutations and combinations), and the basics of probability. These topics are *discrete* — about counting and combinations rather than continuous curves — and they complete the foundation that calculus, statistics, and discrete mathematics will build upon.

### Learning objectives

By the end of this chapter, you should be able to:

- **Identify** arithmetic and geometric sequences and write their terms using explicit and recursive formulas.
- **Compute** sums of arithmetic and geometric series, including infinite geometric series.
- **Apply** the binomial theorem to expand $(a + b)^n$.
- **Use** the multiplication principle, permutations, and combinations to count outcomes.
- **Compute** probabilities of simple, mutually exclusive, and complementary events.

### Prerequisites

Algebraic manipulation from Chapter 1; functions from Chapter 3; exponentials from Chapter 6.

---

## 2. Concept 1 — Sequences and Series

A *sequence* is an ordered list of numbers, typically denoted $a_1, a_2, a_3, \ldots, a_n, \ldots$.

A sequence is defined by giving a rule for $a_n$: either an *explicit formula* (telling you $a_n$ in terms of $n$) or a *recursive formula* (telling you $a_n$ in terms of earlier terms).

### Arithmetic sequences

Each term is the previous plus a constant — the *common difference* $d$.

Explicit: $a_n = a_1 + (n-1)d$.

Example: $5, 8, 11, 14, 17, \ldots$ is arithmetic with $a_1 = 5$ and $d = 3$. So $a_n = 5 + 3(n-1) = 3n + 2$.

### Geometric sequences

Each term is the previous times a constant — the *common ratio* $r$.

Explicit: $a_n = a_1 \cdot r^{n-1}$.

Example: $3, 6, 12, 24, 48, \ldots$ is geometric with $a_1 = 3$ and $r = 2$. So $a_n = 3 \cdot 2^{n-1}$.

### Series — sums of sequences

A *series* is the sum of the terms of a sequence. *Sigma notation*:

$$\sum_{i=1}^n a_i = a_1 + a_2 + \ldots + a_n$$

**Arithmetic series.** The sum of the first $n$ terms of an arithmetic sequence:

$$S_n = \frac{n(a_1 + a_n)}{2} = \frac{n}{2}[2a_1 + (n-1)d]$$

**Geometric series.** The sum of the first $n$ terms of a geometric sequence:

$$S_n = a_1 \cdot \frac{1 - r^n}{1 - r}, \quad r \neq 1$$

**Infinite geometric series.** When $|r| < 1$, the sequence terms shrink toward zero, and the series converges:

$$S_\infty = \frac{a_1}{1 - r}$$

If $|r| \geq 1$, the series diverges (sum is infinite or undefined).

### Worked example

Find the sum of the first 20 terms of the arithmetic sequence with $a_1 = 4$ and $d = 3$.

$a_{20} = 4 + 19 \cdot 3 = 61$. Sum: $S_{20} = \frac{20(4 + 61)}{2} = 10 \cdot 65 = 650$.

### Worked example — repeating decimal as infinite series

The repeating decimal $0.\overline{36} = 0.363636\ldots$ is an infinite geometric series:
$$0.36 + 0.0036 + 0.000036 + \ldots = \sum_{n=1}^\infty 0.36 \cdot (0.01)^{n-1}$$

With $a_1 = 0.36$ and $r = 0.01$, since $|r| < 1$:
$$S_\infty = \frac{0.36}{1 - 0.01} = \frac{0.36}{0.99} = \frac{36}{99} = \frac{4}{11}$$

So $0.\overline{36} = 4/11$. The infinite sum gives a clean rational fraction.

---

## 3. Concept 2 — Binomial Theorem and Counting

### Binomial theorem

The expansion of $(a + b)^n$ has $n+1$ terms:

$$(a + b)^n = \sum_{k=0}^n \binom{n}{k} a^{n-k} b^k$$

The coefficients $\binom{n}{k}$ — *binomial coefficients* — count the number of ways to choose $k$ items from $n$:

$$\binom{n}{k} = \frac{n!}{k!(n-k)!}$$

where $n! = n \cdot (n-1) \cdot (n-2) \cdots 2 \cdot 1$ is the *factorial*.

The first few rows of *Pascal's triangle* give the coefficients:

```
                  1
                1   1
              1   2   1
            1   3   3   1
          1   4   6   4   1
        1   5   10  10  5   1
```

Each entry is the sum of the two above it. Row $n$ gives the coefficients of $(a+b)^n$.

### Worked example

Expand $(x + 2)^4$.

$$(x + 2)^4 = \binom{4}{0}x^4 + \binom{4}{1}x^3 \cdot 2 + \binom{4}{2}x^2 \cdot 4 + \binom{4}{3}x \cdot 8 + \binom{4}{4}\cdot 16$$
$$= x^4 + 8x^3 + 24x^2 + 32x + 16$$

### Counting principles

**Multiplication principle.** If task A can be done in $m$ ways and task B in $n$ ways (independently), the total is $mn$.

A pizza shop offers 4 sizes and 6 toppings. Number of ways to order one size with one topping: $4 \cdot 6 = 24$.

**Permutations.** Arrangements of objects where order matters. Permutations of $r$ objects from $n$:

$$P(n, r) = \frac{n!}{(n-r)!}$$

Number of ways 8 horses can finish 1st, 2nd, 3rd in a race: $P(8, 3) = 8!/5! = 8 \cdot 7 \cdot 6 = 336$.

**Combinations.** Selections where order doesn't matter:

$$C(n, r) = \binom{n}{r} = \frac{n!}{r!(n-r)!}$$

Number of 5-card poker hands from a 52-card deck: $C(52, 5) = 2{,}598{,}960$.

The relationship: $P(n,r) = C(n,r) \cdot r!$ — every selection produces $r!$ orderings.

---

## 4. Concept 3 — Probability

The *probability* of an event $E$ is

$$P(E) = \frac{\text{number of outcomes in } E}{\text{number of equally-likely outcomes}}$$

assuming all outcomes are equally likely. Probability is between 0 (impossible) and 1 (certain).

### Basic events

**Single event.** Roll a die. Probability of rolling a 4: $1/6$.

**Multiple favorable outcomes.** Probability of rolling an even number: $3/6 = 1/2$ (three favorable out of six total).

**Complementary events.** $P(\text{not } E) = 1 - P(E)$. Probability of *not* rolling a 4: $1 - 1/6 = 5/6$.

### Combinations of events

**Union (or):** $P(A \cup B) = P(A) + P(B) - P(A \cap B)$.

The subtraction prevents double-counting outcomes that are in both events.

If $A$ and $B$ are *mutually exclusive* (cannot both occur), $P(A \cap B) = 0$ and the formula reduces to $P(A) + P(B)$.

**Intersection (and).** For independent events, $P(A \cap B) = P(A) \cdot P(B)$.

Roll two dice. Probability of two sixes: $\frac{1}{6} \cdot \frac{1}{6} = \frac{1}{36}$.

### Worked example

A jar contains 5 red, 3 blue, 2 green marbles. Draw one at random.

$P(\text{red}) = 5/10 = 1/2$. $P(\text{blue}) = 3/10$. $P(\text{green}) = 2/10$.

$P(\text{red or blue}) = 5/10 + 3/10 = 8/10 = 4/5$ (mutually exclusive: a marble can't be both colors).

$P(\text{not red}) = 1 - 5/10 = 1/2$.

### Worked example — birthday problem

In a room of 23 people, what is the probability that at least two share a birthday?

Easier to compute the complement — probability all 23 have *different* birthdays. The first person has 365 choices; the second 364; the third 363; and so on.

$$P(\text{all different}) = \frac{365 \cdot 364 \cdot 363 \cdots 343}{365^{23}} \approx 0.493$$

So $P(\text{at least one match}) = 1 - 0.493 = 0.507$ — slightly more than half. The number 23 is a famous threshold.

---

## 5. Integration — One Worked Problem

A startup is planning a 3-year financial projection. They expect:
- $\$50{,}000$ in revenue in year 1, growing at 25% per year.
- A one-time grant of $\$30{,}000$ at the start of year 1.
- The grant is invested at 4% annual interest, compounded annually.

(a) What is total revenue across 3 years?

Geometric sequence with $a_1 = 50000$, $r = 1.25$. Sum of three terms:
$$S_3 = 50000 \cdot \frac{1 - 1.25^3}{1 - 1.25} = 50000 \cdot \frac{1 - 1.953125}{-0.25} = 50000 \cdot 3.8125 = 190{,}625$$

(b) What is the grant's value at the end of year 3?

$30000 \cdot 1.04^3 = 30000 \cdot 1.124864 \approx 33{,}746$.

(c) The startup's pitch deck claims they have a 60% chance of profitability by year 3, and a 40% chance the grant fully covers shortfall. What is the probability that *both* events happen (profitable AND grant covers)?

If independent: $0.60 \cdot 0.40 = 0.24$. So 24% chance both occur.

What is the probability *at least one* occurs?

$P(A \cup B) = P(A) + P(B) - P(A \cap B) = 0.60 + 0.40 - 0.24 = 0.76$.

The example uses Concept 1 (geometric series), Concept 2 (compound interest using sequences), and Concept 3 (probability of unions).

[FIGURE: A growing-revenue bar chart for 3 years (50k, 62.5k, 78.125k), beside a compound-interest curve for the grant (30k → 33.7k). The student should notice the geometric structure of both.]

---

## 6. Exercises

### Warm-up

**Exercise 13.1.** Find the 10th term of the arithmetic sequence with $a_1 = 7$ and $d = 4$. Difficulty: low.

**Exercise 13.2.** Find the sum of the first 10 terms of the geometric sequence with $a_1 = 3$ and $r = 2$. Difficulty: low.

**Exercise 13.3.** Compute $\binom{6}{2}$. Difficulty: low.

### Application

**Exercise 13.4.** Convert $0.\overline{72}$ to a fraction using infinite geometric series. Difficulty: medium.

**Exercise 13.5.** Expand $(2x - 1)^3$ using the binomial theorem. Difficulty: medium.

**Exercise 13.6.** A committee of 5 is to be chosen from 10 people. How many possible committees? Difficulty: medium.

**Exercise 13.7.** A card is drawn from a standard 52-card deck. Find the probability that it is (a) a heart, (b) a face card, (c) a heart or a face card. Difficulty: medium.

### Synthesis

**Exercise 13.8.** A loan of $\$10{,}000$ at 6% annual interest is paid off by equal annual payments of $\$2{,}000$. Express the remaining balance after $n$ years as a geometric/arithmetic combination. After how many years is the balance zero? Difficulty: medium-high.

### Challenge

**Exercise 13.9.** Five fair coins are flipped. (a) Probability of exactly 3 heads. (b) Probability of at least 3 heads. Difficulty: high.

---

## 7. Chapter Summary

You can identify arithmetic and geometric sequences, write their terms, and compute sums (including infinite geometric series). You can use the binomial theorem to expand binomial powers. You can apply counting principles (multiplication, permutations, combinations) and compute probabilities of simple events, unions, intersections, and complements.

The single idea that matters most: **discrete mathematics counts; algebra describes.** This chapter completes the algebra-and-trigonometry tour by adding the discrete tools that count and combine — and that scaffold further study in statistics, computer science, and combinatorics.

---

## 8. Connections Forward (Out of the Book)

This is the final chapter. Across thirteen chapters, the book has built the algebraic, geometric, trigonometric, and discrete tools that constitute college algebra. What you do with them — calculus, statistics, engineering, computer science, finance — is the next step. The vocabulary is in place; the work that fills the vocabulary into a career is the work of years that follow this course.

Read on, in everything that comes.

---

### Sources (from chapter source files)

- *College Algebra*, source modules m49443 through m49450 (OpenStax-derived).
