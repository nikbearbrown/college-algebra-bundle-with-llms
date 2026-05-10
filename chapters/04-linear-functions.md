# Chapter 4 — Linear Functions

## 1. Chapter Opening

A heating bill in Vermont in January reads: $\$45$ base service charge plus $\$1.20$ per gallon of oil delivered. The homeowner who orders $80$ gallons pays $45 + 1.20 \cdot 80 = \$141$. The homeowner who orders $120$ gallons pays $\$189$. The relationship between gallons and bill is *linear*: a constant base, plus a constant rate per unit. The graph of the bill against gallons is a straight line.

Linear relationships are everywhere. Cell-phone plans (base + per-minute charge). Wages (hourly rate × hours, possibly with overtime). Driving distance (speed × time, when speed is constant). Anytime a relationship has the form *fixed amount + constant rate × variable*, it is linear. This chapter develops the technique for working with such relationships — recognizing them, writing them down, graphing them, and using them to model data.

### Learning objectives

By the end of this chapter, you should be able to:

- **Identify** a linear function from a formula, a table, or a graph, and determine whether it is increasing, decreasing, or constant.
- **Compute** the slope of a line from two points and **write** the equation of a line in slope-intercept, point-slope, and standard forms.
- **Build** a linear model from a verbal description of a real-world situation.
- **Identify** parallel and perpendicular lines from their slopes.
- **Recognize** when data is approximately linear, draw a line of best fit, and interpret slope and intercept in context.

### Prerequisites

Chapters 1–3. Linear functions are a special case of the function concept from Chapter 3, with formula $f(x) = mx + b$.

### Why this chapter matters

Linear models are the workhorse of applied mathematics, science, and engineering. They are not the most accurate for every situation, but they are the most tractable, the most interpretable, and the most teachable. Most more-sophisticated models start from a linear approximation and build complexity from there. Master the linear case here, and the rest of college algebra has a baseline to compare against.

---

## 2. Concept 1 — Linear Functions: Form, Slope, and Intercept

A linear function is one whose graph is a straight line. Algebraically:

$$f(x) = mx + b$$

The constant $m$ is the *slope*: the rate at which the function changes per unit of input. The constant $b$ is the *$y$-intercept*: the value of the function when $x = 0$, i.e. where the line crosses the $y$-axis.

For the heating bill example: $f(g) = 1.20g + 45$. Slope $1.20$ (dollars per gallon — the rate of change). Intercept $45$ (the bill if no oil is delivered — the base service charge).

### Slope

For two points $(x_1, y_1)$ and $(x_2, y_2)$ on a line, the slope is

$$m = \frac{y_2 - y_1}{x_2 - x_1} = \frac{\Delta y}{\Delta x}$$

This is *rise over run* — the vertical change divided by the horizontal change.

A positive slope means the function is *increasing*: as $x$ grows, $y$ grows. Negative slope: *decreasing*. Zero slope: *constant* (a horizontal line).

For the heating bill, $m = 1.20$: every additional gallon adds $\$1.20$ to the bill.

### Three forms of a linear equation

Linear equations can be written in several forms; each is convenient for different purposes.

**Slope-intercept form:** $y = mx + b$. Best when you know the slope and the $y$-intercept.

**Point-slope form:** $y - y_1 = m(x - x_1)$. Best when you know the slope and one point on the line.

**Standard form:** $Ax + By = C$ where $A, B, C$ are integers and $A \geq 0$. Best for finding intercepts and for systems of equations (chapter 11).

All three forms describe the *same line*; you can convert among them.

**Example.** Find the equation of the line through $(2, 5)$ with slope $3$.

Point-slope: $y - 5 = 3(x - 2)$. Distribute and solve for $y$: $y = 3x - 6 + 5 = 3x - 1$. Slope-intercept: $y = 3x - 1$. Standard: $3x - y = 1$.

### Parallel and perpendicular lines

Two lines are *parallel* if they have the same slope: $m_1 = m_2$.

Two lines are *perpendicular* if their slopes are *negative reciprocals*: $m_1 \cdot m_2 = -1$.

So the line $y = 3x - 1$ is parallel to $y = 3x + 7$ and perpendicular to $y = -\frac{1}{3}x + 4$.

