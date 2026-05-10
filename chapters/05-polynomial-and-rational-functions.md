# Chapter 5 — Polynomial and Rational Functions

## 1. Chapter Opening

Galileo drops a cannonball from the Tower of Pisa in 1589 (the experiment may be apocryphal but the physics is real). The ball falls. He measures the distance fallen at one second, two seconds, three seconds. Plot the data: $16$ ft, $64$ ft, $144$ ft. The pairing is not linear — the differences grow. The relationship is *quadratic*: $d(t) = 16t^2$. Every additional second adds more distance than the second before, because gravity is accelerating the ball.

A quadratic is the simplest *nonlinear* function. Its graph is a parabola. Beyond quadratic lie cubic, quartic, and higher-degree polynomials — each adding more flexibility, more zeros, more turning points. Beyond polynomials lie *rational functions*: polynomials divided by polynomials, with the new behavior that they can be undefined at certain inputs and shoot off to infinity near them.

This chapter develops the technique for working with these richer function families. Quadratics first (the simplest case, and the one that appears in projectile motion, optimization problems, and conic sections). Polynomial functions of higher degree (with their full set of zeros and end behavior). Rational functions (with their asymptotes and discontinuities).

### Learning objectives

By the end of this chapter, you should be able to:

- **Identify** the vertex, axis of symmetry, intercepts, maximum or minimum, and end behavior of a quadratic function.
- **Sketch** the graph of a polynomial function from its formula, including its zeros (with multiplicities), end behavior, and turning points.
- **Find** the zeros of a polynomial function using factoring, the rational zero theorem, and synthetic division.
- **Identify** the domain, vertical and horizontal asymptotes, and intercepts of a rational function and sketch its graph.
- **Solve** applications involving polynomial and rational functions, including direct, inverse, and joint variation.

### Prerequisites

Chapters 1–4. The factoring techniques from Chapter 1, the equation-solving from Chapter 2, the function concept from Chapter 3, and the linear-modeling logic from Chapter 4 all return as tools applied to richer functions.

---

## 2. Concept 1 — Quadratic Functions

A quadratic function has the form

$$f(x) = ax^2 + bx + c, \quad a \neq 0$$

The graph is a *parabola*. If $a > 0$, the parabola opens upward (cup-shaped). If $a < 0$, downward (cap-shaped). The parabola has a single *vertex* — the lowest point if it opens up, the highest if it opens down.

### Finding the vertex

Two ways to locate the vertex.

**By formula.** The vertex of $f(x) = ax^2 + bx + c$ is at

$$x = -\frac{b}{2a}, \quad y = f\!\left(-\frac{b}{2a}\right)$$

**By completing the square.** Rewrite $f(x)$ in *vertex form*:

$$f(x) = a(x - h)^2 + k$$

The vertex is $(h, k)$. The parabola opens up if $a > 0$, down if $a < 0$.

**Example.** Find the vertex of $f(x) = 2x^2 - 8x + 5$.

By formula: $x = -\frac{-8}{2 \cdot 2} = 2$. Then $f(2) = 8 - 16 + 5 = -3$. Vertex: $(2, -3)$.

By completing the square: $f(x) = 2(x^2 - 4x) + 5 = 2(x^2 - 4x + 4 - 4) + 5 = 2(x - 2)^2 - 8 + 5 = 2(x - 2)^2 - 3$. Vertex: $(2, -3)$. Same answer.

### Maximum or minimum

Because the vertex is the extreme point, it gives the maximum or minimum value of the function.

If $a > 0$: minimum value is $k$ (the $y$-coordinate of the vertex), occurring at $x = h$.

If $a < 0$: maximum value is $k$, occurring at $x = h$.

This is the key fact for *optimization problems*. Set up the quantity to be optimized as a quadratic in one variable; the vertex tells you the answer.

**Example — fencing optimization.** A farmer has 100 ft of fencing to enclose a rectangular pen. What dimensions maximize the area?

Let $x$ be one side. The perimeter is $2x + 2y = 100$, so $y = 50 - x$. Area $A(x) = x(50 - x) = -x^2 + 50x$.

This is a downward parabola. Vertex: $x = -\frac{50}{2 \cdot (-1)} = 25$. So $y = 25$ as well, and $A = 625$ ft². The pen is a $25 \times 25$ square — a special case of a general result: *for a fixed perimeter, the rectangle of maximum area is a square*.

### Trade-off

Quadratic functions are powerful enough to describe many physical phenomena (projectile motion, area optimization, parabolic mirrors) but limited to a single bend. Functions with multiple bends require higher-degree polynomials, the topic of the next concept.

---

## 3. Concept 2 — Polynomial Functions

A *polynomial function* has the form

