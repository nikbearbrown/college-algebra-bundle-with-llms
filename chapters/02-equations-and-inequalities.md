# Chapter 2 — Equations and Inequalities

## 1. Chapter Opening

A driver pulls up to a toll plaza on the New Jersey Turnpike. The display reads $\$8.50$. The driver punches a $\$10$ bill into the machine, and the change tray spits out $\$1.50$. None of this took a calculator. The driver paid a quantity (the toll), the machine subtracted that from a quantity (the bill), and the difference came back. *Without anyone announcing it, the driver and the machine just solved a linear equation*: $x + 8.50 = 10$, where $x = 1.50$ is the change owed.

Most algebra is this — situations described in words become *equations* in symbols, and *solving* the equation produces the number we wanted to know. The toll-plaza version is trivial; the algebraic moves are the same. Take a relationship you can describe in words ("the change plus the toll equals the bill"), translate it into symbols ($x + 8.50 = 10$), apply rules to isolate the unknown, get the answer ($x = 1.50$). When the relationship is harder — quadratic in the unknown, or inside a square root, or part of an inequality — the rules change but the structure does not. *Set it up, isolate, solve, check.*

This chapter teaches three families of equations and inequalities. Linear equations, where the unknown appears to the first power. Quadratic equations, where the unknown is squared, and which require a small set of named techniques. And inequalities, which substitute "$<$" or "$\geq$" for "$=$" and answer not "what value?" but "which range of values?". Each family has its own moves; the moves rest on the algebraic foundation chapter 1 built.

### Learning objectives

By the end of this chapter, you should be able to:

- **Plot** points on the Cartesian plane and use the distance and midpoint formulas to measure between them.
- **Solve** linear equations in one variable, including rational equations and equations from real-world setups.
- **Solve** quadratic equations using factoring, the square-root property, completing the square, and the quadratic formula, and use the discriminant to predict the number and type of solutions.
- **Recognize** complex numbers as the natural extension when the discriminant is negative, and perform basic operations on them.
- **Solve** linear, compound, and absolute-value inequalities, and express solutions in interval notation.

### Prerequisites

Chapter 1. The properties of real numbers, exponent rules, factoring techniques, and rational-expression simplification all return here as the moves used to solve equations.

### Why this chapter matters

Solving equations is the central activity of college algebra. Almost every quantitative problem you will encounter for the rest of this book — finding zeros of functions, intersecting curves, modeling growth, matching trigonometric identities — collapses, eventually, to an equation that has to be solved. The four quadratic methods you meet here will be applied in every later chapter that involves a polynomial. The inequality techniques will resurface in optimization, in domain analysis, and in any context where the answer is a range rather than a number.

---

## 2. Concept 1 — The Cartesian Plane and Linear Equations

A nautical chart of New York Harbor, c. 1840. Two perpendicular axes are drawn — one running east-west, one running north-south — with the Battery at their intersection. A buoy sits at coordinates *(2.3 mi east, 1.7 mi south)*. Another at *(0.6 mi west, 0.4 mi north)*. The captain who reads the chart can compute, in seconds, the distance between the two buoys: about $3.5$ miles. The chart is not a metaphor. It is *coordinate geometry*, a system invented by René Descartes in the seventeenth century, and the same system underlies everything we will plot in this book [source m51252].

A *Cartesian coordinate system* assigns each point in the plane an ordered pair $(x, y)$ where $x$ is the horizontal distance from a chosen origin and $y$ is the vertical distance. The two axes meet at the *origin*, $(0, 0)$. Positive $x$ runs right, positive $y$ runs up. The two axes divide the plane into four *quadrants*, numbered I (upper-right) through IV (lower-right) counterclockwise.

### Distance and midpoint formulas

Given two points $(x_1, y_1)$ and $(x_2, y_2)$, the *distance* between them is

$$d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$$

This is the Pythagorean theorem in coordinate dress. The horizontal leg of the right triangle has length $|x_2 - x_1|$; the vertical leg has length $|y_2 - y_1|$; the hypotenuse — the straight-line distance — is the formula above.

The *midpoint* of the segment between $(x_1, y_1)$ and $(x_2, y_2)$ is

