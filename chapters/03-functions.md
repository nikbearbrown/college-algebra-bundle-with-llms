# Chapter 3 — Functions

## 1. Chapter Opening

A weather station in Anchorage records the outdoor temperature at noon every day in October. Day 1: $42°\text{F}$. Day 2: $38°\text{F}$. Day 3: $41°\text{F}$. Day 4: $35°\text{F}$. The pairing is rigid: each day produces *exactly one* temperature reading. Two days never share a reading. Two readings never share a day. *The pairing — day to temperature — is a function.*

Most quantitative relationships in the world are functions. A car's odometer reading is a function of how long you've been driving. The price of a stock is a function of time. The brightness of a star is a function of how far away it is. In each case, an input produces a single output. Once you start looking, functions are everywhere.

This chapter takes the idea seriously. It defines function precisely, develops the notation that makes functions easy to manipulate, and introduces the basic moves — analyzing behavior, combining, transforming, inverting — that the next ten chapters will use repeatedly. The goal is fluency, not novelty. By the end, $f(x)$ should read as naturally as $x + 5$.

### Learning objectives

By the end of this chapter, you should be able to:

- **Determine** whether a given relation is a function (using the vertical-line test for graphs and the input-output rule for sets and equations).
- **Find** the domain and range of a function from its formula, its graph, or its description.
- **Compute** the average rate of change of a function over an interval and identify intervals where the function is increasing, decreasing, or constant.
- **Combine** functions using arithmetic operations and composition, and decompose a composite function into its component functions.
- **Transform** the graph of a function using shifts, reflections, stretches, and compressions, and **find** the inverse of a one-to-one function.

### Prerequisites

Chapters 1 and 2. The arithmetic of functions reuses Chapter 1's algebraic moves; the equation-solving from Chapter 2 returns when finding zeros, evaluating at specific inputs, and inverting.

### Why this chapter matters

After this chapter, every quantitative relationship in college algebra will be expressed as a function. Linear functions in chapter 4 are functions where $f(x) = mx + b$. Polynomial functions in chapter 5 are functions where $f(x)$ is a polynomial. Exponential functions in chapter 6, trigonometric functions in chapters 7–10 — all are particular kinds of functions. *The vocabulary you build here is the working language of every chapter that follows.*

---

## 2. Concept 1 — What a Function Is

A vending machine offers ten products, each at its own button. Press B3 and a candy bar drops out. Press B3 again and the same candy bar (or its identical sibling) drops out. *Press B3 a hundred times and you never get an apple, never get nothing, always get the same candy bar.* That rigidity — same input always produces the same output — is what makes the machine useful. It is also what makes it a *function*.

A **function** is a rule that assigns to each input from a set called the *domain* exactly one output. The set of all possible outputs is called the *range*. Notation:

$$f: A \to B, \quad f(x) = \text{some expression}$$

Here $A$ is the domain, $B$ contains the range, and $f(x)$ is the rule for computing the output from input $x$.

If a relation produces *two different outputs for the same input*, it is *not* a function. The relation that pairs each person with their phone numbers is not a function (a person can have several phone numbers); the relation that pairs each phone number with its primary subscriber is a function (a phone number has one primary subscriber).

### Function notation

The symbol $f(x)$ — read "f of x" — denotes the output that the function $f$ produces when given input $x$. So if $f(x) = 2x + 3$, then $f(4) = 11$, $f(0) = 3$, $f(-2) = -1$. The notation $f$ refers to the rule itself; $f(4)$ refers to the specific value the rule produces at input 4.

Common shapes:

| Shape | Form | Example |
|---|---|---|
| Constant | $f(x) = c$ | $f(x) = 7$ |
| Identity | $f(x) = x$ | $f(x) = x$ |
| Linear | $f(x) = mx + b$ | $f(x) = 3x + 2$ |
| Quadratic | $f(x) = ax^2 + bx + c$ | $f(x) = x^2$ |
| Cubic | $f(x) = ax^3 + \ldots$ | $f(x) = x^3$ |
| Square root | $f(x) = \sqrt{x}$ | $f(x) = \sqrt{x}$ |
| Reciprocal | $f(x) = 1/x$ | $f(x) = 1/x$ |
| Absolute value | $f(x) = \|x\|$ | $f(x) = \|x\|$ |

These are sometimes called the *toolkit functions*. They are the building blocks; most functions you will meet are combinations or transformations of them.

### The vertical-line test

