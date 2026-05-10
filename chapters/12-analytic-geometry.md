# Chapter 12 — Analytic Geometry

## 1. Chapter Opening

A satellite orbits Earth in an ellipse — closer to the planet at one point, farther at another. The shape of the orbit is determined by physics, but its mathematical description is one equation in $x$ and $y$. The same equation also describes the ceiling of a whispering gallery (where a sound at one focus reaches the other across the room) and the cross-section of a cooking solar oven. *The same curve, the ellipse, recurs across optics, acoustics, and astronomy.*

A *conic section* is any curve obtained by intersecting a cone with a plane. Tilt the plane one way and you get an ellipse. Tilt it parallel to a side of the cone and you get a parabola. Tilt it more steeply and you get a hyperbola. These three curves — ellipse, parabola, hyperbola — together with the circle (a special ellipse) — are the four conic sections, and they have been studied since the Greeks.

This chapter develops their algebraic descriptions: how to write each conic's equation, how to graph it, how to recognize it from the equation alone.

### Learning objectives

By the end of this chapter, you should be able to:

- **Identify** an ellipse from its standard-form equation, locate its center, vertices, and foci, and graph it.
- **Identify** a hyperbola from its standard-form equation, locate its center, vertices, foci, and asymptotes, and graph it.
- **Identify** a parabola from its standard-form equation, locate its vertex, focus, and directrix, and graph it.
- **Recognize** the type of conic from a general second-degree equation $Ax^2 + Bxy + Cy^2 + \ldots = 0$ using the discriminant.
- **Convert** between rectangular and polar forms of conic equations.

### Prerequisites

Chapters 1–3 (algebra, completing the square, function basics). Chapter 5 (quadratic functions). Chapter 7 (trigonometry, polar coordinates).

---

## 2. Concept 1 — The Ellipse

An *ellipse* is the set of points whose total distance from two fixed points (the *foci*) is constant.

The standard form, centered at the origin, with horizontal major axis:

$$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1, \quad a > b > 0$$

- *Vertices:* $(\pm a, 0)$ — the endpoints of the major axis.
- *Co-vertices:* $(0, \pm b)$ — endpoints of the minor axis.
- *Foci:* $(\pm c, 0)$, where $c = \sqrt{a^2 - b^2}$.
- *Major axis length:* $2a$. *Minor axis length:* $2b$.

For a vertical major axis: swap roles, $\frac{x^2}{b^2} + \frac{y^2}{a^2} = 1$.

For an ellipse centered at $(h, k)$:

$$\frac{(x-h)^2}{a^2} + \frac{(y-k)^2}{b^2} = 1$$

### Eccentricity

The *eccentricity* $e = c/a$ measures how "stretched" the ellipse is. For a circle, $a = b$ so $c = 0$ and $e = 0$. For increasingly elongated ellipses, $e$ approaches 1. (Earth's orbit: $e \approx 0.017$, very nearly circular. Halley's comet: $e \approx 0.967$, highly elongated.)

### Worked example

Find the equation of the ellipse with vertices at $(\pm 5, 0)$ and foci at $(\pm 3, 0)$.

$a = 5$, $c = 3$, so $b^2 = a^2 - c^2 = 25 - 9 = 16$, $b = 4$.

$$\frac{x^2}{25} + \frac{y^2}{16} = 1$$

### Application — whispering galleries

In a room with an elliptical ceiling, a sound made at one focus is reflected off the ceiling and converges at the other focus. Statuary Hall in the U.S. Capitol is a famous example. The geometric property — distances from foci sum to a constant — produces the acoustic effect.

---

## 3. Concept 2 — The Hyperbola

A *hyperbola* is the set of points whose absolute *difference* of distances from two foci is constant. Where the ellipse uses the sum, the hyperbola uses the difference.

Standard form, centered at origin, transverse axis horizontal:

$$\frac{x^2}{a^2} - \frac{y^2}{b^2} = 1$$

The hyperbola has two separate branches. Its features:

- *Vertices:* $(\pm a, 0)$.
- *Foci:* $(\pm c, 0)$, where $c = \sqrt{a^2 + b^2}$ (note: addition, not subtraction).
- *Asymptotes:* $y = \pm \frac{b}{a} x$ (the diagonals of the central rectangle).
- *Center:* $(0, 0)$.

For a vertical transverse axis: $\frac{y^2}{a^2} - \frac{x^2}{b^2} = 1$.

For a hyperbola centered at $(h, k)$:

$$\frac{(x-h)^2}{a^2} - \frac{(y-k)^2}{b^2} = 1$$

### Worked example

Identify and graph $\frac{x^2}{16} - \frac{y^2}{9} = 1$.

$a^2 = 16$, $b^2 = 9$, so $a = 4$, $b = 3$. $c^2 = 16 + 9 = 25$, $c = 5$.

Vertices: $(\pm 4, 0)$. Foci: $(\pm 5, 0)$. Asymptotes: $y = \pm \frac{3}{4} x$. Two branches opening left and right.

---

## 4. Concept 3 — The Parabola, General Conics, and Polar Form

### Parabola

A *parabola* is the set of points equidistant from a fixed point (the *focus*) and a fixed line (the *directrix*).

Standard forms:

- Vertex at origin, opening right: $y^2 = 4px$ where $p > 0$. Focus at $(p, 0)$, directrix $x = -p$.
- Opening up: $x^2 = 4py$. Focus at $(0, p)$, directrix $y = -p$.

Parabolas with vertex at $(h, k)$:
- Opening right: $(y - k)^2 = 4p(x - h)$.
- Opening up: $(x - h)^2 = 4p(y - k)$.

### Application — parabolic reflectors

A parabolic mirror reflects parallel rays (light from a distant source) to its focus. Used in telescopes (collecting starlight), satellite dishes (collecting radio signals), and headlights (where the light source at the focus produces parallel rays going outward).

### General second-degree equation

Any conic in the plane can be described by

$$Ax^2 + Bxy + Cy^2 + Dx + Ey + F = 0$$

The *discriminant* $B^2 - 4AC$ classifies the conic:

- $B^2 - 4AC < 0$: ellipse (or circle if $A = C, B = 0$).
- $B^2 - 4AC = 0$: parabola.
- $B^2 - 4AC > 0$: hyperbola.

The presence of a $Bxy$ term means the conic is rotated; eliminating it via rotation of axes gives a standard form.

### Conics in polar form

With one focus at the origin, the conic equation in polar coordinates is

$$r = \frac{ed}{1 - e\cos\theta} \quad \text{or} \quad r = \frac{ed}{1 + e\cos\theta}$$

(or with $\sin$ for vertical-axis conics), where $e$ is the eccentricity and $d$ is the distance from focus to directrix.

- $e < 1$: ellipse.
- $e = 1$: parabola.
- $e > 1$: hyperbola.

Polar form is natural for orbital mechanics — Kepler's first law states that planets move in ellipses with the Sun at one focus, which is exactly the polar-form picture.

---

## 5. Integration — One Worked Problem

A satellite is in elliptical orbit around Earth. At its closest (perigee) it is 200 km above Earth's surface; at its farthest (apogee) it is 2,000 km above the surface. Find the equation of the orbit, with Earth's center at one focus.

Earth's radius: about 6,371 km.

Distance from Earth's center at perigee: $6371 + 200 = 6571$ km.
Distance at apogee: $6371 + 2000 = 8371$ km.

For an ellipse with one focus at the origin:
- Perigee distance = $a - c$ (closest point on ellipse to focus).
- Apogee distance = $a + c$ (farthest point).

So: $a - c = 6571$ and $a + c = 8371$. Adding: $2a = 14942$, $a = 7471$. Subtracting: $2c = 1800$, $c = 900$. Then $b^2 = a^2 - c^2 = 7471^2 - 900^2 = 55{,}815{,}841 - 810{,}000 = 55{,}005{,}841$, so $b \approx 7416.6$ km.

Equation (in km, centered at the ellipse's geometric center, but with Earth's center offset 900 km from the origin):

$$\frac{x^2}{7471^2} + \frac{y^2}{7416.6^2} = 1$$

Eccentricity: $e = c/a = 900/7471 \approx 0.12$. The orbit is moderately elliptical (a circular orbit has $e = 0$).

The example uses Concept 1 (ellipse standard form) and the application of conics to physics.

[FIGURE: An ellipse with Earth at one focus, marked perigee and apogee points, axes labeled. The student should notice that one focus (Earth) is offset from the ellipse's center.]

---

## 6. Exercises

### Warm-up

**Exercise 12.1.** Identify the conic and find its center: $\frac{x^2}{9} + \frac{y^2}{16} = 1$. Difficulty: low.

**Exercise 12.2.** Find the vertex, focus, and directrix of $y^2 = 8x$. Difficulty: low.

### Application

**Exercise 12.3.** Write the equation of an ellipse with vertices at $(\pm 6, 0)$ and minor-axis endpoints at $(0, \pm 4)$. Difficulty: medium.

**Exercise 12.4.** Find the foci and asymptotes of $\frac{x^2}{4} - \frac{y^2}{9} = 1$. Difficulty: medium.

**Exercise 12.5.** Identify the conic: $4x^2 - 9y^2 + 16x + 18y - 29 = 0$. (Hint: complete the square.) Difficulty: medium.

### Synthesis

**Exercise 12.6.** Use the discriminant to identify $3x^2 + 5xy + 2y^2 - 4 = 0$. Difficulty: medium-high.

### Challenge

**Exercise 12.7.** A whispering gallery is built so that the foci are 60 ft apart and the ceiling is 30 ft high at the center. Find the equation of the elliptical ceiling cross-section. Difficulty: high.

---

## 7. Chapter Summary

You can now identify, graph, and write equations for all four conic sections — circle, ellipse, parabola, hyperbola. You can extract their key features (vertices, foci, asymptotes, directrix) from the standard forms. You can recognize a conic from its general second-degree equation using the discriminant. You can write conics in polar form with one focus at the origin.

The single idea that matters most: **all four conics are the locus of points satisfying a simple distance relationship to a focus (and possibly a second focus or a directrix).** The equations are different surfaces of the same underlying geometric idea.

---

## 8. Connections Forward

Chapter 13 — Sequences, Probability, and Counting Theory — is the final chapter, taking up the discrete mathematics that complements the continuous algebraic and geometric tools developed across the book.

---

### Sources (from chapter source files)

- *College Algebra*, source modules m49437 through m49442 (OpenStax-derived).