$$M = \left(\frac{x_1 + x_2}{2}, \frac{y_1 + y_2}{2}\right)$$

This is just the average of the coordinates: average of the $x$'s, average of the $y$'s.

For our two buoys at $(2.3, -1.7)$ and $(-0.6, 0.4)$:
$$d = \sqrt{(2.3 - (-0.6))^2 + (-1.7 - 0.4)^2} = \sqrt{2.9^2 + (-2.1)^2} = \sqrt{8.41 + 4.41} = \sqrt{12.82} \approx 3.58 \text{ mi}$$

The captain's quick estimate matches.

### Solving linear equations in one variable

A *linear equation* in one variable has the general form $ax + b = c$, where $a, b, c$ are real numbers and $a \neq 0$. The variable appears to the first power, multiplied by a number, possibly added to other numbers, and set equal to something. Solving means finding the value of $x$ that makes the statement true.

The technique is one continuous move: *isolate $x$ on one side*. To do that, undo each operation in reverse. If $x$ is multiplied by $5$, divide both sides by $5$. If $7$ has been added to $x$, subtract $7$ from both sides. The legitimacy of these moves comes from the *equality* — whatever you do to one side, do to the other, and the equation remains true.

**Example.** Solve $3x + 7 = 22$.

$$\begin{aligned}
3x + 7 &= 22 \\
3x &= 15 && \text{subtract 7 from both sides} \\
x &= 5 && \text{divide both sides by 3}
\end{aligned}$$

Check: $3(5) + 7 = 22$. ✓

**Equations with the variable on both sides.** Bring the variable terms to one side first.

$$\begin{aligned}
4x - 3 &= 7x + 9 \\
-3 - 9 &= 7x - 4x && \text{subtract } 4x \text{ and } 9 \\
-12 &= 3x \\
x &= -4
\end{aligned}$$

**Rational equations** — equations with variables in denominators — are linear equations in disguise once you clear the fractions. Multiply both sides by the *least common denominator (LCD)* and the fractions disappear.

$$\begin{aligned}
\frac{x}{2} + \frac{x-1}{3} &= 4 \\
6 \cdot \frac{x}{2} + 6 \cdot \frac{x-1}{3} &= 6 \cdot 4 && \text{multiply by LCD} = 6 \\
3x + 2(x - 1) &= 24 \\
3x + 2x - 2 &= 24 \\
5x &= 26 \\
x &= \frac{26}{5}
\end{aligned}$$

**Watch for extraneous solutions.** When you multiply by a denominator that contains the variable, you may introduce solutions that do not satisfy the original equation. After solving, *check* every candidate by substituting back. Any value that makes a denominator zero in the original is *extraneous* — it must be discarded.

### Setting up a linear equation from a word problem

Translation is the hard part. Source m51254 emphasizes a four-step recipe.

**(1) Read carefully and identify the unknown.** Assign it a variable.
**(2) Identify the relationship in plain English.** *Twice the number plus seven is thirty-five.*
**(3) Translate into symbols.** $2x + 7 = 35$.
**(4) Solve, check, and report the answer in the original units.**

**Example.** A car rental costs $\$30$ per day plus $\$0.20$ per mile. If a renter has $\$120$ to spend on a one-day rental, how many miles can they drive?

Let $m$ = miles driven. The total cost is $30 + 0.20m$. Set equal to the budget:
$$30 + 0.20m = 120$$
$$0.20m = 90$$
$$m = 450 \text{ miles}$$

The math is trivial. The setup — converting the rental contract into the expression $30 + 0.20m$ — is the work.

### Trade-off

Linear equations are the simplest kind. The trade-off is that they capture only relationships where the unknown enters once, to the first power, with no products or powers of itself. Most real-world relationships are linear *over short ranges* (small price changes, small distances, short times) and become non-linear over longer ones. Linear models are often used as first approximations because they are easy to solve; the chapters that follow introduce the non-linear families that handle the rest.

### Common misconceptions

**"Multiplying both sides by zero is fine."** Don't. $5 = 5$ is true, but multiplying both sides by 0 gives $0 = 0$, which loses the original. More importantly, in a rational equation, multiplying by a denominator that *equals zero for some value of $x$* introduces extraneous solutions.