A graph in the $xy$-plane represents a function if and only if every vertical line intersects the graph at most once.

The reasoning: a vertical line $x = a$ asks "what is the output when the input is $a$?" If the line hits the graph at two different points, the input $a$ produces two different outputs — and the rule is not a function.

The graph of $y = x^2$ passes the test: every vertical line hits the parabola at most once. The graph of $x = y^2$ (a sideways parabola) fails: a vertical line at $x = 4$ hits the graph at $y = 2$ and at $y = -2$.

### Domain and range

The *domain* is the set of allowed inputs. The *range* is the set of actual outputs.

For most functions defined by formulas, the domain is "all real numbers except those that make the formula undefined." Two common constraints:

- **Division by zero is undefined.** For $f(x) = \frac{1}{x - 2}$, the domain excludes $x = 2$.
- **Even roots of negatives are not real.** For $f(x) = \sqrt{x - 5}$, the domain requires $x - 5 \geq 0$, so $x \geq 5$.

The range is harder to find from a formula alone — you often need the graph. But for the toolkit functions:

| Function | Domain | Range |
|---|---|---|
| $f(x) = c$ | $(-\infty, \infty)$ | $\{c\}$ |
| $f(x) = x$ | $(-\infty, \infty)$ | $(-\infty, \infty)$ |
| $f(x) = x^2$ | $(-\infty, \infty)$ | $[0, \infty)$ |
| $f(x) = \sqrt{x}$ | $[0, \infty)$ | $[0, \infty)$ |
| $f(x) = 1/x$ | $(-\infty, 0) \cup (0, \infty)$ | $(-\infty, 0) \cup (0, \infty)$ |
| $f(x) = \|x\|$ | $(-\infty, \infty)$ | $[0, \infty)$ |

### Worked example

Determine whether each relation defines $y$ as a function of $x$.

(a) $\{(1, 2), (3, 4), (5, 6), (3, 8)\}$.

The input $x = 3$ pairs with both $y = 4$ and $y = 8$. *Not a function.*

(b) $y = 2x + 3$.

For each $x$, the formula produces exactly one $y$. Yes, function.

(c) $x^2 + y^2 = 25$ (a circle of radius 5).

For $x = 3$, both $y = 4$ and $y = -4$ satisfy. *Not a function.* (The vertical line $x = 3$ hits the circle twice.)

### Trade-off

The function definition is restrictive — it bans relations like the circle, which cannot be a single-valued function but is a perfectly good geometric object. The benefit is that *the operations of algebra and calculus are well-defined on functions*. You can solve $f(x) = 5$, find rates of change, take derivatives, integrate. The restrictions on what counts as a function pay back in the operations the restriction makes possible.

### Common misconceptions

**"$f(x+y) = f(x) + f(y)$."** False in general. $f(x) = x^2$ gives $f(2+3) = 25$ but $f(2) + f(3) = 4 + 9 = 13$. This identity holds only for *linear functions* (and even then, only when the constant term is zero).

**"The domain is whatever I want it to be."** No. The domain is constrained by what makes the formula well-defined. You can sometimes *restrict* a formula's natural domain to model a specific situation, but you cannot extend it.

---

## 3. Concept 2 — How Functions Behave

A car accelerates from a stoplight. After 1 second it has traveled 5 ft; after 2 seconds, 20 ft; after 3 seconds, 45 ft. The position is a function of time. *How fast is it going?* The question asks not about position but about *rate of change* — the derivative idea, presented at the algebra level.

### Average rate of change

For a function $f$ on the interval $[a, b]$, the *average rate of change* is

$$\frac{f(b) - f(a)}{b - a}$$

This is the slope of the line through $(a, f(a))$ and $(b, f(b))$.

For our car at $f(t) = 5t^2$: from $t = 1$ to $t = 3$, the average rate of change is

$$\frac{f(3) - f(1)}{3 - 1} = \frac{45 - 5}{2} = 20 \text{ ft/sec}$$

The average speed over those two seconds is 20 ft/sec. Note this is *not* the speed at any specific moment — that would require calculus — but the average over the interval.

### Increasing, decreasing, constant

A function is *increasing* on an interval if its outputs grow as inputs grow:

$$x_1 < x_2 \implies f(x_1) < f(x_2) \quad \text{for all } x_1, x_2 \text{ in the interval}$$

It is *decreasing* if the inequality reverses: $x_1 < x_2 \implies f(x_1) > f(x_2)$. *Constant* if $f(x_1) = f(x_2)$ for all $x_1, x_2$.

