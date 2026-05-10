# Chapter 6 — Exponential and Logarithmic Functions

## 1. Chapter Opening

A radioactive sample is placed in a Geiger counter at noon. The counter reads $1{,}000$ counts per second. At 1 PM, $750$. At 2 PM, $562$. At 3 PM, $422$. The numbers do not decrease by a fixed amount each hour — they decrease by a fixed *fraction*, about 25%, each hour. This is *exponential decay*. Plot the data; the curve is not a line. The relationship is

$$N(t) = 1000 \cdot (0.75)^t$$

where $t$ is hours after noon. Exponential functions describe processes where the rate of change is *proportional to the current amount* — radioactive decay, bacterial growth, compound interest, viral spread, atmospheric pressure with altitude.

Logarithms are the inverse — given an exponential output, find the input. *How many years will it take an investment to double?* That question requires inverting an exponential, which is what a logarithm does.

This chapter develops both families together because they are inverses. By the end, you should be able to read $\log_2 8 = 3$ as fluently as $2^3 = 8$ — and recognize that they say the same thing.

### Learning objectives

By the end of this chapter, you should be able to:

- **Evaluate** and graph exponential functions $f(x) = ab^x$ and the natural exponential $f(x) = e^x$.
- **Apply** the compound-interest formula and the continuous-compounding formula $A = Pe^{rt}$.
- **Convert** between exponential and logarithmic form, evaluate logarithms with various bases, and use common ($\log_{10}$) and natural ($\ln$) logarithms.
- **Apply** the product, quotient, power, and change-of-base rules for logarithms to expand, condense, and rewrite logarithmic expressions.
- **Solve** exponential and logarithmic equations and apply them to real-world growth, decay, and modeling problems.

### Prerequisites

Chapter 1's exponent rules. Chapter 3's function notation, especially inverses. Chapter 5's rational functions (asymptotes — exponentials approach $0$ asymptotically, logarithms have vertical asymptotes at $x = 0$).

---

## 2. Concept 1 — Exponential Functions

An *exponential function* has the form

$$f(x) = a \cdot b^x$$

where $a$ is the *initial value* (the value at $x = 0$, since $b^0 = 1$), and $b$ is the *base* (positive, $b \neq 1$).

If $b > 1$, the function is *exponential growth*. If $0 < b < 1$, *exponential decay*.

For our radioactive sample: $f(t) = 1000 \cdot (0.75)^t$. Initial value $1000$. Base $0.75 < 1$, so it's decay.

### The natural base $e$

A particular base — $e \approx 2.71828$ — appears so often in mathematics, science, and finance that it has its own name. It arises naturally as the limit

$$e = \lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n$$

The natural exponential function is $f(x) = e^x$. Its graph passes through $(0, 1)$ and has the special property that *its rate of change at any point equals its value there* — a property that makes calculus dramatically cleaner with $e$ than with any other base.

### Compound interest

A bank pays interest at annual rate $r$, compounded $n$ times per year. The value of an initial deposit $P$ after $t$ years is

$$A = P\left(1 + \frac{r}{n}\right)^{nt}$$

If interest is compounded *continuously* (the limit as $n \to \infty$):

$$A = Pe^{rt}$$

**Example.** Deposit $\$1{,}000$ at 5% annual interest, compounded monthly, for 10 years.

$$A = 1000\left(1 + \frac{0.05}{12}\right)^{120} \approx 1000(1.00417)^{120} \approx \$1{,}647.01$$

If compounded continuously instead: $A = 1000 e^{0.5} \approx \$1{,}648.72$. Slight difference; same order of magnitude.

### Graphing exponential functions

The graph of $f(x) = b^x$ for $b > 1$:
- Passes through $(0, 1)$.
- Increases for all $x$.
- Horizontal asymptote $y = 0$ as $x \to -\infty$.

For $0 < b < 1$:
- Passes through $(0, 1)$.
- Decreases for all $x$.
- Horizontal asymptote $y = 0$ as $x \to +\infty$.

Transformations work as in Chapter 3: $f(x) = a \cdot b^{x - h} + k$ shifts the basic graph.

### Trade-off

Exponential functions are extraordinarily flexible — they capture growth and decay processes from cells to compound interest to civilizations. The cost is that they grow *or shrink very fast*, which makes long-term predictions sensitive to the parameters. Small changes in the base $b$ produce huge changes after many time steps.

---

## 3. Concept 2 — Logarithmic Functions

