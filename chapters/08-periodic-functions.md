# Chapter 8 — Periodic Functions

## 1. Chapter Opening

Stand on a beach at Boston Harbor. The water rises slowly, peaks at high tide, falls, bottoms at low tide, rises again. Two complete cycles in roughly 25 hours. Plot water level against time and you get a smooth wave that repeats — a *periodic function*.

The same wave shape appears in alternating current, in the swing of a pendulum, in the vibration of a guitar string, in the seasonal temperature cycle, in light and sound and ocean swells. *Anything that repeats* — and a great many things in nature do — can be described by a sum of sines and cosines. This chapter develops the graphs of trigonometric functions: sine, cosine, tangent, and their reciprocals, with their amplitudes, periods, and phase shifts. By the end you should be able to read a wave shape from its formula and write a formula from its wave shape.

### Learning objectives

By the end of this chapter, you should be able to:

- **Graph** $y = a\sin(bx - c) + d$ and $y = a\cos(bx - c) + d$, identifying amplitude $|a|$, period $\frac{2\pi}{|b|}$, phase shift $\frac{c}{b}$, and vertical shift $d$.
- **Graph** $y = \tan x$, $y = \sec x$, $y = \csc x$, $y = \cot x$, identifying their vertical asymptotes and periods.
- **Evaluate** the inverse trigonometric functions $\sin^{-1}, \cos^{-1}, \tan^{-1}$ and recognize their restricted domains and ranges.
- **Solve** simple trigonometric equations using inverse functions.
- **Build** sinusoidal models from real-world periodic data.

### Prerequisites

Chapter 7 (unit circle, special angles, identities). Chapter 3 (function transformations).

---

## 2. Concept 1 — Sine and Cosine Graphs

Plot $y = \sin x$ for $0 \leq x \leq 2\pi$. The curve starts at $(0, 0)$, rises smoothly to $(\pi/2, 1)$, falls back through $(\pi, 0)$ down to $(3\pi/2, -1)$, and returns to $(2\pi, 0)$. After that, the pattern repeats. The function has *period* $2\pi$.

The graph of $y = \cos x$ has the same shape, shifted left by $\pi/2$ — it starts at the maximum $(0, 1)$ instead of zero.

### The general sinusoidal function

$$y = a\sin(bx - c) + d, \quad y = a\cos(bx - c) + d$$

Each parameter has a geometric meaning:

- **Amplitude $|a|$**: the half-distance between maximum and minimum. The graph of $y = a\sin x$ oscillates between $-|a|$ and $|a|$.
- **Period $P = \frac{2\pi}{|b|}$**: the horizontal length of one complete cycle. If $b = 2$, the period is $\pi$ (the wave compresses horizontally to half its standard width). If $b = 1/2$, the period is $4\pi$ (the wave stretches).
- **Phase shift $\frac{c}{b}$**: the horizontal shift of the wave. To the right if positive, left if negative.
- **Vertical shift $d$**: the up-down translation. The midline of the wave is at $y = d$.

**Example.** Sketch $y = 3\sin\!\left(2x - \frac{\pi}{2}\right) + 1$.

Amplitude: 3 (oscillation from $-3$ to $3$, then shifted up).
Period: $\frac{2\pi}{2} = \pi$.
Phase shift: $\frac{\pi/2}{2} = \frac{\pi}{4}$ (right).
Vertical shift: 1.

So the wave oscillates between $-2$ and $4$ (midline $1$, amplitude $3$), with period $\pi$, starting its standard sine pattern at $x = \pi/4$.

### Sinusoidal modeling

A real-world periodic phenomenon often fits

$$y = a\sin(bt - c) + d$$

where:
- $a$ is half the (max − min) of the data,
- $d$ is the average of max and min,
- $b = \frac{2\pi}{P}$ where $P$ is the observed period,
- $c$ adjusts the phase to match the data's starting state.

**Example — daylight hours in Boston.** Daylight ranges from about 9 hours (Dec 21) to about 15 hours (Jun 21). Period: 365 days. Midline: 12 hours.

$$L(t) = 3\sin\!\left(\frac{2\pi}{365}(t - 81)\right) + 12$$

where $t$ is the day of year. The phase shift $81$ aligns the maximum with day 172 (June 21st), via the standard sine reaching its first peak a quarter-period after its zero crossing.

---

## 3. Concept 2 — Tangent, Cotangent, Secant, Cosecant

The other four trigonometric functions are defined as ratios:

$$\tan x = \frac{\sin x}{\cos x}, \quad \cot x = \frac{\cos x}{\sin x}, \quad \sec x = \frac{1}{\cos x}, \quad \csc x = \frac{1}{\sin x}$$