**"Adding the same thing to both sides changes the equation."** It doesn't. Equality is preserved under addition, subtraction, multiplication by a nonzero constant, and division by a nonzero constant. These four moves are what isolating $x$ uses.

---

## 3. Concept 2 — Quadratic Equations and Complex Numbers

A baseball leaves a bat at 100 mph at an angle of 30°. How long is it in the air? *That's a quadratic equation.* The height $h$ as a function of time $t$ has the form

$$h(t) = -16t^2 + v_0 t + h_0$$

where $v_0$ is the initial vertical velocity in feet per second, $h_0$ is the initial height, and $-16$ is half the acceleration due to gravity in ft/s² (with sign reversed because positive is up). Setting $h = 0$ asks: when does the ball hit the ground? The answer requires solving a quadratic equation. This kind of equation appears in projectile motion, in orbit calculations, in the geometry of conic sections, in optimization problems — anywhere a relationship involves a squared quantity.

A *quadratic equation* in standard form is
$$ax^2 + bx + c = 0, \quad a \neq 0$$

The four methods for solving it are not interchangeable; each has a context where it is the best choice [source m51256].

### Method 1: Factoring

If you can write $ax^2 + bx + c = (px + q)(rx + s)$, then the *zero-product property* says: a product of factors is zero if and only if at least one factor is zero. So set each factor to zero and solve.

**Example.** Solve $x^2 - 5x + 6 = 0$.

Factor: $(x - 2)(x - 3) = 0$. By the zero-product property, $x - 2 = 0$ or $x - 3 = 0$. So $x = 2$ or $x = 3$.

Factoring is the *fastest* method when the polynomial factors over the integers. Most textbook quadratics are designed to factor; most quadratics in nature are not.

### Method 2: The square-root property

If $x^2 = k$ for some constant $k \geq 0$, then $x = \pm\sqrt{k}$. Both signs are solutions because $(\sqrt{k})^2 = k$ and $(-\sqrt{k})^2 = k$.

**Example.** Solve $(x - 3)^2 = 16$.

By the square-root property, $x - 3 = \pm 4$. So $x = 3 + 4 = 7$ or $x = 3 - 4 = -1$.

The square-root property works when the quadratic is already in the form $(x - h)^2 = k$ — a perfect square equals a constant. When it isn't, you can sometimes *make* it that form, by *completing the square*.

### Method 3: Completing the square

Take a quadratic $x^2 + bx + c = 0$ and rewrite the left side as a perfect square plus a constant.

The trick: $x^2 + bx$ becomes a perfect square when you add $\left(\frac{b}{2}\right)^2$. That is, $x^2 + bx + \left(\frac{b}{2}\right)^2 = \left(x + \frac{b}{2}\right)^2$.

**Example.** Solve $x^2 + 6x - 7 = 0$ by completing the square.

$$\begin{aligned}
x^2 + 6x &= 7 && \text{move constant} \\
x^2 + 6x + 9 &= 7 + 9 && \text{add } (6/2)^2 = 9 \text{ to both sides} \\
(x + 3)^2 &= 16 && \text{factor left side} \\
x + 3 &= \pm 4 && \text{square-root property} \\
x &= -3 \pm 4 \\
x &= 1 \text{ or } x = -7
\end{aligned}$$

Completing the square always works. It is also the *derivation* of the next method, the quadratic formula.

### Method 4: The quadratic formula

For any quadratic $ax^2 + bx + c = 0$ with $a \neq 0$, the solutions are

$$\boxed{x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}}$$

This formula is *completing the square once and for all*, with the answer expressed in terms of $a$, $b$, $c$. Memorize it. Every quadratic yields its solutions through this formula, regardless of whether it factors over the integers.

**Example.** Solve $2x^2 - 7x + 3 = 0$.

Here $a = 2$, $b = -7$, $c = 3$. Substituting:
$$x = \frac{-(-7) \pm \sqrt{(-7)^2 - 4(2)(3)}}{2(2)} = \frac{7 \pm \sqrt{49 - 24}}{4} = \frac{7 \pm \sqrt{25}}{4} = \frac{7 \pm 5}{4}$$

So $x = \frac{12}{4} = 3$ or $x = \frac{2}{4} = \frac{1}{2}$.