A *logarithm* answers the inverse question: $\log_b(y)$ is the exponent you need to put on $b$ to get $y$. By definition:

$$\log_b(y) = x \iff b^x = y$$

So $\log_2(8) = 3$ because $2^3 = 8$. And $\log_{10}(1000) = 3$ because $10^3 = 1000$.

### Common and natural logarithms

Two bases appear so often that they have shorthand:

- *Common logarithm:* $\log(x)$ means $\log_{10}(x)$ (base 10).
- *Natural logarithm:* $\ln(x)$ means $\log_e(x)$ (base $e$).

These are the bases of nearly all real-world applications. Chemistry's pH uses base 10. Physics uses base $e$ for almost everything.

### Properties of logarithms

The exponent rules from Chapter 1 translate into logarithm rules.

**Product rule.** $\log_b(MN) = \log_b(M) + \log_b(N)$. (Multiplication becomes addition.)

**Quotient rule.** $\log_b(M/N) = \log_b(M) - \log_b(N)$.

**Power rule.** $\log_b(M^p) = p \log_b(M)$.

**Change of base.** $\log_b(M) = \frac{\log_a(M)}{\log_a(b)}$. (Lets you compute any logarithm using any base — useful with calculators.)

**Special values.** $\log_b(1) = 0$ (because $b^0 = 1$). $\log_b(b) = 1$ (because $b^1 = b$).

### Graphing logarithms