$$f(x) = a_n x^n + a_{n-1} x^{n-1} + \ldots + a_1 x + a_0$$

The largest exponent $n$ is the *degree*. The coefficient $a_n$ is the *leading coefficient*. The constant $a_0$ is the *y-intercept*: $f(0) = a_0$.

### End behavior

What happens as $x \to \pm\infty$? The end behavior of a polynomial is determined entirely by its *leading term* $a_n x^n$.

| Degree | Leading coefficient | Left end | Right end |
|---|---|---|---|
| Even ($n = 2, 4, 6, \ldots$) | Positive | $+\infty$ | $+\infty$ |
| Even | Negative | $-\infty$ | $-\infty$ |
| Odd ($n = 1, 3, 5, \ldots$) | Positive | $-\infty$ | $+\infty$ |
| Odd | Negative | $+\infty$ | $-\infty$ |

So $f(x) = -2x^4 + \ldots$ goes to $-\infty$ on both ends; $f(x) = x^3 + \ldots$ goes from $-\infty$ on the left to $+\infty$ on the right.

### Zeros and multiplicities

A *zero* of a polynomial is a value $x = r$ where $f(r) = 0$. By the *factor theorem*, $r$ is a zero if and only if $(x - r)$ is a factor of $f(x)$.

The *multiplicity* of a zero is the number of times its factor appears. If $f(x) = (x - 2)^3 (x + 1)$, the zero $x = 2$ has multiplicity 3 and $x = -1$ has multiplicity 1.

Multiplicity affects the *graph behavior at the zero*:

- **Odd multiplicity:** the graph crosses the $x$-axis at the zero.
- **Even multiplicity:** the graph touches the $x$-axis but does not cross (it "bounces" off).

### Turning points

A polynomial of degree $n$ has at most $n - 1$ turning points (places where the graph changes from increasing to decreasing or vice versa). A cubic has at most 2 turning points; a quartic has at most 3.

### Finding zeros

Three techniques for finding zeros of a polynomial:

**1. Factoring.** If you can factor the polynomial, set each factor to zero. Works for low-degree polynomials with rational zeros.

**2. The rational zero theorem.** If a polynomial with integer coefficients has a rational zero $\frac{p}{q}$ (in lowest terms), then $p$ divides the constant term and $q$ divides the leading coefficient. This gives a finite list of *candidates* to test.

**Example.** Find the zeros of $f(x) = 2x^3 - 5x^2 - 4x + 3$.

Constant term 3, leading coefficient 2. Possible rational zeros: $\pm 1, \pm 3, \pm \frac{1}{2}, \pm \frac{3}{2}$. Test $x = 3$: $f(3) = 54 - 45 - 12 + 3 = 0$. So $x = 3$ is a zero, and $(x - 3)$ is a factor.

**3. Synthetic division.** Divide by $(x - r)$ to factor out a known zero. For $f(x) = 2x^3 - 5x^2 - 4x + 3$ divided by $(x - 3)$:

$$2x^3 - 5x^2 - 4x + 3 = (x - 3)(2x^2 + x - 1) = (x - 3)(2x - 1)(x + 1)$$

Zeros: $x = 3, x = \frac{1}{2}, x = -1$.

### The fundamental theorem of algebra

A polynomial of degree $n$ has *exactly* $n$ zeros, counting multiplicities and including complex zeros. So a cubic has 3 zeros, a quartic has 4, etc. Some may be repeated; some may be complex.

### Worked example

Sketch the graph of $f(x) = (x + 2)(x - 1)^2(x - 3)$.

**Zeros:** $-2$ (multiplicity 1), $1$ (multiplicity 2), $3$ (multiplicity 1).

**Behavior at zeros:** $-2$ and $3$ have odd multiplicity → graph crosses. $1$ has even multiplicity → graph bounces.

**Degree:** $1 + 2 + 1 = 4$. Even degree.

**Leading coefficient:** $+1$ (multiplying out). Even degree, positive leading → graph goes to $+\infty$ on both ends.

**Y-intercept:** $f(0) = 2 \cdot 1 \cdot (-3) = -6$.

So the graph: starts at $+\infty$ on the left, comes down, crosses at $x = -2$, bounces off the $x$-axis at $x = 1$, goes back down (or stays low), crosses at $x = 3$, then heads to $+\infty$. With $y$-intercept $-6$.

### Trade-off

Polynomial functions are flexible enough to model many real-world phenomena (population dynamics, projectile motion, economic curves) but their flexibility is bounded by degree. A polynomial of degree $n$ has at most $n - 1$ turning points; a sinusoidal pattern with infinitely many oscillations cannot be captured by any polynomial. Trigonometric functions (chapters 7–9) handle that.

---

## 4. Concept 3 — Rational Functions

A *rational function* is a ratio of two polynomials:

$$f(x) = \frac{p(x)}{q(x)}, \quad q(x) \not\equiv 0$$

The denominator can be zero at specific points; at those points, the function is *undefined*. This single feature — undefined points — gives rational functions their characteristic shape: vertical asymptotes, where the function shoots to $\pm\infty$ near the bad inputs.

### Domain

The domain excludes any $x$ where $q(x) = 0$.

For $f(x) = \frac{x + 1}{x^2 - 4} = \frac{x + 1}{(x-2)(x+2)}$: domain is $(-\infty, -2) \cup (-2, 2) \cup (2, \infty)$.

### Vertical asymptotes

A *vertical asymptote* is a vertical line $x = c$ that the graph approaches but never crosses. They occur where the denominator is zero (after simplifying) and the numerator is nonzero.

For $f(x) = \frac{x + 1}{(x-2)(x+2)}$: vertical asymptotes at $x = 2$ and $x = -2$ (the numerator is nonzero at both points).

### Removable discontinuities (holes)

If a factor cancels between numerator and denominator, the function has a *hole* at that point — not a vertical asymptote.

For $f(x) = \frac{x^2 - 4}{x - 2} = \frac{(x-2)(x+2)}{x - 2} = x + 2$ for $x \neq 2$. The function equals $x + 2$ everywhere except at $x = 2$, where it is undefined. The graph is the line $y = x + 2$ with a hole at $(2, 4)$.

### Horizontal asymptotes

A *horizontal asymptote* is a horizontal line $y = c$ that the graph approaches as $x \to \pm\infty$. Determined by comparing degrees of numerator and denominator.

Let $\deg(p) = n$ and $\deg(q) = m$.

- $n < m$: horizontal asymptote $y = 0$.
- $n = m$: horizontal asymptote $y = \frac{a_n}{b_m}$ (ratio of leading coefficients).
- $n > m$: no horizontal asymptote (graph goes to $\pm\infty$). If $n = m + 1$, there is a *slant asymptote* (a non-horizontal line).

**Example.** $f(x) = \frac{2x^2 + 3}{x^2 - 4}$: degrees equal, ratio of leading coefficients $\frac{2}{1} = 2$. Horizontal asymptote $y = 2$.

### Worked example

Graph $f(x) = \frac{x - 1}{x + 2}$.

**Domain:** $x \neq -2$.

**Vertical asymptote:** $x = -2$ (denominator zero, numerator nonzero).

**Horizontal asymptote:** Degrees equal. Ratio of leading coefficients $\frac{1}{1} = 1$. Asymptote $y = 1$.

**X-intercept:** Numerator zero when $x = 1$. So $(1, 0)$.

**Y-intercept:** $f(0) = \frac{-1}{2} = -\frac{1}{2}$. So $(0, -\frac{1}{2})$.

The graph has two branches separated by $x = -2$. The right branch (for $x > -2$) passes through $(0, -\frac{1}{2})$ and $(1, 0)$, then approaches $y = 1$ from below as $x \to \infty$. The left branch (for $x < -2$) approaches $y = 1$ from above as $x \to -\infty$ and shoots to $-\infty$ as $x \to -2^-$.

### Variation — a special case of rational functions

**Direct variation:** $y = kx$. $y$ is proportional to $x$.

**Inverse variation:** $y = \frac{k}{x}$. $y$ is inversely proportional to $x$.

**Joint variation:** $y = kxz$ (or with more variables). $y$ varies with multiple quantities at once.

The constant $k$ is the *constant of variation*, found by plugging in one known data point.

**Example.** Light intensity $I$ varies inversely as the square of distance $r$: $I = \frac{k}{r^2}$. If $I = 100$ at $r = 5$ m, find $I$ at $r = 10$ m.

$100 = \frac{k}{25}$, so $k = 2500$. At $r = 10$: $I = \frac{2500}{100} = 25$. Doubling the distance reduces intensity to one-fourth — the *inverse-square law*.

### Trade-off

Rational functions are flexible enough to model relationships with discontinuities — situations where a quantity blows up near a critical input (light intensity at distance zero, the price of a good when supply approaches zero). The cost is that you must be careful about the domain; the "interesting" inputs are exactly where the function is undefined, and analyzing the behavior near them requires the asymptote machinery.

---

## 5. Integration — One Worked Problem

A rectangular box is to be built from a flat sheet of cardboard $20$ inches wide and $30$ inches long, by cutting equal squares of side $x$ from the four corners and folding up the sides.

(a) Express the box's volume $V$ as a function of $x$.

The box dimensions: length $30 - 2x$, width $20 - 2x$, height $x$. So:
$$V(x) = x(30 - 2x)(20 - 2x) = x(600 - 100x + 4x^2) = 4x^3 - 100x^2 + 600x$$

