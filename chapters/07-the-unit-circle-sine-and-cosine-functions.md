# Chapter 7 — The Unit Circle: Sine and Cosine Functions

## 1. Chapter Opening

A Ferris wheel turns slowly outside a county fair, twenty cars distributed evenly around its rim. Watch one car. Its height above the ground rises, peaks at the top, falls, bottoms out near the ground, rises again. Plot the height against time and you get a smooth, regular wave — a *sinusoid*. The same wave appears in tides, in alternating current, in sound, in the swing of a pendulum, in seasonal temperature cycles. *Anything that returns to where it started, periodically, is a candidate for trigonometric description.*

Trigonometry began as the measurement of triangles — *trigonon* + *metron*, Greek for "triangle measure" — but its modern domain extends far beyond triangles. The unit circle is the central tool. Each point on the unit circle has coordinates that depend on the angle from the positive $x$-axis; those coordinates are exactly the cosine and sine of the angle. From this construction follows everything else: trigonometric identities, the graphs of sine and cosine waves, the analysis of periodic phenomena.

### Learning objectives

By the end of this chapter, you should be able to:

- **Convert** between degree and radian measures of an angle.
- **Find** coterminal and reference angles, the length of an arc, and the area of a sector.
- **Use** right-triangle trigonometry (sine, cosine, tangent and their reciprocals) to find unknown sides and angles.
- **Evaluate** sine and cosine at standard angles using the unit circle, and identify their domain and range.
- **Apply** the fundamental Pythagorean identity $\sin^2\theta + \cos^2\theta = 1$ and the cofunction relationships.

### Prerequisites

Chapters 1–3 (algebraic manipulation, function concept). Chapter 5 (rational functions for cofunctions). Geometry concepts: right triangle, Pythagorean theorem, similar triangles.

---

## 2. Concept 1 — Angles, Arcs, and Sectors

An *angle* is the figure formed by two rays sharing a common endpoint. The angle is measured by the amount of rotation from one ray (the *initial side*) to the other (the *terminal side*). Counterclockwise is positive; clockwise is negative.

### Degrees and radians

Two systems of angle measure:

- **Degrees**: $360°$ in a full circle. Familiar from everyday geometry.
- **Radians**: $2\pi$ radians in a full circle. The natural unit for advanced mathematics.

A *radian* is defined as the angle subtending an arc equal in length to the radius. So an arc of length $r$ on a circle of radius $r$ corresponds to 1 radian.

**Conversion:**
$$\pi \text{ radians} = 180°, \quad 1 \text{ rad} = \frac{180°}{\pi} \approx 57.3°, \quad 1° = \frac{\pi}{180} \text{ rad}$$

So $30° = \frac{\pi}{6}$ rad, $90° = \frac{\pi}{2}$ rad, $180° = \pi$ rad, $360° = 2\pi$ rad.

### Coterminal and reference angles

Two angles are *coterminal* if they have the same terminal side. They differ by a full revolution: $360°$ or $2\pi$ rad. So $30°$ and $390°$ and $-330°$ are all coterminal.

A *reference angle* is the acute angle between the terminal side and the $x$-axis. It's always positive, always between $0$ and $90°$ (or $0$ and $\pi/2$ rad). Reference angles let you reduce any trig calculation to one in the first quadrant.

For example: the reference angle for $210°$ is $30°$ (since $210° = 180° + 30°$); for $315°$ is $45°$ (since $360° - 45° = 315°$).

### Arc length and sector area

For a circle of radius $r$ and a central angle $\theta$ in radians:

- *Arc length:* $s = r\theta$
- *Sector area:* $A = \frac{1}{2}r^2\theta$

These formulas require $\theta$ in radians. (In degrees: $s = \frac{\theta \pi r}{180}$ and $A = \frac{\theta \pi r^2}{360}$.)

**Example.** A pizza of radius 9 inches is cut into 8 equal slices. Find the arc length and area of one slice.

Each slice has central angle $\frac{2\pi}{8} = \frac{\pi}{4}$ rad. Arc length: $s = 9 \cdot \frac{\pi}{4} \approx 7.07$ in. Area: $A = \frac{1}{2}(9)^2 \cdot \frac{\pi}{4} \approx 31.8$ in².

### Linear and angular speed

A point moving on a circular path has both *linear speed* (distance per time) and *angular speed* (angle per time). They are related:

$$v = r\omega$$

where $v$ is linear speed, $\omega$ is angular speed in radians per unit time, and $r$ is the radius.

**Example.** A bicycle wheel of radius 14 inches rotates at $5$ revolutions per second. Linear speed at the rim?

$\omega = 5 \cdot 2\pi = 10\pi$ rad/sec. Linear speed: $v = 14 \cdot 10\pi = 140\pi \approx 440$ in/sec, or about 25 mph.

---

## 3. Concept 2 — Right-Triangle Trigonometry

In a right triangle, the six trigonometric functions of an acute angle $\theta$ are defined as ratios of side lengths.

