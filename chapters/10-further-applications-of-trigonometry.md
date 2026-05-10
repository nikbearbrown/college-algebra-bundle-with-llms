# Chapter 10 — Further Applications of Trigonometry

## 1. Chapter Opening

A surveyor in 19th-century India is mapping the Himalayan foothills. From a station 1.2 miles from a mountain's base, the angle of elevation to the peak is $42°$. From a second station 2 miles further along the same direction, the angle is $28°$. These two angles and one distance, with the law of sines and the law of cosines, are enough to compute the height of the peak. The mountain itself was Mount Everest; the survey was the *Great Trigonometric Survey of India*; the result was the first measurement of the world's highest mountain — $29{,}002$ ft, off by only a few hundred feet from the modern value [historically anchored, source m49405].

Trigonometry's reach extends far beyond right triangles. This chapter takes the trig of Chapters 7–9 and applies it to: oblique (non-right) triangles, polar coordinates, complex numbers in polar form, parametric equations, and vectors. Each topic is its own application; together they cover the breadth of trigonometry's modern role.

### Learning objectives

By the end of this chapter, you should be able to:

- **Apply** the law of sines and law of cosines to solve oblique triangles.
- **Plot** and convert between polar and rectangular coordinates; **graph** simple polar equations.
- **Express** complex numbers in polar form and **multiply** or take powers using De Moivre's theorem.
- **Parameterize** a curve and convert between parametric and rectangular forms.
- **Add** vectors, **find** their components, magnitude, and direction; **resolve** vectors into perpendicular components.

### Prerequisites

Chapters 7–9 (trig functions, identities). Chapter 2 (coordinate geometry, distance formula).

---

## 2. Concept 1 — Oblique Triangles: Laws of Sines and Cosines

A right triangle has a $90°$ angle and is solvable with sine, cosine, tangent. An *oblique* triangle has no right angle. Two laws extend trig to oblique triangles.

### Law of sines

In any triangle, the ratio of a side's length to the sine of the opposite angle is constant:

$$\frac{a}{\sin A} = \frac{b}{\sin B} = \frac{c}{\sin C}$$

Useful when you know:
- Two angles and one side (AAS or ASA).
- Two sides and a non-included angle (SSA — the *ambiguous case*: 0, 1, or 2 triangles may satisfy).

**Example.** In triangle $ABC$, $A = 50°$, $B = 60°$, $a = 10$. Find $b$.

By the law of sines: $\frac{b}{\sin 60°} = \frac{10}{\sin 50°}$, giving $b = \frac{10\sin 60°}{\sin 50°} \approx 11.30$.

### Law of cosines

A generalization of the Pythagorean theorem. For a triangle with sides $a$, $b$, $c$ and angles $A$, $B$, $C$ opposite them:

$$c^2 = a^2 + b^2 - 2ab\cos C$$

(And similar for $a^2$ and $b^2$.) When $C = 90°$, $\cos C = 0$ and we recover the Pythagorean theorem.

Useful when you know:
- All three sides (SSS) — find an angle.
- Two sides and the included angle (SAS) — find the third side.

**Example — Mount Everest setup.** Two stations measure the peak's angle of elevation. Station 1 at distance $d_1$ from the base, angle $\alpha$. Station 2 at distance $d_1 + d_2$ from the base, angle $\beta$. Using the difference of two right triangles, the peak height $h$ satisfies $h = d_1 \tan\alpha$ and $h = (d_1 + d_2)\tan\beta$. (For non-collinear stations, the laws of sines and cosines extend the calculation.)

### Heron's formula

For a triangle with sides $a, b, c$, the area is

$$\text{Area} = \sqrt{s(s-a)(s-b)(s-c)}$$

where $s = (a + b + c)/2$ is the *semiperimeter*. Useful when you know all three sides but no angles.

---

## 3. Concept 2 — Polar Coordinates and Complex Numbers

A point in the plane can be specified two ways: rectangular coordinates $(x, y)$ or polar coordinates $(r, \theta)$, where $r$ is the distance from the origin and $\theta$ is the angle from the positive $x$-axis.

### Conversion

$$x = r\cos\theta, \quad y = r\sin\theta$$
$$r = \sqrt{x^2 + y^2}, \quad \tan\theta = y/x$$

(Care needed when finding $\theta$: the quadrant of $(x, y)$ determines the correct $\theta$.)

### Polar equations

Polar form makes some curves much simpler than rectangular form. Examples:

- $r = a$: a circle of radius $a$ centered at origin.
- $r = a\cos\theta$ or $r = a\sin\theta$: a circle (passes through origin).
- $r = a + b\cos\theta$: a *limaçon*; cardioid if $a = b$.
- $r = a\cos(n\theta)$: a *rose* with $n$ petals (if $n$ odd) or $2n$ (if $n$ even).
- $r = a\theta$: an Archimedean spiral.

These shapes are clean to draw in polar but messy in rectangular.

### Complex numbers in polar form

A complex number $z = x + yi$ corresponds to the point $(x, y)$. In polar form:

$$z = r(\cos\theta + i\sin\theta)$$

where $r = |z| = \sqrt{x^2 + y^2}$ is the *modulus* (or absolute value) and $\theta$ is the *argument*.

The notation $r\,\text{cis}\,\theta = r(\cos\theta + i\sin\theta)$ is sometimes used.

### Multiplication and powers (De Moivre's theorem)

Multiplication of complex numbers in polar form is simple:
$$(r_1 \text{cis}\,\theta_1)(r_2 \text{cis}\,\theta_2) = r_1 r_2 \,\text{cis}(\theta_1 + \theta_2)$$

Multiply moduli; add arguments.

For powers: $(r\,\text{cis}\,\theta)^n = r^n \,\text{cis}(n\theta)$. This is *De Moivre's theorem*.

**Example.** $(1 + i)^4$. Convert: $1 + i = \sqrt{2}\,\text{cis}(\pi/4)$. Then $(1+i)^4 = (\sqrt{2})^4 \,\text{cis}(4 \cdot \pi/4) = 4\,\text{cis}(\pi) = -4$.

(Verify by direct expansion: $(1+i)^2 = 2i$, $(2i)^2 = -4$. ✓)

---

## 4. Concept 3 — Parametric Equations and Vectors

### Parametric equations

A curve in the plane can be described by giving $x$ and $y$ as functions of a parameter $t$:

$$x = f(t), \quad y = g(t)$$

The parameter often represents time. As $t$ varies, the point $(x(t), y(t))$ traces the curve.

**Example — projectile motion.** A ball thrown at speed $v_0$ at angle $\alpha$ above horizontal has trajectory

$$x(t) = v_0 t \cos\alpha, \quad y(t) = v_0 t \sin\alpha - \tfrac{1}{2}gt^2$$

where $g$ is gravity. The parameter $t$ is time. Eliminating $t$: $t = x/(v_0\cos\alpha)$, substitute into $y$:

$$y = x\tan\alpha - \frac{g x^2}{2v_0^2\cos^2\alpha}$$

a parabola in $x$ — but the parametric form preserves the time information.

### Eliminating the parameter

Given parametric equations, sometimes you can solve for $t$ in one and substitute into the other to get a relation between $x$ and $y$ alone. Other parameterizations (like trig parameterizations of circles: $x = r\cos t$, $y = r\sin t$) eliminate via $\sin^2 + \cos^2 = 1$.

### Vectors

A *vector* in the plane has both magnitude and direction. Geometrically, an arrow from one point to another. Algebraically, a pair $\langle a, b \rangle$ — the components.

**Magnitude:** $|\vec{v}| = \sqrt{a^2 + b^2}$.

**Direction:** angle from positive $x$-axis: $\theta = \tan^{-1}(b/a)$ (with quadrant tracking).

**Addition:** $\langle a_1, b_1 \rangle + \langle a_2, b_2 \rangle = \langle a_1 + a_2, b_1 + b_2 \rangle$. Geometrically: tip-to-tail.

**Scalar multiplication:** $k\langle a, b\rangle = \langle ka, kb\rangle$. Stretches the vector by factor $k$.

**Component form from magnitude and direction:** if $\vec{v}$ has magnitude $r$ and direction $\theta$, then $\vec{v} = \langle r\cos\theta, r\sin\theta \rangle$.

**Example.** A plane flies at 500 mph heading $30°$ east of north (i.e., $60°$ from positive $x$-axis). The wind blows at 50 mph from the west (positive $x$-direction).

Plane vector (heading): $\vec{p} = 500\langle\cos 60°, \sin 60°\rangle = \langle 250, 433\rangle$.
Wind vector: $\vec{w} = \langle 50, 0\rangle$.
Resultant ground velocity: $\vec{r} = \vec{p} + \vec{w} = \langle 300, 433\rangle$.
Magnitude: $|\vec{r}| = \sqrt{300^2 + 433^2} \approx 526$ mph.
Direction: $\theta = \tan^{-1}(433/300) \approx 55.3°$ — slightly east of original heading.

