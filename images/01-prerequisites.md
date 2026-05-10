# Figure briefs — Prerequisites (Chapter 1)

The chapter ships with two explicit `[FIGURE: ...]` placeholders. Three production candidates flagged.

---

## Figure 1: The hierarchy of real numbers

**Placement:** Section 2, *Concept 1*, after the description of the nested hierarchy.

**Description:** A nested-rectangle diagram.

- Outermost rectangle labeled **Real numbers** ($\mathbb{R}$).
- Inside, a horizontal split: **Rationals** ($\mathbb{Q}$) on the left, **Irrationals** on the right.
- Inside Rationals, nested rectangles: **Integers** ($\mathbb{Z}$) containing **Whole numbers** ($\mathbb{W}$) containing **Naturals** ($\mathbb{N}$).
- Sample numbers placed in each region:
  - Irrationals: $\sqrt{2}$, $\pi$, $e$ (if used later).
  - Rationals (outside Integers): $\frac{2}{3}$, $0.\overline{36}$, $-1.5$.
  - Integers (outside Whole): $-7$, $-2$.
  - Whole (outside Naturals): $0$.
  - Naturals: $1$, $5$, $42$.

**Pedagogical purpose:** The student should see at a glance that every natural is a whole is an integer is a rational is a real, but not every real is a natural. The visual relationship makes the abstract hierarchy concrete.

**Style notes:** Clean nested-rectangle layout, distinct colors per region, sample numbers placed deliberately near boundaries. Width: full text-block.

---

## Figure 2: The garden as polynomial

**Placement:** Section 5, *Integration*, after the worked example.

**Description:** A small rectangle diagram showing the vegetable garden.

- Short side labeled $x$.
- Long side labeled $2x + 3$.
- Inside the rectangle: $x(2x+3)$ written as the area.

Below the rectangle, a single one-line equation chain:
$$C = 2.50 \cdot x(2x+3) = 2.50(2x^2 + 3x) = 5x^2 + 7.5x$$

**Pedagogical purpose:** The student should notice that the geometry produces the polynomial directly, and that the polynomial form is what lets the cost coefficient change without redrawing the rectangle.

**Style notes:** Clean line drawing, dimensional labels in italics, equation chain in display format below. Width: half text-block, sized to keep both rectangle and equation legible.

---

## Figure 3 (candidate, not in current draft): The number line

**Placement:** Section 2, *Concept 1*, after the *Real numbers* paragraph mentioning the one-to-one correspondence.

**Description:** A horizontal number line from $-5$ to $5$, with integer tick marks. A few specific values marked above the line:
- $-\sqrt{2} \approx -1.414$
- $-\frac{1}{2}$
- $0$
- $\frac{2}{3}$
- $\pi \approx 3.14159$
- $\sqrt{17} \approx 4.123$

Each marked value labeled with both its symbolic form and its decimal approximation (if irrational).

**Pedagogical purpose:** The student should see that *every* point on the line corresponds to *exactly one* real number — and vice versa. The mix of rationals and irrationals on the line makes the density of the real number system visible.

**Style notes:** Clean horizontal line, equally-spaced integer ticks, marks above the line for the labeled values. Width: full text-block.

---

## Figure 4 (candidate, not in current draft): Difference of squares as area

**Placement:** Section 4, *Concept 3*, in the difference-of-squares subsection.

**Description:** A geometric proof of $a^2 - b^2 = (a+b)(a-b)$:

- A square of side $a$ with a smaller square of side $b$ removed from one corner.
- The remaining L-shape is dissected into two rectangles: one of dimensions $a \times (a-b)$, the other of dimensions $b \times (a-b)$.
- Combined, the two rectangles have total area $(a + b)(a - b)$.

**Pedagogical purpose:** The student should see that the algebraic identity has a geometric meaning — that factoring the difference of squares is not arbitrary symbolic manipulation but a recognition that two areas are the same.

**Style notes:** Clean two-panel layout: first panel shows the L-shape; second panel shows it dissected and rearranged into the two rectangles. Width: full text-block.

---

## Figure 5 (candidate, not in current draft): Bacterial growth as exponential

**Placement:** Section 3, *Concept 2*, in the cold-open paragraph.

**Description:** A simple plot showing the doubling sequence — $x$-axis is *number of divisions* (0 through 30), $y$-axis is *cell count* on a log scale. The curve is a straight line on the log scale, starting at $2^0 = 1$ and reaching $2^{30} \approx 1.07 \times 10^9$ at division 30.

A note alongside: *the same data on a linear scale would be invisible until the last few points.*

**Pedagogical purpose:** The student should see why exponential growth defeats linear thinking — the early divisions barely register; the late ones dominate everything. The log scale makes the underlying constant doubling visible.

**Style notes:** Clean two-panel layout (linear and log) showing the same data. Annotation pointing to the absurd scale change at the end. Width: full text-block.

---

## Notes on figures the source contains

The source modules reference several figures (Figure_01_00_001 through Figure_01_01_005 in the chapter opening; additional figures in m51246's polynomial discussion). Most are illustrative chapter-opener images. The source's number-line figure is referenced in m51239 but not provided as rendered content. Production should commission Figures 1 and 2 as priorities; figures 3–5 are useful additions if budget allows.
