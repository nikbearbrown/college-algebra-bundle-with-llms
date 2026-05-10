# Chapter 9 — Trigonometric Identities and Equations

## 1. Chapter Opening

A radio engineer wants to combine two signals — one a pure $440$-Hz tone, the other a $660$-Hz tone — into a single waveform that the receiver can decode. The mathematics is one line of trigonometry: $\sin(2\pi \cdot 440\, t) + \sin(2\pi \cdot 660\, t)$. Whether the engineer can simplify or solve equations involving such expressions depends on a small but powerful set of *trigonometric identities* — equations that hold for every angle.

This chapter develops those identities and uses them to solve equations involving trig functions. The identities are not memorization for its own sake; they are the moves that let trig calculations be done at all.

### Learning objectives

By the end of this chapter, you should be able to:

- **Apply** the fundamental Pythagorean, reciprocal, and quotient identities to simplify trig expressions.
- **Use** sum and difference formulas for sine, cosine, and tangent.
- **Apply** double-angle, reduction (power-reducing), and half-angle formulas.
- **Convert** product expressions to sums and sum expressions to products.
- **Solve** trigonometric equations algebraically using identities and inverse functions.

### Prerequisites

Chapters 7 and 8 (unit circle, trig functions and graphs).

---

## 2. Concept 1 — Fundamental and Sum/Difference Identities

### Fundamental identities

Already met in Chapter 7. The Pythagorean identity:
$$\sin^2\theta + \cos^2\theta = 1$$

Two consequences (divide by $\cos^2\theta$ or $\sin^2\theta$):
$$1 + \tan^2\theta = \sec^2\theta, \quad 1 + \cot^2\theta = \csc^2\theta$$

Reciprocal identities:
$$\sec\theta = \frac{1}{\cos\theta}, \quad \csc\theta = \frac{1}{\sin\theta}, \quad \cot\theta = \frac{1}{\tan\theta}$$

Quotient identities:
$$\tan\theta = \frac{\sin\theta}{\cos\theta}, \quad \cot\theta = \frac{\cos\theta}{\sin\theta}$$

Even/odd:
$$\sin(-\theta) = -\sin\theta, \quad \cos(-\theta) = \cos\theta, \quad \tan(-\theta) = -\tan\theta$$

### Sum and difference formulas

These take the trig of a sum (or difference) of two angles and break it into trig of the individual angles.

$$\cos(A \pm B) = \cos A \cos B \mp \sin A \sin B$$

$$\sin(A \pm B) = \sin A \cos B \pm \cos A \sin B$$

$$\tan(A \pm B) = \frac{\tan A \pm \tan B}{1 \mp \tan A \tan B}$$

(Watch the signs carefully — the $\mp$ in cosine flips relative to the $\pm$ in the input; same for the denominator of tangent.)

**Example.** Compute $\cos(75°) = \cos(45° + 30°)$.
$$\cos 45° \cos 30° - \sin 45° \sin 30° = \frac{\sqrt{2}}{2} \cdot \frac{\sqrt{3}}{2} - \frac{\sqrt{2}}{2} \cdot \frac{1}{2} = \frac{\sqrt{6} - \sqrt{2}}{4}$$

The exact value of $\cos 75°$ — derived from two angles whose values are known.

### Verifying identities

A common exercise: prove that two trig expressions are equal for all valid $\theta$. The standard technique:

1. Start with the more complicated side.
2. Rewrite using fundamental identities until you reach the simpler side.

**Example.** Verify $\frac{1 - \cos 2\theta}{\sin 2\theta} = \tan\theta$.

(Using the double-angle formulas from Concept 2: $\cos 2\theta = 1 - 2\sin^2\theta$ and $\sin 2\theta = 2\sin\theta\cos\theta$.)

$$\frac{1 - (1 - 2\sin^2\theta)}{2\sin\theta\cos\theta} = \frac{2\sin^2\theta}{2\sin\theta\cos\theta} = \frac{\sin\theta}{\cos\theta} = \tan\theta \quad \checkmark$$

---

## 3. Concept 2 — Double, Half, and Power-Reducing Formulas

### Double-angle formulas

Set $A = B = \theta$ in the sum formulas:

$$\sin 2\theta = 2\sin\theta\cos\theta$$
$$\cos 2\theta = \cos^2\theta - \sin^2\theta = 2\cos^2\theta - 1 = 1 - 2\sin^2\theta$$
$$\tan 2\theta = \frac{2\tan\theta}{1 - \tan^2\theta}$$

Three forms of $\cos 2\theta$ — all equivalent, useful in different contexts.

### Half-angle formulas

Solve $\cos 2\theta = 1 - 2\sin^2\theta$ for $\sin\theta$:
$$\sin\frac{\theta}{2} = \pm\sqrt{\frac{1 - \cos\theta}{2}}, \quad \cos\frac{\theta}{2} = \pm\sqrt{\frac{1 + \cos\theta}{2}}$$

Choose the sign based on which quadrant $\theta/2$ is in.

$$\tan\frac{\theta}{2} = \frac{1 - \cos\theta}{\sin\theta} = \frac{\sin\theta}{1 + \cos\theta}$$

**Example.** Find $\sin 22.5° = \sin(45°/2)$.

$$\sin 22.5° = \sqrt{\frac{1 - \cos 45°}{2}} = \sqrt{\frac{1 - \sqrt{2}/2}{2}} = \frac{\sqrt{2 - \sqrt{2}}}{2}$$

### Power-reducing (reduction) formulas

These rewrite $\sin^2$ and $\cos^2$ in terms of $\cos 2\theta$:
$$\sin^2\theta = \frac{1 - \cos 2\theta}{2}, \quad \cos^2\theta = \frac{1 + \cos 2\theta}{2}$$

These are useful in calculus for integration of $\sin^2$ and $\cos^2$.

### Product-to-sum and sum-to-product

These convert between products and sums:

$$\sin A \cos B = \tfrac{1}{2}[\sin(A+B) + \sin(A-B)]$$
$$\cos A \cos B = \tfrac{1}{2}[\cos(A-B) + \cos(A+B)]$$
$$\sin A \sin B = \tfrac{1}{2}[\cos(A-B) - \cos(A+B)]$$

And the reverse direction (sum-to-product):

$$\sin A + \sin B = 2\sin\frac{A+B}{2}\cos\frac{A-B}{2}$$
$$\cos A + \cos B = 2\cos\frac{A+B}{2}\cos\frac{A-B}{2}$$

These appear in signal processing (mixing frequencies) and acoustics (beats).

---

## 4. Concept 3 — Solving Trigonometric Equations

A trig equation is solved when you find all $\theta$ that satisfy it.

### Equations involving a single trig function

To solve $\sin\theta = c$ for some constant $c \in [-1, 1]$:

1. Find one solution: $\theta = \sin^{-1}(c)$.
2. Find the second solution in $[0, 2\pi)$: $\theta = \pi - \sin^{-1}(c)$ (using sine's symmetry).
3. The general solution is each plus $2\pi n$ for integer $n$.

For cosine, the symmetry is different: solutions are $\theta = \pm\cos^{-1}(c) + 2\pi n$.

For tangent, period is $\pi$, so solutions are $\theta = \tan^{-1}(c) + \pi n$.

**Example.** Solve $2\sin\theta - 1 = 0$ on $[0, 2\pi)$.

$$\sin\theta = \frac{1}{2} \implies \theta = \frac{\pi}{6} \text{ or } \theta = \pi - \frac{\pi}{6} = \frac{5\pi}{6}$$

### Equations in quadratic form

If the equation is quadratic in a trig function, treat the trig function as a single variable, factor or apply the quadratic formula, then back out.

**Example.** Solve $2\sin^2\theta - 3\sin\theta + 1 = 0$ on $[0, 2\pi)$.

Let $u = \sin\theta$. Equation becomes $2u^2 - 3u + 1 = 0$, factoring to $(2u - 1)(u - 1) = 0$. So $u = 1/2$ or $u = 1$.

$\sin\theta = 1/2$: $\theta = \pi/6$ or $5\pi/6$.
$\sin\theta = 1$: $\theta = \pi/2$.

Three solutions on $[0, 2\pi)$: $\pi/6, \pi/2, 5\pi/6$.

### Equations using identities

Sometimes the equation is solvable only after using an identity to simplify.

**Example.** Solve $\sin 2\theta = \cos\theta$ on $[0, 2\pi)$.

Use the double-angle formula:
$$2\sin\theta\cos\theta = \cos\theta$$
$$\cos\theta(2\sin\theta - 1) = 0$$

So $\cos\theta = 0$ (giving $\theta = \pi/2$ or $3\pi/2$) or $\sin\theta = 1/2$ (giving $\theta = \pi/6$ or $5\pi/6$).

Four solutions: $\pi/6, \pi/2, 5\pi/6, 3\pi/2$.

---

## 5. Integration — One Worked Problem

A pendulum's angular displacement (in radians) from vertical is modeled by $\theta(t) = 0.2\cos(2t) + 0.05\sin(2t)$. (a) Express this as a single sinusoid $R\cos(2t - \phi)$. (b) Find the maximum amplitude. (c) When is the pendulum first at zero displacement after $t = 0$?

**(a) Convert to single sinusoid.** The form $R\cos(2t - \phi)$ expands as $R\cos\phi \cos 2t + R\sin\phi \sin 2t$. Matching:

$$R\cos\phi = 0.2, \quad R\sin\phi = 0.05$$

Then $R^2 = 0.2^2 + 0.05^2 = 0.0425$, giving $R \approx 0.206$ rad. And $\tan\phi = 0.05/0.2 = 0.25$, giving $\phi \approx 0.245$ rad.

So $\theta(t) \approx 0.206\cos(2t - 0.245)$.

**(b) Maximum amplitude.** $R \approx 0.206$ rad, or about $11.8°$.

**(c) First zero.** $\cos(2t - 0.245) = 0$ when $2t - 0.245 = \pi/2$, i.e. $t = (\pi/2 + 0.245)/2 \approx 0.908$ s.

The example uses Concept 1 (sum/difference formula run in reverse, for the linear combination), Concept 2 (the implicit double-angle identity for $\cos$), and Concept 3 (solving for the zero).

[FIGURE: Graph of $\theta(t) = 0.2\cos(2t) + 0.05\sin(2t)$ over the first 3 seconds, with the equivalent $0.206\cos(2t - 0.245)$ overlaid. The student should notice that the two are identical functions. Marked: maximum at $t = 0.245/2 \approx 0.123$, first zero at $t \approx 0.908$.]

---

## 6. Exercises

### Warm-up

**Exercise 9.1.** Verify the Pythagorean identity for $\theta = 5\pi/6$. Difficulty: low.

**Exercise 9.2.** Use the sum formula to find $\sin 75°$. Difficulty: low.

### Application

**Exercise 9.3.** Solve $2\cos\theta + \sqrt{3} = 0$ on $[0, 2\pi)$. Difficulty: medium.

**Exercise 9.4.** Verify: $\frac{\sin 2\theta}{1 + \cos 2\theta} = \tan\theta$. Difficulty: medium.

**Exercise 9.5.** Solve $\cos 2\theta + \cos\theta = 0$ on $[0, 2\pi)$. Difficulty: medium.

### Synthesis

**Exercise 9.6.** Find $\cos\theta$ exactly if $\sin\theta = 1/3$ and $\theta$ is in Q II. Difficulty: medium-high.

**Exercise 9.7.** Solve $2\sin^2\theta = 1 + \cos\theta$ on $[0, 2\pi)$. Difficulty: medium-high.

### Challenge

**Exercise 9.8.** Express $\sin 4\theta$ as a polynomial in $\sin\theta$ and $\cos\theta$. Difficulty: high.

---

## 7. Chapter Summary

You can now apply the fundamental Pythagorean identity, the sum/difference formulas, the double-angle and half-angle formulas, and the product-to-sum and sum-to-product formulas. You can verify identities and solve trigonometric equations using algebraic factoring and quadratic-form techniques.

The single idea that matters most: **trig identities reduce complex trig expressions to simpler ones using a small, structured catalog.** With the catalog in hand, most trig equations become solvable.

---

## 8. Connections Forward

Chapter 10 takes trigonometry to non-right triangles (law of sines, law of cosines) and to vectors. Chapter 12's analytic geometry uses trig parameterizations of conic sections. The identity machinery from this chapter is the foundation for both.

---

### Sources (from chapter source files)

- *College Algebra*, source modules m51287 through m51292 (OpenStax-derived).