These ratios produce graphs unlike sine and cosine. Where the denominator is zero, the function is undefined and the graph has a *vertical asymptote*.

### $y = \tan x$

$\tan x = \frac{\sin x}{\cos x}$ is undefined where $\cos x = 0$, i.e. at $x = \pi/2, 3\pi/2, \ldots$ — every $\pi/2 + n\pi$ for integer $n$. Vertical asymptotes there.

Period: $\pi$ (not $2\pi$ — tangent repeats faster than sine and cosine).

The graph: increasing from $-\infty$ at $x = -\pi/2^+$ through $(0, 0)$ to $+\infty$ as $x \to \pi/2^-$. Then the next branch starts at $-\infty$ at $x = \pi/2^+$, again passing through $(\pi, 0)$ to $+\infty$ at $x = 3\pi/2^-$.

### $y = \cot x$

$\cot x = \frac{\cos x}{\sin x}$ is undefined where $\sin x = 0$, i.e. at $x = 0, \pi, 2\pi, \ldots$. Vertical asymptotes there.

Period: $\pi$.

The graph is similar to tangent but decreasing on each branch.

### $y = \sec x$ and $y = \csc x$

$\sec x = 1/\cos x$ has vertical asymptotes wherever $\cos x = 0$. Where $\cos x$ is large (near $\pm 1$), $\sec x$ is small (near $\pm 1$). Where $\cos x$ is near zero, $\sec x$ blows up.

The graph of secant looks like a series of parabolic-like cups: above the $x$-axis where cosine is positive (peaks at $y = 1$), below where cosine is negative (peaks at $y = -1$).

$\csc x = 1/\sin x$ behaves analogously, with asymptotes where $\sin x = 0$.

Period for both secant and cosecant: $2\pi$.

### Transformations of these functions

The same transformation rules apply: amplitude (which becomes the minimum-distance from the asymptote for tan/cot), period $\pi/|b|$ for tangent and cotangent, and vertical/horizontal shifts.

For $y = a\tan(bx - c) + d$:
- Period: $\frac{\pi}{|b|}$
- Vertical asymptotes: where $bx - c = \frac{\pi}{2} + n\pi$
- Vertical shift: $d$

---

## 4. Concept 3 — Inverse Trigonometric Functions

If $\sin x = 0.5$, what is $x$?

The trouble is that infinitely many values satisfy this: $x = \pi/6$, $5\pi/6$, $\pi/6 + 2\pi$, $5\pi/6 + 2\pi$, and so on. Sine is not one-to-one on its full domain, so it has no inverse on its full domain.

The fix: *restrict the domain* to a region where sine is one-to-one, then define the inverse on that restricted domain.

### Standard restricted domains

$\sin^{-1}$ (also written $\arcsin$): domain $[-1, 1]$, range $[-\pi/2, \pi/2]$. So $\sin^{-1}(1/2) = \pi/6$.

$\cos^{-1}$ ($\arccos$): domain $[-1, 1]$, range $[0, \pi]$. So $\cos^{-1}(1/2) = \pi/3$.

$\tan^{-1}$ ($\arctan$): domain all reals, range $(-\pi/2, \pi/2)$. So $\tan^{-1}(1) = \pi/4$.

The choice of restricted ranges is conventional but consistent. They were chosen to keep each inverse a function (single output per input) and to include the key reference angles.

### Composition

If $\sin^{-1}$ and $\sin$ compose, do they cancel?

In one direction, yes: $\sin(\sin^{-1}(x)) = x$ for $x \in [-1, 1]$. Always.

In the other direction, sometimes: $\sin^{-1}(\sin(x)) = x$ only when $x$ is in the restricted range $[-\pi/2, \pi/2]$. For $x$ outside that range, the composition returns the *equivalent* angle in $[-\pi/2, \pi/2]$.

Example: $\sin^{-1}(\sin(3\pi/4)) = \pi/4$. (The original $3\pi/4$ has the same sine as $\pi/4$, and $\pi/4$ is the value in the restricted range.)

### Solving simple trig equations

To solve $\sin x = 0.6$: take $\sin^{-1}$ of both sides, getting $x = \sin^{-1}(0.6) \approx 0.6435$ rad. But sine is positive in two quadrants (I and II), so the other solution in $[0, 2\pi)$ is $\pi - 0.6435 \approx 2.498$ rad. And of course any of these plus a multiple of $2\pi$ also works.

The general solution is $x = 0.6435 + 2\pi n$ or $x = 2.498 + 2\pi n$ for integer $n$.

---

## 5. Integration — Building a Tide Model

A coastal city's tide table shows: high tide at 6:00 AM (water height 14 ft), low tide at 12:00 PM (water height 2 ft), next high tide at 6:00 PM. (The cycle is 12 hours, simpler than the actual 12.4 hours, for this example.)