### The discriminant

The expression under the square root, $b^2 - 4ac$, is called the *discriminant*. It tells you how many real solutions the quadratic has, before you finish solving.

- If $b^2 - 4ac > 0$: two distinct real solutions.
- If $b^2 - 4ac = 0$: one repeated real solution.
- If $b^2 - 4ac < 0$: no real solutions; two complex solutions.

The discriminant is a quick check before committing to a full computation. If you see $b^2 - 4ac = -7$, you know the equation has no real roots, and you can either stop or proceed into complex numbers.

### Complex numbers — the extension when the discriminant is negative

When $b^2 - 4ac < 0$, the square root in the quadratic formula is the square root of a negative number. Real numbers don't include such values; mathematicians extended the system to handle them.

Define $i = \sqrt{-1}$. Then $i^2 = -1$. A *complex number* is any expression of the form $a + bi$ where $a$ and $b$ are real. The real number $a$ is the *real part*; the real number $b$ is the *imaginary part* [source m51255].

**Operations on complex numbers** mirror polynomial arithmetic in $i$, with the substitution $i^2 = -1$ when it appears.

*Add/subtract:* $(a + bi) + (c + di) = (a + c) + (b + d)i$.

*Multiply:* $(a + bi)(c + di) = ac + adi + bci + bdi^2 = (ac - bd) + (ad + bc)i$.

*Divide:* multiply numerator and denominator by the *conjugate* $\bar z = a - bi$ of the denominator, then simplify:
$$\frac{a + bi}{c + di} \cdot \frac{c - di}{c - di} = \frac{(ac + bd) + (bc - ad)i}{c^2 + d^2}$$

**Example using complex numbers.** Solve $x^2 + 2x + 5 = 0$.

Discriminant: $b^2 - 4ac = 4 - 20 = -16 < 0$. Two complex solutions. Apply the formula:
$$x = \frac{-2 \pm \sqrt{-16}}{2} = \frac{-2 \pm 4i}{2} = -1 \pm 2i$$

The two solutions are $-1 + 2i$ and $-1 - 2i$. Note they are *complex conjugates* of each other — when a real-coefficient quadratic has complex roots, they always come in conjugate pairs.

### Trade-off

Quadratic equations are powerful enough to model many physical situations (projectile motion, area optimization, conic-section geometry) but limited to relationships that involve at most a squared term. Higher-degree polynomial equations exist (chapter 5) and require additional techniques. The four methods given here form a complete toolkit for any quadratic; the choice of method is a matter of efficiency.

### Common misconceptions

**"$\sqrt{a^2} = a$."** Half-right. $\sqrt{a^2} = |a|$. The square root always returns the non-negative root.

**"If $x^2 = 9$, then $x = 3$."** Half-right. The square-root property gives $x = \pm 3$. The "$\pm$" is essential.

**"Complex numbers don't really exist."** They are as well-defined as negative numbers, which were once also called "false" or "fictitious." Complex numbers underlie quantum mechanics, AC electrical engineering, signal processing, and most of modern physics.

**"You always need the quadratic formula."** No — when factoring is fast, factor. Use the formula when factoring is hard or impossible.

---

## 4. Concept 3 — Inequalities and Other Equations

A driver enters a highway with a posted speed limit: $45 \leq v \leq 65$. The same kind of statement — a range of acceptable values rather than a single one — appears all over engineering and finance. *The structural beam must support a load between 1,000 and 5,000 pounds. The bank account must remain above $0$ at all times. The medication must be taken in doses between 200 mg and 800 mg per day.* Each is an *inequality*, and solving them requires modifying the linear-equation technique with a single critical change in rule.

An *inequality* is a statement of the form $a < b$, $a \leq b$, $a > b$, or $a \geq b$. Solving means finding the set of values that make the statement true.

### Interval notation

The solution to an inequality is rarely a single number; it is usually a *range*, written most compactly in *interval notation*. Five conventions:

- $(a, b)$: all real numbers strictly between $a$ and $b$. Endpoints excluded.
- $[a, b]$: all real numbers between $a$ and $b$, including endpoints.
- $[a, b)$: half-open. Includes $a$, excludes $b$.
- $(a, \infty)$: all real numbers greater than $a$. Infinity is always written with an open parenthesis (it is not a number, just a direction).
- $\mathbb{R} = (-\infty, \infty)$.