This is a *cubic polynomial* in $x$.

(b) What is the domain (in context)?

Physical constraints: $x > 0$ (cuts must be positive), $x < 10$ (otherwise width $20 - 2x \leq 0$). Domain: $(0, 10)$.

(c) For what value of $x$ is the volume maximized?

This requires calculus (or graphing). For our purposes, plot the cubic on $(0, 10)$. The cubic crosses zero at $x = 0$ and $x = 10$ (and at $x = 15$, outside the domain). The maximum on $(0, 10)$ is at some interior point. Numerical inspection or calculus shows the maximum at $x \approx 3.92$, with $V \approx 1056$ in³. The point: *cubic functions can model real geometric optimization problems*, and the graph (with its turning points and zeros) is the analytic tool.

(d) Sketch the graph of $V(x)$ on its domain.

Cubic, leading coefficient $+4$, so end behavior: $-\infty$ left, $+\infty$ right (outside the domain). On the domain $(0, 10)$: starts at $V(0) = 0$, rises to a peak around $x \approx 3.92$ (max volume ~1056), then falls to $V(10) = 0$.

The example used Concepts 1 (quadratic-like analysis), 2 (cubic polynomial behavior), and the principle that polynomial functions model geometric structure directly.

[FIGURE: Two-panel figure. Top: a flat rectangle 30 × 20 with squares of side $x$ marked at each corner; arrows indicate folding. Bottom: a graph of $V(x) = 4x^3 - 100x^2 + 600x$ on $[0, 10]$, with the maximum point at $x \approx 3.92$ marked. The student should notice that the polynomial structure of the volume reflects the geometric structure of the box.]

---

## 6. Exercises

### Warm-up

**Exercise 5.1.** Find the vertex and the maximum or minimum of $f(x) = -2x^2 + 8x - 3$. Difficulty: low.

**Exercise 5.2.** State the end behavior of $f(x) = -3x^4 + 5x^2 + 2$. Difficulty: low.

**Exercise 5.3.** Find the zeros and their multiplicities of $f(x) = x(x - 2)^2(x + 5)$. Difficulty: low.

### Application

**Exercise 5.4.** A ball is thrown upward from a height of 5 ft with initial velocity 64 ft/s. Its height is $h(t) = -16t^2 + 64t + 5$. (a) When does it reach maximum height? (b) What is that height? (c) When does it hit the ground? Difficulty: medium.

**Exercise 5.5.** Find all zeros of $f(x) = 2x^3 - 3x^2 - 11x + 6$. Difficulty: medium.

**Exercise 5.6.** Identify all asymptotes (vertical and horizontal) and intercepts of $f(x) = \frac{2x^2 - 8}{x^2 - 1}$. Difficulty: medium.

### Synthesis

**Exercise 5.7.** A rectangular pen is to be enclosed using 200 ft of fencing along three sides (a barn forms the fourth side). Find dimensions that maximize area. Difficulty: medium-high.

**Exercise 5.8.** Sketch the graph of $f(x) = (x + 1)^2(x - 3)$. Indicate zeros, multiplicities, end behavior, and y-intercept. Difficulty: medium-high.

### Challenge

**Exercise 5.9.** A 100 m × 60 m rectangular field has a uniform path of width $w$ around its border. The remaining (un-pathed) area is $5{,}000$ m². Find $w$. Difficulty: high.

---

## 7. Chapter Summary

You can do something now you may not have been able to do an hour ago. You can take any quadratic and find its vertex, max/min, zeros, and end behavior. You can sketch the graph of a polynomial of any degree by combining its end behavior, its zeros (with multiplicities), and its $y$-intercept. You can find zeros using factoring, the rational zero theorem, and synthetic division. You can identify the asymptotes of a rational function, sketch its graph, and recognize variation problems as special rational structures.

The single idea that matters most: **the graph of a polynomial or rational function is determined by a small set of features — degree, leading coefficient, zeros and multiplicities, asymptotes, intercepts.** Once you know these, the graph follows. The rest of the chapter is technique for finding the features.

The common mistake to watch for: confusing zeros with $y$-intercepts. The $x$-intercepts (zeros) are where $y = 0$. The $y$-intercept is where $x = 0$. They answer different questions.

---

## 8. Connections Forward

Chapter 6 introduces *exponential and logarithmic* functions — function families that polynomial functions cannot capture. Bacterial growth, radioactive decay, compound interest, and earthquake magnitudes all live in this family. The techniques developed for polynomials and rational functions transfer in spirit; the new family adds a fundamentally new shape to the function vocabulary.

---

### Sources (from chapter source files)

- *College Algebra* with Co-Requisite Skills, source modules m51273 through m51281 (OpenStax-derived).