The perpendicular condition follows from geometry: rotating a line of slope $m$ by $90°$ produces a line of slope $-\frac{1}{m}$.

### Worked example

A car rental costs $\$30$ per day plus $\$0.20$ per mile. Express the daily cost $C$ as a linear function of miles $m$. Find the cost for 150 miles. Find the number of miles that produces a $\$60$ daily cost.

**Setup.** $C(m) = 0.20m + 30$. Slope: $\$0.20$/mile. Intercept: $\$30$ base.

**Cost for 150 miles.** $C(150) = 0.20(150) + 30 = 30 + 30 = \$60$.

**Miles for $\$60$.** Set $0.20m + 30 = 60$. $0.20m = 30$. $m = 150$ miles.

The same setup answered both questions — *evaluate at* $m = 150$ for one, *solve for* $m$ when $C = 60$ for the other.

### Trade-off

Linear functions are easy to work with — two parameters describe them completely; one rule fits them all. The cost is that they cannot represent any relationship that *changes its rate*. A bacterial population that doubles every 20 minutes is not linear; the speed of a falling object is not linear with time; the price of a stock is not linear over a year. Linear models are first approximations; they are useful precisely because they are simple, and they are useful only when the simplicity matches the data.

### Common misconceptions

**"Slope is the difference $y_2 - y_1$."** No. Slope is the difference $y_2 - y_1$ *divided by* $x_2 - x_1$. The denominator matters.

**"Parallel lines never meet, so they have no slope in common."** Backwards. Parallel lines *do* have a slope in common — that is what makes them parallel.

**"$y = 5$ has slope 5."** No. $y = 5$ is a horizontal line with slope 0. The "5" is the $y$-intercept (and the constant value).

---

## 3. Concept 2 — Building Linear Models from Words

Most real-world problems arrive as descriptions, not equations. The work is *translation*: turn the description into a formula, then use Chapter 2's techniques to solve.

The recipe (from source m51271):

**(1) Identify what's varying and what's fixed.** The variable is what you don't know yet. The constants are the per-unit rates and the base amounts.

**(2) Identify the rate of change.** This is the slope. It is usually a phrase like "per hour" or "per dollar" or "per item."

**(3) Identify the starting value.** This is the $y$-intercept — the value when the input is zero.

**(4) Write the function.** $f(x) = mx + b$, with $m$ the rate and $b$ the starting value.

**(5) Use the function to answer the specific question.**

### Worked examples

**Example A — Saving money.** Anya has $\$200$ saved. She saves an additional $\$50$ each week. Express her savings $S$ as a function of weeks $w$. When will she have $\$1{,}000$?

*Rate of change:* $\$50$ per week. *Starting value:* $\$200$.

$$S(w) = 50w + 200$$

To reach $\$1{,}000$: $50w + 200 = 1000$, so $w = 16$ weeks.

**Example B — Cell-phone plan.** A plan charges $\$25$ per month plus $\$0.10$ per text. If a user sends $T$ texts, what is the monthly bill $B$? At what number of texts does the bill reach $\$50$?

$B(T) = 0.10T + 25$. Setting $B = 50$: $0.10T = 25$, so $T = 250$ texts.

**Example C — Truck depreciation.** A delivery truck costs $\$45{,}000$ new and loses value at $\$3{,}500$ per year. Express the truck's value $V$ as a function of years $t$. When is the truck worth $\$10{,}000$?

*Rate:* $-3{,}500$ per year (negative — losing value). *Starting:* $\$45{,}000$.

$V(t) = -3500t + 45000$. Setting $V = 10{,}000$: $-3500t = -35{,}000$, so $t = 10$ years.

### Modeling intersecting situations

Some problems involve two linear functions and ask when one equals the other. *Set them equal and solve.*

**Example.** Plan A charges $\$30$/month plus $\$0.10$ per text. Plan B charges $\$20$/month plus $\$0.20$ per text. At what number of texts do the two plans cost the same?

$$30 + 0.10T = 20 + 0.20T$$
$$10 = 0.10T$$
$$T = 100 \text{ texts}$$