So the inequality $-2 \leq x < 5$ is written as $[-2, 5)$ in interval notation.

### Properties of inequalities

Most algebraic moves work the same way for inequalities as for equations:

- Add or subtract the same number from both sides: inequality preserved.
- Multiply or divide both sides by the *same positive number*: inequality preserved.

**The exception** — and the one rule worth memorizing carefully:

- Multiply or divide both sides by a *negative number*: **the inequality reverses**.

Example: $-2x < 6$. Divide both sides by $-2$: $x > -3$. The "$<$" flipped to "$>$" because we divided by a negative.

### Solving linear inequalities

The technique is the same as for linear equations — isolate the variable — with the flip rule applied whenever you multiply or divide by a negative.

**Example.** Solve $5 - 2x \geq 11$.

$$\begin{aligned}
5 - 2x &\geq 11 \\
-2x &\geq 6 && \text{subtract } 5 \\
x &\leq -3 && \text{divide by } -2; \text{ flip the inequality}
\end{aligned}$$

In interval notation: $(-\infty, -3]$.

### Compound inequalities

A *compound inequality* combines two inequalities. The two cases:

**"And" (intersection).** Both must be true. Written $a < x < b$ or as the intersection $\{x : a < x \text{ and } x < b\}$.

**"Or" (union).** Either is sufficient. Written as $\{x : x < a \text{ or } x > b\}$.

**Example (and).** Solve $-1 \leq 3x + 2 < 8$.

Subtract $2$ from all three parts: $-3 \leq 3x < 6$. Divide by $3$: $-1 \leq x < 2$. In interval notation: $[-1, 2)$.

### Absolute-value inequalities

The absolute value $|x|$ is the distance of $x$ from $0$. So $|x| < 3$ means *all $x$ within distance 3 of zero*, which is $-3 < x < 3$. And $|x| > 3$ means *all $x$ farther than distance 3 from zero*, which is $x < -3$ or $x > 3$.

The general rules:

$$|x| < a \iff -a < x < a$$
$$|x| > a \iff x < -a \text{ or } x > a$$

**Example.** Solve $|2x - 1| \leq 5$.

$$\begin{aligned}
-5 &\leq 2x - 1 \leq 5 \\
-4 &\leq 2x \leq 6 \\
-2 &\leq x \leq 3
\end{aligned}$$

In interval notation: $[-2, 3]$.

### Other types of equations: radical, rational-exponent, absolute-value

Source m51258 collects the equations that don't fit neatly into linear or quadratic. Three patterns are worth naming.

**Radical equations** have the variable inside a radical. Solve by isolating the radical and squaring (or raising to whatever power undoes the radical), then *check for extraneous solutions* — squaring can introduce them.

$$\sqrt{x + 5} = x - 1 \implies x + 5 = (x-1)^2 = x^2 - 2x + 1 \implies x^2 - 3x - 4 = 0 \implies (x-4)(x+1) = 0$$

Candidates: $x = 4$ or $x = -1$. Check: $\sqrt{4+5} = 3$ and $4 - 1 = 3$ ✓; $\sqrt{-1+5} = 2$ and $-1 - 1 = -2$ ✗. Only $x = 4$ is a real solution.

**Equations with rational exponents.** Treat the rational exponent as an instruction to raise both sides to the reciprocal power. To solve $x^{2/3} = 4$, raise both sides to the $3/2$ power: $x = 4^{3/2} = 8$.

**Absolute-value equations.** $|x - 3| = 5$ means $x - 3 = 5$ or $x - 3 = -5$, so $x = 8$ or $x = -2$. The absolute-value bars say the *distance* is 5; that distance can land on either side.

### Trade-off

Inequalities give you ranges of valid values rather than single solutions, which is what most physical and engineering constraints require. The cost is one extra rule (the flip on negative multiplication) and the need to track interval notation. The investment is small; the application range is large.

### Common misconceptions

**"$|x| < -3$ has solutions."** It doesn't. Absolute values are never negative; no $x$ satisfies $|x| < -3$.