Let the side opposite $\theta$ have length $\text{opp}$, the adjacent side have length $\text{adj}$, and the hypotenuse have length $\text{hyp}$. Then:

$$\sin\theta = \frac{\text{opp}}{\text{hyp}}, \quad \cos\theta = \frac{\text{adj}}{\text{hyp}}, \quad \tan\theta = \frac{\text{opp}}{\text{adj}}$$

The reciprocal functions:

$$\csc\theta = \frac{\text{hyp}}{\text{opp}}, \quad \sec\theta = \frac{\text{hyp}}{\text{adj}}, \quad \cot\theta = \frac{\text{adj}}{\text{opp}}$$

The mnemonic *SOH-CAH-TOA* captures sine-cosine-tangent: Sine = Opposite/Hypotenuse, Cosine = Adjacent/Hypotenuse, Tangent = Opposite/Adjacent.

### Special triangles

Two right triangles produce nice exact values:

**45-45-90.** Sides in ratio $1 : 1 : \sqrt{2}$. So $\sin 45° = \cos 45° = \frac{\sqrt{2}}{2}$, $\tan 45° = 1$.

**30-60-90.** Sides in ratio $1 : \sqrt{3} : 2$. So $\sin 30° = \cos 60° = \frac{1}{2}$, $\sin 60° = \cos 30° = \frac{\sqrt{3}}{2}$, $\tan 30° = \frac{1}{\sqrt{3}}$, $\tan 60° = \sqrt{3}$.

### Cofunction relationships

In a right triangle, the two non-right angles are *complementary*: they sum to $90°$. The trigonometric functions of complementary angles are related:

$$\sin(90° - \theta) = \cos\theta, \quad \cos(90° - \theta) = \sin\theta$$
$$\tan(90° - \theta) = \cot\theta, \quad \cot(90° - \theta) = \tan\theta$$

This is why they're called *co*-functions.

### Worked example — distance from base of building

A surveyor stands $50$ ft from the base of a building. The angle of elevation to the top is $40°$. Height of the building?

Let $h$ = height. Then $\tan 40° = \frac{h}{50}$, so $h = 50 \tan 40° \approx 50 \cdot 0.839 \approx 41.9$ ft.

---

## 4. Concept 3 — The Unit Circle and Sine/Cosine Beyond Triangles

The unit circle is the circle of radius 1 centered at the origin: $x^2 + y^2 = 1$.

For any angle $\theta$ (measured from the positive $x$-axis, counterclockwise), draw the terminal ray. The point where it intersects the unit circle has coordinates $(\cos\theta, \sin\theta)$.

This *defines* sine and cosine for *all* real numbers, not just acute angles. The right-triangle definitions still work in the first quadrant; the unit-circle definition extends them everywhere.

### Standard angle values

| $\theta$ (rad) | $\theta$ (deg) | $\cos\theta$ | $\sin\theta$ |
|---|---|---|---|
| $0$ | $0°$ | $1$ | $0$ |
| $\pi/6$ | $30°$ | $\sqrt{3}/2$ | $1/2$ |
| $\pi/4$ | $45°$ | $\sqrt{2}/2$ | $\sqrt{2}/2$ |
| $\pi/3$ | $60°$ | $1/2$ | $\sqrt{3}/2$ |
| $\pi/2$ | $90°$ | $0$ | $1$ |
| $\pi$ | $180°$ | $-1$ | $0$ |
| $3\pi/2$ | $270°$ | $0$ | $-1$ |
| $2\pi$ | $360°$ | $1$ | $0$ |

### Domain, range, and signs

Both $\sin$ and $\cos$ have domain all real numbers and range $[-1, 1]$.

The signs of sine and cosine in each quadrant — useful for evaluating and graphing:

| Quadrant | $\cos\theta$ | $\sin\theta$ |
|---|---|---|
| I | $+$ | $+$ |
| II | $-$ | $+$ |
| III | $-$ | $-$ |
| IV | $+$ | $-$ |

Mnemonic: *All Students Take Calculus* — All trig functions positive in Q I; only Sine in Q II; only Tangent in Q III; only Cosine in Q IV.

### Reference angle technique

To find $\sin(150°)$: reference angle is $180° - 150° = 30°$. So $|\sin(150°)| = \sin(30°) = 1/2$. Quadrant II → sine positive. So $\sin(150°) = 1/2$.

To find $\cos(225°)$: reference angle $45°$. $|\cos(225°)| = \frac{\sqrt{2}}{2}$. Quadrant III → cosine negative. So $\cos(225°) = -\frac{\sqrt{2}}{2}$.

### The Pythagorean identity

The unit circle's defining equation $x^2 + y^2 = 1$ becomes, when $(x, y) = (\cos\theta, \sin\theta)$:

$$\sin^2\theta + \cos^2\theta = 1$$

This is the *fundamental Pythagorean identity*. It holds for every real $\theta$. It is the most-used identity in trigonometry.

Two consequences:

$$1 + \tan^2\theta = \sec^2\theta$$
$$1 + \cot^2\theta = \csc^2\theta$$

These follow from dividing the fundamental identity by $\cos^2\theta$ or $\sin^2\theta$.

### Even/odd functions

$\cos$ is *even*: $\cos(-\theta) = \cos\theta$ (the $x$-coordinate doesn't depend on direction of rotation).

$\sin$ is *odd*: $\sin(-\theta) = -\sin\theta$ (the $y$-coordinate flips).

These are visible on the unit circle: rotating counterclockwise by $\theta$ vs. clockwise by $\theta$ gives points symmetric across the $x$-axis.

---

## 5. Integration — One Worked Problem

A clock's minute hand is 5 inches long. (a) What angle (in radians) does it sweep in 20 minutes? (b) What is the arc length traced by the tip? (c) What is the area swept by the hand? (d) If the tip's position is given by $(x, y)$ at time $t$ measured from 12 o'clock (in minutes), express $x$ and $y$ in terms of $t$.

**(a) Angle.** A full revolution (60 minutes) is $2\pi$ rad. So 20 minutes = $\frac{20}{60} \cdot 2\pi = \frac{2\pi}{3}$ rad.

**(b) Arc length.** $s = r\theta = 5 \cdot \frac{2\pi}{3} = \frac{10\pi}{3} \approx 10.47$ in.

**(c) Sector area.** $A = \frac{1}{2}r^2\theta = \frac{1}{2}(25)\frac{2\pi}{3} = \frac{25\pi}{3} \approx 26.18$ in².

**(d) Position.** The hand starts at 12 o'clock, pointing straight up. Going clockwise (the standard direction for clock hands), the position at time $t$ is

$$x(t) = 5\sin\left(\frac{\pi t}{30}\right), \quad y(t) = 5\cos\left(\frac{\pi t}{30}\right)$$

(Note: clock convention is clockwise, so the standard counterclockwise unit-circle parameterization gets adjusted — sine for $x$, cosine for $y$.)

The example uses Concept 1 (radians, arc length, sector area), Concept 2 (trig as ratio in a right triangle, since position is the projection), and Concept 3 (the unit circle as parameterizing angle to coordinates).

[FIGURE: Clock face with minute hand at 4 o'clock position (sweeping from 12). Annotated arc length, sector area, and angle. The student should notice that the trig functions parameterize circular motion.]

---

## 6. Exercises

### Warm-up

**Exercise 7.1.** Convert. (a) $60°$ to radians. (b) $\frac{3\pi}{4}$ rad to degrees. Difficulty: low.

**Exercise 7.2.** Find the reference angle. (a) $135°$. (b) $\frac{4\pi}{3}$. (c) $-30°$. Difficulty: low.

**Exercise 7.3.** Evaluate. (a) $\sin(\pi/6)$. (b) $\cos(\pi/3)$. (c) $\tan(\pi/4)$. (d) $\sin(3\pi/2)$. Difficulty: low.

### Application

**Exercise 7.4.** A ladder leans against a wall at angle $70°$ from the ground. The ladder is 12 ft long. How high up the wall does the ladder reach? Difficulty: medium.

**Exercise 7.5.** A circular pizza of radius 8 inches is cut into 6 equal slices. (a) Central angle of each slice (in radians). (b) Arc length of crust on one slice. (c) Area of one slice. Difficulty: medium.

**Exercise 7.6.** Evaluate using reference angles. (a) $\sin(120°)$. (b) $\cos(225°)$. (c) $\sin(-60°)$. Difficulty: medium.

### Synthesis

**Exercise 7.7.** A water wheel of diameter 20 ft rotates at 4 rpm. Find the angular speed (in rad/sec) and linear speed at the rim. Difficulty: medium-high.

**Exercise 7.8.** Verify the Pythagorean identity for $\theta = \pi/3$. Difficulty: medium-high.

### Challenge

**Exercise 7.9.** A satellite is in circular orbit 200 km above Earth's surface (Earth's radius ≈ 6371 km). It completes one orbit in 90 minutes. Find linear and angular speeds. Difficulty: high.

---

## 7. Chapter Summary

You can now convert any angle between degrees and radians. You can find reference angles, coterminal angles, arc lengths, and sector areas. You can use right-triangle trigonometry to solve geometric problems. You can evaluate sine, cosine, and tangent at any standard angle using the unit circle and reference-angle technique. You can apply the Pythagorean identity to relate trig functions.

The single idea that matters most: **sine and cosine are coordinates on the unit circle.** From that single fact follows everything else — the periodicity, the identities, the connection to right triangles, the application to circular motion.

---

## 8. Connections Forward

Chapter 8 takes the cosine and sine functions from this chapter and graphs them as functions of angle, producing the wave shapes that describe oscillation. The transformations (amplitude, period, phase) give us the toolkit for modeling tides, sound, and any periodic phenomenon.

---

### Sources (from chapter source files)

- *College Algebra*, source modules m51282 through m51286 (OpenStax-derived).