For $f(x) = x^2$, the function is decreasing on $(-\infty, 0)$ (as $x$ goes from $-3$ to $-2$ to $-1$, $f(x)$ goes from $9$ to $4$ to $1$) and increasing on $(0, \infty)$.

### Maxima and minima

A point $(c, f(c))$ is an *absolute maximum* if $f(c) \geq f(x)$ for every $x$ in the domain. *Absolute minimum* with the inequality reversed.

A *local* maximum at $c$ requires only that $f(c) \geq f(x)$ for $x$ in some open interval around $c$, not necessarily across the whole domain. Same idea, smaller scope.

The graph of $f(x) = -x^2 + 4$ has an absolute maximum at $(0, 4)$ — the highest point of the downward parabola. It has no minimum; the parabola goes to $-\infty$ on both sides.

### Worked example

The number of bacteria in a culture (in thousands) after $t$ hours is $N(t) = 50 + 10t - t^2$ for $0 \leq t \leq 12$.

(a) What is the average rate of change of $N$ from $t = 0$ to $t = 5$?

$$\frac{N(5) - N(0)}{5 - 0} = \frac{(50 + 50 - 25) - 50}{5} = \frac{25}{5} = 5 \text{ thousand per hour}$$

(b) When is the population maximum?

$N(t) = -t^2 + 10t + 50 = -(t - 5)^2 + 75$ (completing the square). Maximum at $t = 5$ hours, where $N = 75$ thousand.

(c) When is the population increasing, decreasing?

Increasing on $[0, 5)$, decreasing on $(5, 12]$.

### Trade-off

The average rate of change is a coarse approximation. It tells you the *net* change over an interval, not what happened inside the interval — the function might have shot up, then come back down, with an average that misses the peak. This coarseness is the cost; the benefit is that average rates are easy to compute from two function values, with no calculus required. Calculus refines the idea by taking limits as the interval shrinks to zero, giving the *instantaneous* rate. That refinement is the topic of a later course.

### Common misconceptions

**"A function with a positive average rate of change must be increasing throughout the interval."** No. The average is only the *net* change; the function might decrease, then increase, with a positive net.

**"A maximum is wherever the graph turns around."** The graph might turn around at a *local* maximum without that point being the *absolute* maximum. The distinction is between local and global behavior.

---

## 4. Concept 3 — Building Functions from Other Functions

You have $f(x) = x^2$ and $g(x) = x + 3$. From these, you can build:

- **Sum:** $(f + g)(x) = f(x) + g(x) = x^2 + x + 3$.
- **Product:** $(fg)(x) = f(x) \cdot g(x) = x^2(x + 3) = x^3 + 3x^2$.
- **Composition:** $(f \circ g)(x) = f(g(x)) = (x + 3)^2 = x^2 + 6x + 9$.

The arithmetic operations are straightforward. *Composition* is the new move — apply $g$ first, then apply $f$ to the result. The order matters: $(f \circ g)(x) \neq (g \circ f)(x)$ in general.

For $f(x) = x^2$ and $g(x) = x + 3$:
$$(g \circ f)(x) = g(f(x)) = x^2 + 3$$
which is different from $(f \circ g)(x) = (x + 3)^2 = x^2 + 6x + 9$.

### Domain of a composition

$(f \circ g)(x)$ requires that $x$ is in the domain of $g$ *and* that $g(x)$ is in the domain of $f$. Both constraints must hold.

If $f(x) = \sqrt{x}$ and $g(x) = x - 4$, then $(f \circ g)(x) = \sqrt{x - 4}$, which requires $x - 4 \geq 0$, i.e. $x \geq 4$. The domain of the composition is $[4, \infty)$.

### Decomposing a composite function

Sometimes you need the reverse — given a function, identify its inner and outer parts.

For $h(x) = \sqrt{2x + 1}$, an outer-then-inner decomposition: outer $f(u) = \sqrt{u}$, inner $g(x) = 2x + 1$. Then $h(x) = f(g(x))$.

This decomposition is essential for differentiation in calculus (the chain rule) and useful in algebra for graphing transformed functions.

### Transformations of graphs

Once you know the graph of one function, you can deduce the graphs of related functions through *transformations*. Five basic moves:

**Vertical shift.** $f(x) + c$ shifts the graph up by $c$ units (or down if $c < 0$).
**Horizontal shift.** $f(x - c)$ shifts the graph right by $c$ units (counterintuitively — *minus* in the formula means *right* on the graph).
**Vertical reflection.** $-f(x)$ reflects across the $x$-axis.
**Horizontal reflection.** $f(-x)$ reflects across the $y$-axis.
**Vertical stretch/compression.** $cf(x)$ for $c > 1$ stretches vertically; $0 < c < 1$ compresses.
**Horizontal stretch/compression.** $f(cx)$ for $c > 1$ compresses horizontally; $0 < c < 1$ stretches.

These transformations compose. The graph of $g(x) = -2(x - 3)^2 + 5$, for instance, is the parabola $y = x^2$:
1. Shifted right 3 units (the $x - 3$).
2. Stretched vertically by factor 2 (the leading coefficient).
3. Reflected across the $x$-axis (the negative sign).
4. Shifted up 5 units (the $+ 5$).

The order matters: do horizontal shifts first, then any stretches or reflections, then vertical shifts.

### Even and odd functions

A function is *even* if $f(-x) = f(x)$ for all $x$ in the domain. The graph is symmetric about the $y$-axis. $f(x) = x^2$ and $f(x) = \cos x$ are even.

A function is *odd* if $f(-x) = -f(x)$. The graph is symmetric about the origin. $f(x) = x^3$ and $f(x) = \sin x$ are odd.

Most functions are neither.

### Inverse functions

If $f$ takes input $x$ to output $y$, the *inverse* $f^{-1}$ takes input $y$ back to $x$. Not every function has an inverse — only those that are *one-to-one* (each output is produced by exactly one input). This is checked by the *horizontal-line test*: a horizontal line should intersect the graph at most once.

To find the inverse algebraically:

1. Start with $y = f(x)$.
2. Swap $x$ and $y$.
3. Solve for $y$.
4. The result is $f^{-1}(x)$.

**Example.** Find the inverse of $f(x) = 2x + 3$.

Swap: $x = 2y + 3$. Solve: $y = \frac{x - 3}{2}$. So $f^{-1}(x) = \frac{x - 3}{2}$.

Verify: $f(f^{-1}(x)) = 2 \cdot \frac{x - 3}{2} + 3 = x - 3 + 3 = x$. ✓

### Trade-off

Composition and transformations let you build complex functions from simple ones, but at the cost of careful tracking — domains, order of operations, sign conventions all matter. The horizontal-shift convention ($f(x - c)$ shifts right) trips up many students. The benefit, once you internalize the rules, is that you can recognize the structure of any function in terms of toolkit pieces and transformations.

### Common misconceptions

**"$f(x + 3)$ shifts the graph up."** No. $f(x + 3)$ shifts the graph *left* by 3. To shift *up*, add to the *output*: $f(x) + 3$.

**"$f^{-1}(x) = \frac{1}{f(x)}$."** No. The notation $f^{-1}$ means *inverse function*, not *reciprocal*. The reciprocal would be $\frac{1}{f(x)}$.

**"Every function has an inverse."** No. Only one-to-one functions do. $f(x) = x^2$ has no inverse over its full domain because both $x$ and $-x$ produce the same output.

---

## 5. Integration — One Function, Multiple Lenses

Consider a delivery van whose distance from a depot, in miles, after $t$ hours of driving is $d(t) = 60t - 5t^2$ for $0 \leq t \leq 12$. (After 12 hours, the van returns to the depot.)

**Concept 1 (function basics).** $d(t)$ is a function — each $t$ produces exactly one distance. Domain: $[0, 12]$. Range: by completing the square, $d(t) = -5(t-6)^2 + 180$, so the maximum is 180 miles at $t = 6$. Range: $[0, 180]$.

**Concept 2 (behavior).** $d$ is increasing on $[0, 6)$ (the van is moving outward) and decreasing on $(6, 12]$ (returning). Average speed on $[0, 3]$:

$$\frac{d(3) - d(0)}{3 - 0} = \frac{(180 - 45) - 0}{3} = 45 \text{ mph}$$

Average speed on $[3, 6]$:

$$\frac{d(6) - d(3)}{6 - 3} = \frac{180 - 135}{3} = 15 \text{ mph}$$

The van slows as it approaches the turnaround.

**Concept 3 (transformation).** Suppose the van starts an hour later. The new distance function is $d_{\text{new}}(t) = d(t - 1) = 60(t - 1) - 5(t - 1)^2$. The graph is the original shifted right by 1. The maximum still equals 180, now reached at $t = 7$.