**"You can square both sides of any equation safely."** Squaring can introduce extraneous solutions (it can also lose them, in some configurations). Always check the candidates against the original equation.

**"$\sqrt{x + 5} = -3$ has a solution somewhere."** It doesn't — the principal square root is always non-negative.

---

## 5. Integration — One Worked Problem, All Three Concepts

A homeowner wants to build a fenced rectangular garden against the side of their house. They have $40$ feet of fencing to enclose three sides (the house forms the fourth side). Let $x$ be the side perpendicular to the house. (a) Express the enclosed area as a function of $x$. (b) For what value of $x$ is the area maximized? (c) For what range of $x$ does the area exceed 150 square feet?

**Setup (Concept 1).** With $x$ feet on each of the two perpendicular sides, the parallel side gets $40 - 2x$ feet. The area is

$$A = x(40 - 2x) = 40x - 2x^2$$

This is a polynomial in $x$ — Chapter 1 territory, applied here.

**Where is the area maximized?** This is a *quadratic* in $x$ (Concept 2), and we want the vertex of the parabola. Complete the square:

$$A = -2x^2 + 40x = -2(x^2 - 20x) = -2(x^2 - 20x + 100) + 200 = -2(x - 10)^2 + 200$$

The maximum of $-2(x-10)^2 + 200$ occurs when $(x-10)^2 = 0$, i.e. when $x = 10$. The maximum area is $200$ square feet, with dimensions $x = 10$ ft (the two perpendicular sides) and $40 - 2(10) = 20$ ft (the parallel side).

**For what range does $A > 150$?** This is an *inequality* (Concept 3). Solve:

$$40x - 2x^2 > 150$$
$$-2x^2 + 40x - 150 > 0$$
$$x^2 - 20x + 75 < 0 \quad \text{(divide by } -2\text{; flip the inequality)}$$
$$(x - 5)(x - 15) < 0$$

The product is negative when the two factors have opposite signs. That happens for $5 < x < 15$. In interval notation: $(5, 15)$.

So if the homeowner wants more than 150 square feet, the perpendicular dimension must be between 5 and 15 feet — and the maximum is reached at $x = 10$.

The problem used all three concepts: setting up an algebraic relationship from a word problem (Concept 1), finding a quadratic optimum by completing the square (Concept 2), and solving a quadratic inequality (Concept 3). *The same family of techniques applies whether the rectangle is a garden or a steel beam or a marketing campaign budget.* That is the design philosophy of this chapter — the algebraic moves are general; the contexts that use them are everything.

[FIGURE: A rectangle drawn against a horizontal house line, with the two perpendicular sides labeled $x$ and the parallel side labeled $40 - 2x$. Inside the rectangle, the area $A = x(40-2x)$. Below, a small graph of $A(x) = 40x - 2x^2$ showing a downward parabola with vertex at $(10, 200)$ and zeros at $0$ and $20$. The horizontal line $y = 150$ crosses the parabola at $x = 5$ and $x = 15$, marking the interval where $A > 150$. The student should notice that the geometry, the algebra, and the inequality all describe the same situation from different angles.]

---

## 6. Exercises

### Warm-up

**Exercise 2.1.** *Tests Learning Objective 1.* Plot the points $(2, 3)$, $(-1, 4)$, $(-3, -2)$, and $(0, -1)$. Find the distance between the first and third points. Difficulty: low.

**Exercise 2.2.** *Tests Learning Objective 2.* Solve each linear equation. (a) $4x - 7 = 5$. (b) $\frac{x}{3} + 2 = 7$. (c) $5(x - 2) = 3x + 4$. Difficulty: low.

**Exercise 2.3.** *Tests Learning Objective 3.* For each quadratic, compute the discriminant and state how many real solutions it has. (a) $x^2 - 6x + 9 = 0$. (b) $2x^2 + 3x + 5 = 0$. (c) $x^2 - 5x + 4 = 0$. Difficulty: low.

### Application

**Exercise 2.4.** *Tests Learning Objective 2.* A taxi charges a $\$3.50$ flag drop plus $\$2.40$ per mile. If the total fare is $\$23.90$, how far did the passenger ride? Difficulty: medium.