The graph of $f(x) = \log_b(x)$ for $b > 1$:
- Domain: $x > 0$ (you can't take the log of zero or a negative).
- Passes through $(1, 0)$ (since $\log_b(1) = 0$).
- Vertical asymptote $x = 0$.
- Slowly increasing.

The logarithm grows very slowly. $\log_{10}(1000) = 3$, $\log_{10}(1{,}000{,}000) = 6$, $\log_{10}(1{,}000{,}000{,}000) = 9$. The output gains 1 each time the input multiplies by 10.

### Worked example

Solve $\log_2(x) + \log_2(x - 2) = 3$.

Combine using the product rule:
$$\log_2(x(x-2)) = 3$$

Convert to exponential form:
$$x(x-2) = 2^3 = 8$$
$$x^2 - 2x - 8 = 0$$
$$(x - 4)(x + 2) = 0$$

So $x = 4$ or $x = -2$. Check both in the original. $x = -2$ makes $\log_2(-2)$ undefined (logs of negatives don't exist), so it's extraneous. Only $x = 4$ is valid.

---

## 4. Concept 3 — Solving Equations and Modeling

Most real exponential and logarithmic problems reduce to *solving an equation*.

### Solving exponential equations

Two strategies:

**Like bases.** If you can rewrite both sides with the same base, equate the exponents.

$$2^{3x} = 16 \implies 2^{3x} = 2^4 \implies 3x = 4 \implies x = \tfrac{4}{3}$$

**Take a logarithm.** When like bases don't work, take $\log$ or $\ln$ of both sides and use the power rule.

$$5^x = 12 \implies \ln(5^x) = \ln(12) \implies x \ln(5) = \ln(12) \implies x = \tfrac{\ln(12)}{\ln(5)} \approx 1.544$$

### Solving logarithmic equations

If a single logarithm equals a constant, convert to exponential form. If multiple logs appear, combine them using the product/quotient/power rules first, then convert.

Always check candidates against the original — extraneous solutions are common when logs are involved.

### Exponential growth and decay

The general model: $A(t) = A_0 e^{kt}$, where $A_0$ is the initial amount and $k$ is the *growth rate* ($k > 0$ for growth, $k < 0$ for decay).

**Example — radioactive decay.** Carbon-14 has half-life $5{,}730$ years. A sample initially containing $A_0$ atoms will have $A(t) = A_0 e^{kt}$ atoms after $t$ years, where $k$ satisfies $\frac{1}{2}A_0 = A_0 e^{5730k}$. Solving: $k = \frac{\ln(1/2)}{5730} \approx -0.000121$.

A bone fragment is found with 30% of the original carbon-14 still present. How old is it?

$$0.3 = e^{-0.000121 t} \implies t = \frac{\ln(0.3)}{-0.000121} \approx 9{,}953 \text{ years old}$$

### Newton's law of cooling

An object at temperature $T_0$ in an environment at temperature $T_a$ cools (or warms) according to

$$T(t) = T_a + (T_0 - T_a)e^{-kt}$$

The temperature approaches the ambient $T_a$ exponentially.

### Logistic growth

For populations with carrying-capacity limits:

$$P(t) = \frac{c}{1 + ae^{-bt}}$$

The graph rises rapidly at first, then levels off at $c$ (the carrying capacity). Used for populations under resource constraints.

### Worked example — compound interest doubling time

How long does it take an investment at 6% annual interest, compounded continuously, to double?

$$2P = Pe^{0.06 t} \implies 2 = e^{0.06t} \implies \ln 2 = 0.06t \implies t = \frac{\ln 2}{0.06} \approx 11.55 \text{ years}$$

This is the *Rule of 72* approximation: doubling time $\approx 72/r$ where $r$ is the percentage rate. $72/6 = 12$, close to the exact $11.55$.

---

## 5. Integration — One Worked Problem

A petri dish initially contains $500$ bacteria. After $4$ hours, the count is $1{,}500$. (a) Build an exponential growth model. (b) When will the count reach $10{,}000$?

**(a) Build the model.** $P(t) = 500 e^{kt}$. Use the data point: $P(4) = 1500$, so $1500 = 500 e^{4k}$, giving $e^{4k} = 3$, so $k = \frac{\ln 3}{4} \approx 0.275$.

Model: $P(t) = 500 e^{0.275t}$.

**(b) Time to reach 10,000.** $10000 = 500 e^{0.275 t}$, so $e^{0.275 t} = 20$, giving $t = \frac{\ln 20}{0.275} \approx 10.9$ hours.

The example uses Concept 1 (exponential function), Concept 2 (logarithm to invert), and Concept 3 (modeling and solving). All three concepts collaborate to answer one specific question.

[FIGURE: Graph of $P(t) = 500e^{0.275t}$ from $t = 0$ to $t = 12$. Curve passes through $(0, 500)$, $(4, 1500)$, and $(10.9, 10000)$ marked. The student should notice the rapid acceleration of exponential growth.]

---

## 6. Exercises

### Warm-up

**Exercise 6.1.** Evaluate. (a) $3^4$. (b) $\log_3(81)$. (c) $\ln(e^5)$. Difficulty: low.

**Exercise 6.2.** Convert. (a) $2^5 = 32$ to log form. (b) $\log_5(125) = 3$ to exponential form. Difficulty: low.

### Application

**Exercise 6.3.** $\$2{,}000$ at 4% annual interest, compounded continuously. Value after 10 years? Difficulty: medium.

**Exercise 6.4.** Solve. (a) $4^x = 64$. (b) $7^{x+1} = 50$. (c) $\log_2(x) + \log_2(x+6) = 4$. Difficulty: medium.

**Exercise 6.5.** A population doubles every 7 years. How long to triple? Difficulty: medium.

### Synthesis

**Exercise 6.6.** Carbon-14 (half-life 5,730 years). A sample has 60% of original. Age? Difficulty: medium-high.

**Exercise 6.7.** A coffee at $200°F$ cools in a $70°F$ room. After 5 minutes, it's $150°F$. (a) Newton's law constant $k$. (b) When will it reach $90°F$? Difficulty: medium-high.

### Challenge

**Exercise 6.8.** A logistic model fits a city's population over 50 years: $P(t) = \frac{500{,}000}{1 + 9e^{-0.05t}}$. (a) Initial population. (b) Carrying capacity. (c) When does it reach 250,000? Difficulty: high.

---

## 7. Chapter Summary

You can read $\log_b(y) = x$ and $b^x = y$ as the same statement. You can solve any exponential equation by either equating exponents (when bases match) or taking logarithms (when they don't). You can apply the compound-interest formulas, both periodic and continuous. You can build exponential models from data and solve for unknown times.

The single idea that matters most: **exponential functions describe processes where the rate of change is proportional to the current amount.** Logarithms invert them. Together, they handle a vast class of natural and financial phenomena that polynomial functions cannot.

The common mistake to watch for: treating $\log(a + b)$ as $\log(a) + \log(b)$. Logarithms turn *multiplication* into addition, not *addition* into addition. $\log(ab) = \log(a) + \log(b)$, but $\log(a + b)$ has no simplification.

---

## 8. Connections Forward

Chapter 7 introduces *trigonometric functions* — another nonlinear family with periodic behavior, capturing rotation, oscillation, and waves. The tools developed for exponential and logarithmic functions (transformations, identities, equation-solving) transfer in spirit; the new family adds a periodic dimension.

---

### Sources (from chapter source files)

- *College Algebra*, source modules m49356 through m49368 (OpenStax-derived).