The same function, examined through three concepts, yielded a domain, a maximum, two average speeds, and a transformed version that adapts to a delayed start. *That is functions in college algebra in miniature: a single object, looked at from multiple angles, each angle answering a different question.*

[FIGURE: A graph of $d(t) = 60t - 5t^2$ for $0 \leq t \leq 12$. Downward parabola with vertex at $(6, 180)$ and zeros at $t = 0$ and $t = 12$. Two secant lines drawn: one from $(0, 0)$ to $(3, 135)$, slope 45; another from $(3, 135)$ to $(6, 180)$, slope 15. The student should notice that the slope of the secant line is the average rate of change.]

---

## 6. Exercises

### Warm-up

**Exercise 3.1.** *Tests Learning Objective 1.* Determine whether each relation is a function. (a) $\{(1, 2), (2, 3), (3, 4)\}$. (b) $\{(1, 2), (2, 3), (1, 4)\}$. (c) $y = 3x - 7$. (d) $x = y^2$. Difficulty: low.

**Exercise 3.2.** *Tests Learning Objective 2.* For $f(x) = \frac{x + 2}{x - 5}$, find the domain. Difficulty: low.

**Exercise 3.3.** *Tests Learning Objective 3.* Find the average rate of change of $f(x) = x^2 - 3x$ on the interval $[1, 4]$. Difficulty: low.

### Application

**Exercise 3.4.** *Tests Learning Objective 4.* Let $f(x) = 2x + 1$ and $g(x) = x^2$. Find $(f \circ g)(x)$, $(g \circ f)(x)$, and evaluate each at $x = 2$. Difficulty: medium.

**Exercise 3.5.** *Tests Learning Objective 5.* Describe the graph of $g(x) = 2(x + 1)^2 - 3$ as a transformation of $y = x^2$. Difficulty: medium.

**Exercise 3.6.** *Tests Learning Objective 5.* Find the inverse of $f(x) = \frac{x + 3}{2}$. Verify by composition. Difficulty: medium.

### Synthesis

**Exercise 3.7.** *Tests Learning Objectives 2 and 3.* The temperature in a city, in $°F$, $t$ hours after midnight is modeled by $T(t) = -0.4(t - 14)^2 + 75$ for $0 \leq t \leq 24$. (a) What is the maximum temperature, and when does it occur? (b) On what intervals is the temperature increasing? (c) What is the average rate of change from $t = 6$ to $t = 14$? Difficulty: medium-high.

**Exercise 3.8.** *Tests Learning Objective 5.* Decompose $h(x) = \sqrt{(2x + 1)^3}$ into three functions: $h = f \circ g \circ k$. Difficulty: medium-high.

### Challenge

**Exercise 3.9.** *Tests Learning Objectives 4 and 5.* Find $f^{-1}$ for $f(x) = \frac{2x + 3}{x - 1}$, and state the domain and range of both $f$ and $f^{-1}$. Difficulty: high.

---

## 7. Chapter Summary

You can do something now you may not have been able to do an hour ago. You can read $f(x)$ as the output a function produces given input $x$, and you can determine whether a relation is a function by checking if any input has more than one output. You can find domain and range from a formula. You can compute average rate of change between two points and identify intervals where a function is increasing or decreasing. You can compose two functions, decompose a composite, transform a graph using shifts and reflections and stretches, and find the inverse of a one-to-one function.

The single idea that matters most: **a function is a single-valued rule, and most operations of algebra and calculus are defined precisely so they preserve that single-valuedness.** Composition produces a function. Inversion produces a function (when the original is one-to-one). Transformation produces a function. The whole edifice of mathematical analysis is built on the function concept.

The common mistake to watch for: confusing $f$ with $f(x)$. The former is the rule; the latter is the value of the rule at input $x$. The distinction matters when you are composing, transforming, or inverting — operations on rules, not on values.

---

## 8. Connections Forward

Chapter 4 introduces *linear functions* — the simplest nontrivial family — and develops slope, intercepts, and the equation forms (slope-intercept, point-slope) that make linear functions tractable. Chapter 5 generalizes to polynomial and rational functions. Chapter 6 introduces exponentials and logarithms. Each chapter is, in effect, a deep study of one family of functions, using the framework you just built.

---

### Sources (from chapter source files)

- *College Algebra* with Co-Requisite Skills, source modules m51260 through m51268 (OpenStax-derived).