At 100 texts, both plans cost $\$40$. Below that, Plan B is cheaper. Above that, Plan A is cheaper.

### Trade-off

Linear modeling forces you to identify a single rate of change. Real situations sometimes have rates that change — a phone plan with the first 100 texts free, then $\$0.05$ each, then $\$0.10$ after 500. Such situations require *piecewise* linear functions, which are linear within each piece. The simplification is real; the technique adapts.

### Common misconceptions

**"The starting value is whatever value comes first in the problem."** No. The starting value is what the function equals when the input is *zero*. Read carefully.

**"You can't have a linear function with a negative slope."** You can. Depreciation, cooling, sales decline — all have negative slope.

---

## 4. Concept 3 — Fitting Lines to Real Data

The car rental, the heating bill, the cell-phone plan — these are *exact* linear relationships, given by contract. Most data in nature is messier. Plot a scatter of points and you usually see *approximately* linear behavior, with deviations.

A *scatter plot* shows the data points $(x_1, y_1), (x_2, y_2), \ldots$ as dots in the plane. The eye can usually tell when the dots cluster around a line — *correlation* — and when they don't.

### Line of best fit

When data is approximately linear, we look for the *best-fit line* — the line that minimizes the total deviation between predicted and actual values. The standard method, *linear regression*, computes the slope and intercept that minimize the sum of squared deviations. Most calculators and statistical software compute it directly; the formula is

$$m = \frac{n \sum x_i y_i - \sum x_i \sum y_i}{n \sum x_i^2 - (\sum x_i)^2}, \quad b = \frac{\sum y_i - m \sum x_i}{n}$$

You don't have to compute by hand; technology does it. What matters is interpreting the result.

**Example.** A study finds that for $n = 10$ cities, the relationship between average daily temperature and ice-cream sales (per capita) is approximately

$$S = 1.8T - 25$$

where $T$ is temperature in $°F$ and $S$ is sales per capita in dollars.

Slope $1.8$: every additional degree Fahrenheit corresponds to $\$1.80$ more in ice-cream sales per capita. Intercept $-25$: at $T = 0$, predicted sales are $-\$25$, which is meaningless physically. The intercept is mathematically correct but extrapolates far outside the data range; we don't trust it as a real prediction.

This is a key cautionary point. *Linear models are reliable within the range of the data. Outside that range, they are extrapolations and can produce nonsense.* The ice-cream model says nothing useful about sales at $T = 0°F$ — there were probably no cities in the data with that temperature.

### Distinguishing linear from non-linear

Not all data is linear. A quick test: compute the differences $y_2 - y_1, y_3 - y_2, y_4 - y_3, \ldots$ at equally spaced $x$ values. If the differences are *constant*, the relationship is linear. If they grow or shrink in a pattern, it's not.

**Example.** $y$ values at $x = 0, 1, 2, 3, 4$: $5, 7, 11, 17, 25$. Differences: $2, 4, 6, 8$. The differences are themselves linear (growing by 2). The original relationship is *quadratic*, not linear.

### Trade-off

Fitting a linear model to data sacrifices fidelity for tractability. A more flexible model (quadratic, exponential, etc.) might fit better but is harder to interpret and easier to overfit. The discipline is to *use the simplest model that captures the essential pattern*. Linear is often that.

### Common misconceptions

**"The line of best fit passes through every data point."** No — it passes through the *average* trend; individual points sit above and below.

**"Correlation implies causation."** No. Two variables can be correlated for many reasons (common cause, coincidence, reverse causation). The line of best fit is a description, not a causal claim.

---

## 5. Integration — One Worked Problem

Suppose you are given the following data on a hardware store's monthly nail sales (in pounds) versus the average daily temperature (°F):

| Temperature ($T$, °F) | Sales ($S$, lbs) |
|---|---|
| 30 | 110 |
| 45 | 145 |
| 60 | 175 |
| 75 | 210 |

(a) Plot the data and decide whether a linear model fits.

The data points are approximately on a line; differences in $S$ are 35, 30, 35 — close to constant. A linear model is reasonable.

(b) Find a linear model.

The slope between the first and last points is $\frac{210 - 110}{75 - 30} = \frac{100}{45} \approx 2.22$. With slope $2.22$ and the first point $(30, 110)$:

$$S = 2.22(T - 30) + 110 = 2.22T + 43.3$$

(c) Predict sales at $T = 50°F$.

$S(50) = 2.22(50) + 43.3 = 111 + 43.3 = 154.3$ pounds.

(d) Interpret the slope.

For every additional degree of average daily temperature, monthly nail sales increase by about $2.22$ pounds.

(e) Should we predict sales at $T = 100°F$?

Caution. $T = 100$ is outside the data range. The linear trend may not continue; the prediction is an extrapolation.

The example illustrates the full arc of linear modeling: collect data, judge whether linear fits, find the model, use the model within its valid range, and resist extrapolation. *That arc is the same whether the data is nail sales, climate measurements, or financial returns.*

[FIGURE: A scatter plot of the four data points with a best-fit line $S = 2.22T + 43.3$. The line extends from about $T = 25$ to $T = 80$; dashed segments show the extrapolation regions where the model is less reliable. The student should notice that the data points lie close to but not exactly on the line.]

---

## 6. Exercises

### Warm-up

**Exercise 4.1.** Find the slope of the line through $(2, 5)$ and $(7, 20)$. Difficulty: low.

**Exercise 4.2.** Write the equation of a line with slope $-2$ and $y$-intercept $5$. Difficulty: low.

### Application

**Exercise 4.3.** A taxi charges $\$3$ flag drop plus $\$2$ per mile. Express the fare $F$ as a linear function of miles $m$. Find the fare for 8 miles. Find the miles for a $\$25$ fare. Difficulty: medium.

**Exercise 4.4.** Find the equation of the line passing through $(1, 3)$ that is perpendicular to $y = 2x - 5$. Difficulty: medium.

**Exercise 4.5.** Two cell-phone plans cost the same when you send 200 texts. Plan A is $\$30$/month + $\$0.10$ per text. Find Plan B's per-text rate if its base is $\$25$/month. Difficulty: medium.

### Synthesis

**Exercise 4.6.** Data for an experiment: $(1, 4), (2, 7), (3, 10), (4, 13), (5, 16)$. (a) Is the relationship linear? (b) Find the equation. (c) Predict the value at $x = 8$. Difficulty: medium-high.

**Exercise 4.7.** A car depreciates from $\$30{,}000$ when new to $\$15{,}000$ after 5 years. Assuming linear depreciation, when is the car worth $\$5{,}000$? Difficulty: medium-high.

### Challenge

**Exercise 4.8.** A water tank is being drained. After 2 minutes, it contains 80 gallons; after 5 minutes, 50 gallons. (a) Find the linear model for water $W$ as a function of time $t$. (b) When is the tank empty? (c) What was the initial volume? Difficulty: high.

---

## 7. Chapter Summary

You can do something now you may not have been able to do an hour ago. You can recognize a linear function from its formula, table, or graph; compute its slope from any two points; write its equation in three different forms and convert among them. You can take a verbal description of a real-world situation and translate it into a linear model. You can recognize when two lines are parallel or perpendicular from their slopes. You can distinguish linear data from non-linear data and find a line of best fit when linear is appropriate.

The single idea that matters most: **a linear function is fully specified by its slope and one point.** Two pieces of information — that's it. Once you have those, every other property of the function follows: equation in any form, value at any input, point on the graph at any horizontal position. Linear functions are the simplest functions in college algebra, and that simplicity is what makes them ubiquitous.

The common mistake to watch for: extrapolating linear models beyond the data range. The model captures a trend; that trend may not continue.

---

## 8. Connections Forward

Chapter 5 generalizes: instead of $f(x) = mx + b$, allow polynomials of any degree — $f(x) = a_n x^n + \ldots + a_1 x + a_0$. Polynomial functions can have multiple zeros, multiple turning points, and behaviors much richer than the straight line. The graphical understanding from Chapter 3, the equation-solving from Chapter 2, and the modeling logic from Chapter 4 all return as analytical tools applied to polynomials.

---

### Sources (from chapter source files)

- *College Algebra* with Co-Requisite Skills, source modules m51269 through m51272 (OpenStax-derived).