The wind shifts both the speed and direction of the plane.

---

## 5. Integration — One Worked Problem

Two ranger stations are 12 miles apart along an east-west line. From station A, a fire is sighted at bearing $N 35° E$ (i.e., $35°$ east of due north). From station B (east of A), the same fire is sighted at bearing $N 60° W$. How far is the fire from each station?

**Setup.** Let $A$ be the origin, $B$ at $(12, 0)$. The fire is north of both stations (positive $y$).

From $A$: bearing $N 35° E$ means the angle from due north is $35°$ to the east. So the angle the sight-line makes with the positive $x$-axis is $90° - 35° = 55°$.

From $B$: bearing $N 60° W$ means $60°$ west of due north, so $90° + 60° = 150°$ from positive $x$-axis.

**Angles in the triangle $ABF$ (where $F$ is the fire):**

At $A$: angle between $AB$ (east, positive $x$) and $AF$ (at $55°$) is $55°$.
At $B$: angle between $BA$ (west, negative $x$, i.e. $180°$) and $BF$ (at $150°$) is $180° - 150° = 30°$.
Therefore at $F$: $180° - 55° - 30° = 95°$.

**Law of sines.** $\frac{12}{\sin 95°} = \frac{AF}{\sin 30°} = \frac{BF}{\sin 55°}$.

$$AF = \frac{12\sin 30°}{\sin 95°} \approx \frac{6}{0.996} \approx 6.02 \text{ mi}$$
$$BF = \frac{12\sin 55°}{\sin 95°} \approx \frac{9.83}{0.996} \approx 9.87 \text{ mi}$$

The fire is about 6 miles from station A and about 9.9 miles from station B.

The example uses Concept 1 (law of sines) for an applied bearing problem.

[FIGURE: Two ranger stations 12 miles apart with a fire to the north. Bearings from each station drawn. Triangle with angles 55°, 30°, 95° labeled. Fire's distance from each station marked.]

---

## 6. Exercises

### Warm-up

**Exercise 10.1.** In triangle $ABC$, $A = 30°$, $B = 80°$, $a = 5$. Find $b$. Difficulty: low.

**Exercise 10.2.** Convert $(4, 4\sqrt{3})$ to polar. Difficulty: low.

### Application

**Exercise 10.3.** Find side $c$ in triangle with $a = 7$, $b = 9$, $C = 60°$. Difficulty: medium.

**Exercise 10.4.** Convert $z = -3 + 3i$ to polar form. Find $z^4$ using De Moivre's theorem. Difficulty: medium.

**Exercise 10.5.** Eliminate the parameter from $x = 2 + t$, $y = 3 + 2t$ to find a Cartesian equation. Difficulty: medium.

**Exercise 10.6.** Find the resultant vector for $\vec{u} = \langle 4, -2\rangle$ and $\vec{v} = \langle -1, 5\rangle$. State magnitude and direction. Difficulty: medium.

### Synthesis

**Exercise 10.7.** A plane flies at 400 mph heading due north. A 60-mph wind blows from $30°$ east of north. Find the plane's resultant ground speed and direction. Difficulty: medium-high.

**Exercise 10.8.** Two ships leave port at the same time. Ship A travels at 20 mph at bearing $N 30° E$. Ship B at 25 mph at bearing $S 45° E$. How far apart are they after 2 hours? Difficulty: medium-high.

### Challenge

**Exercise 10.9.** Find the cube roots of $8(\cos 60° + i\sin 60°)$. Difficulty: high.

---

## 7. Chapter Summary

You can solve oblique triangles using the law of sines and law of cosines. You can plot polar coordinates and convert between polar and rectangular forms. You can write complex numbers in polar form and use De Moivre's theorem for products and powers. You can parameterize curves with respect to time. You can perform vector arithmetic — adding, scaling, finding magnitude and direction.

The single idea that matters most: **trigonometry extends beyond right triangles to any geometric or vector-arithmetic situation that involves angles and magnitudes.**

---

## 8. Connections Forward

Chapter 11 takes up systems of equations and inequalities — methods for solving multiple equations simultaneously. Chapter 12 returns to coordinate geometry with the conic sections (ellipse, parabola, hyperbola), which can also be parameterized using the trigonometry of this chapter.

---

### Sources (from chapter source files)

- *College Algebra*, source modules m49402 through m49412 (OpenStax-derived).