**Exercise 2.5.** *Tests Learning Objective 3.* Solve by factoring. (a) $x^2 - 9x + 20 = 0$. (b) $3x^2 + 5x - 2 = 0$. (c) $x^2 = 4x$. Difficulty: medium.

**Exercise 2.6.** *Tests Learning Objective 3.* Solve by the quadratic formula. (a) $x^2 + 4x - 1 = 0$. (b) $2x^2 - 3x - 7 = 0$. (c) $x^2 + x + 1 = 0$ (express complex solutions in $a + bi$ form). Difficulty: medium.

**Exercise 2.7.** *Tests Learning Objective 5.* Solve and write the solution in interval notation. (a) $3x - 7 \leq 8$. (b) $-4 < 2x + 1 \leq 11$. (c) $|x - 3| < 5$. (d) $|2x + 1| \geq 7$. Difficulty: medium.

### Synthesis

**Exercise 2.8.** *Tests Learning Objectives 1 and 2.* The midpoint of a segment is $(2, -1)$. One endpoint is $(5, 3)$. Find the other endpoint. Difficulty: medium-high.

**Exercise 2.9.** *Tests Learning Objectives 3 and 4.* A rectangular field with one side along a river is to be enclosed using $200$ meters of fencing. (a) Find the dimensions that maximize the enclosed area. (b) Find the range of widths for which the area exceeds $4{,}000$ m². Difficulty: medium-high.

**Exercise 2.10.** *Tests Learning Objective 3.* A ball is thrown upward from a height of $6$ ft with initial velocity $48$ ft/s. Its height after $t$ seconds is $h(t) = -16t^2 + 48t + 6$. (a) When does it hit the ground? (b) What is the maximum height? (c) For what time interval is the ball above $30$ ft? Difficulty: medium-high.

### Challenge

**Exercise 2.11.** *Tests Learning Objectives 3 and 4.* Find all complex solutions of $x^4 - 16 = 0$. (Hint: factor as a difference of squares first.) Difficulty: high.

**Exercise 2.12.** *Tests Learning Objective 5.* Solve $\frac{x - 1}{x + 2} \geq 2$. Be careful with the sign of the denominator. Difficulty: high.

---

## 7. Chapter Summary

You can do something now you may not have been able to do an hour ago. You can take a real-world situation described in words — a toll booth, a taxi fare, a garden against a house — and translate it into an equation or inequality you can solve. You can plot points and measure between them. You can solve any quadratic equation by choosing the right method (factoring when possible; otherwise the formula). You can recognize when the discriminant tells you to expect real or complex solutions, and you can perform the basic operations on complex numbers. You can solve linear, compound, and absolute-value inequalities and write the solution in interval notation.

The single idea that matters most: **solving an equation is undoing operations until the unknown stands alone.** Every technique in this chapter — clearing fractions, factoring, completing the square, applying the formula, flipping inequality signs — is a controlled application of that one idea. The variety of techniques exists because the variety of equation forms exists; the underlying move is one.

The common mistake to watch for: confusing *algebraic equivalence* with *solution equivalence*. Squaring both sides, multiplying by an expression containing the variable, dividing by a negative — each of these can change the solution set. *Always check candidates against the original equation*, especially when squaring, when multiplying by a denominator, and when working with absolute values.

If you want a test of your understanding: pick any real-world situation that involves a numerical relationship — a recipe scaling, a fuel-economy estimate, a budget allocation — and translate it into an equation. If you can solve it without referring to this chapter, you have the fluency. If you stumble, the part you stumble on is the part to revisit.

---

## 8. Connections Forward

Chapter 1 built algebraic objects; chapter 2 solved equations involving them. Chapter 3 — Functions — generalizes both. A function is, roughly, a rule that produces an output for each input; equations of the form $y = f(x)$ define curves in the plane that we can plot, intersect, transform, and analyze. The linear equations of chapter 2 become *linear functions* in chapter 4; the quadratic equations become the zeros of *polynomial functions* in chapter 5. The structural moves you have just learned — solving, factoring, applying inequality logic — get reapplied as analytical tools on these function families. Read on.

---

### Sources (from chapter source files)

- *College Algebra* with Co-Requisite Skills, source modules m51251 through m51259 (OpenStax-derived).