Build a sinusoidal model.

**Period:** 12 hours. So $b = \frac{2\pi}{12} = \frac{\pi}{6}$.

**Amplitude:** half the difference, $(14 - 2)/2 = 6$ ft.

**Vertical shift (midline):** average, $(14 + 2)/2 = 8$ ft.

**Phase:** at $t = 6$ AM, the tide is at maximum. Use cosine (which is at maximum at $t = 0$) and shift by 6 hours: $h(t) = 6\cos\!\left(\frac{\pi}{6}(t - 6)\right) + 8$.

Verify: at $t = 6$, $\cos(0) = 1$, so $h = 6 + 8 = 14$ ✓. At $t = 12$, $\cos(\pi) = -1$, so $h = -6 + 8 = 2$ ✓. At $t = 18$, $\cos(2\pi) = 1$, so $h = 14$ ✓.

**Question:** at what times is the water level at least 11 ft?

$$6\cos\!\left(\frac{\pi}{6}(t - 6)\right) + 8 \geq 11$$
$$\cos\!\left(\frac{\pi}{6}(t - 6)\right) \geq \frac{1}{2}$$

$\cos \theta \geq 1/2$ when $\theta \in [-\pi/3, \pi/3]$ (per cycle). So $\frac{\pi}{6}(t - 6) \in [-\pi/3, \pi/3]$, giving $t - 6 \in [-2, 2]$, i.e. $t \in [4, 8]$.

Water is at least 11 ft from 4 AM to 8 AM. (And by symmetry, from 4 PM to 8 PM in the next cycle.)

The example uses Concept 1 (sinusoidal modeling) and Concept 3 (solving an inequality with inverse cosine).

[FIGURE: Graph of $h(t) = 6\cos(\pi(t-6)/6) + 8$ over 24 hours showing two complete tide cycles. Horizontal line at $y = 11$. Shaded regions where $h(t) \geq 11$. The student should notice that the model captures the timing and amplitude of the tides.]

---

## 6. Exercises

### Warm-up

**Exercise 8.1.** Identify amplitude, period, phase shift, vertical shift. (a) $y = 4\sin(2x)$. (b) $y = 2\cos(x - \pi/4) + 3$. Difficulty: low.

**Exercise 8.2.** Evaluate. (a) $\sin^{-1}(1/2)$. (b) $\cos^{-1}(0)$. (c) $\tan^{-1}(\sqrt{3})$. Difficulty: low.

### Application

**Exercise 8.3.** Sketch $y = 3\sin(2x - \pi) - 1$. Label amplitude, period, phase shift, vertical shift, and one full cycle. Difficulty: medium.

**Exercise 8.4.** Find all solutions of $\cos x = -1/2$ on $[0, 2\pi)$. Difficulty: medium.

**Exercise 8.5.** A Ferris wheel of radius 30 ft completes one revolution in 60 seconds. The lowest point of a car is 5 ft above the ground. Build a model for the height of a car as a function of time, starting from the lowest point. Difficulty: medium.

### Synthesis

**Exercise 8.6.** Identify the period and vertical asymptotes of $y = \tan(2x)$. Difficulty: medium-high.

**Exercise 8.7.** Daylight hours in Reykjavík range from about 4 hours (Dec 21) to about 21 hours (Jun 21). Build a sinusoidal model. When would the model predict 12 hours of daylight? Difficulty: medium-high.

### Challenge

**Exercise 8.8.** A weight on a spring oscillates with displacement $y(t) = 4\cos(2\pi t) + 0.5\cos(4\pi t)$ inches. (a) What is the period of the combined motion? (b) Approximate maximum and minimum values. Difficulty: high.

---

## 7. Chapter Summary

You can now graph sinusoidal functions with arbitrary amplitude, period, phase, and vertical shift. You can graph the secant, cosecant, tangent, and cotangent functions, identifying their vertical asymptotes. You can evaluate inverse trig functions on their restricted domains. You can build a sinusoidal model from real-world periodic data and use it to solve equations and inequalities.

The single idea that matters most: **a sinusoidal function is fully specified by four parameters — amplitude, period, phase, vertical shift.** Once you have these, the graph follows. Real-world periodic phenomena are usually well-described by such functions over reasonable time scales.

---

## 8. Connections Forward

Chapter 9 develops the *trigonometric identities* that let you simplify and solve more complex trig expressions and equations. Chapter 10 applies trigonometry to non-right triangles and to vectors. The graphical tools from this chapter remain in use throughout.

---

### Sources (from chapter source files)

- *College Algebra*, source modules m49386 through m49390 (OpenStax-derived).
