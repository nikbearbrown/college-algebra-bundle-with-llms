# Chapter 1 — Prerequisites

## 1. Chapter Opening

It is winter at Vostok Station, on the East Antarctic Plateau, 11,000 feet above sea level. A satellite passes overhead. Its instruments record the surface temperature: −89.2°C. The number is not a curiosity. It is the coldest temperature ever measured on Earth, and the day it was recorded — July 21, 1983 — is one of the few days in history we know to that precision because someone wrote the number down [source m51240].

Look at the number for a moment: $-89.2°\text{C}$. It is *negative* — colder than freezing. It has a *decimal* — between two integers. It carries a *unit*. And it is *finite* — you could measure it again with a different instrument and get a slightly different number, but you would never get *infinity* or *nothing*. The single number sitting on that satellite readout uses, between its sign and its decimal point, more kinds of number than the natural counting numbers a child first learns. The Antarctic temperature is not exotic. It is the ordinary world, recorded honestly.

This chapter is about the numbers — and the rules for combining them — that the rest of college algebra will use as a working language. It is not a foreign language. You have spoken most of it your whole life, in fragments, when you split a bill, when you double a recipe, when you stretched a photograph and noticed it was twice as wide. What this chapter does is *name the parts*, *show the rules*, and *line them up in an order* so that when chapter 2 builds equations and chapter 3 builds functions, you have the vocabulary and the muscle memory to keep up.

The math here is foundational rather than glamorous. You will not solve mysteries. You will not derive Einstein's equations. What you will do is establish that $-89.2$ is a real number; that $4^3$ means $4 \cdot 4 \cdot 4$; that $\sqrt{50}$ simplifies to $5\sqrt{2}$; that $(x+3)(x-3) = x^2 - 9$; that $\frac{x^2 - 9}{x+3}$ simplifies to $x-3$ when $x \neq -3$. None of these is hard once you see it. The work is to see all of it without confusion, fluently, in the time it takes to read the next problem.

### Learning objectives

By the end of this chapter, you should be able to:

- **Classify** any number as natural, whole, integer, rational, irrational, or real, and place it on the number line.
- **Apply** the order of operations (PEMDAS) and the five properties of real numbers (commutative, associative, distributive, identity, inverse) to evaluate and simplify algebraic expressions.
- **Manipulate** exponents using the product, quotient, power, zero, and negative rules; convert between standard and scientific notation; and rewrite radicals using rational exponents.
- **Add, subtract, and multiply** polynomials, including using FOIL on binomials.
- **Factor** polynomials using GCF, trinomial factoring, grouping, perfect squares, difference of squares, and sum/difference of cubes — and use that factoring to simplify rational expressions.

### Prerequisites

Comfort with arithmetic — addition, subtraction, multiplication, division of integers and fractions. If $\frac{2}{3} + \frac{1}{4}$ is something you can do without thinking too hard, you are ready. If it isn't, the early sections will rebuild the skill from the ground up; you will not be left behind.

### Why this chapter matters

Every chapter that follows assumes the moves you are about to learn. Chapter 2 (Equations) assumes you can simplify an algebraic expression. Chapter 5 (Polynomial Functions) assumes you can factor a polynomial. Chapter 6 (Logarithms) assumes you can work with exponents. The whole sequence is a tower; this chapter is the foundation pour. Spend the time now and the rest of the term gets easier; rush this and every later chapter has hidden friction you cannot diagnose. *The fluency you build here is the difference between doing math and watching math happen.*

---

## 2. Concept 1 — Real Numbers and Their Properties

Stand at a roadside lemonade stand. A customer hands the kid running it a five-dollar bill for a $2.75 cup. The kid pulls $2.25 out of a tin can, looks at it, hands it back. That tiny exchange used at least three kinds of number — an integer (the bill), a decimal (the price), and a positive remainder (the change) — and one rule of arithmetic ($5 - 2.75 = 2.25$). The kid did not pause to ask whether $2.25$ was a "real number." It is. Most numbers are.

This concept names the kinds of number you have been using since elementary school, places them in a hierarchy, and then names the small handful of rules that say how they can be moved around without changing their value. Knowing the names matters because the rest of the book uses them. Knowing the rules matters because every algebraic manipulation in chapters 2 through 13 is built from this small set.

### The hierarchy of real numbers

The real numbers nest like Russian dolls.

**Natural numbers** $\mathbb{N} = \{1, 2, 3, 4, \ldots\}$. The counting numbers. What you used to count siblings, fingers, marbles in a bag. The set continues forever — the ellipsis means "and so on" — but every member is a positive whole.

**Whole numbers** $\mathbb{W} = \{0, 1, 2, 3, \ldots\}$. The naturals plus zero. Zero is a relatively recent addition to mathematics — it was introduced into the number system in India around the fifth century CE [source m51239]. Before that, mathematicians described emptiness with words rather than as a number you could put in an equation.

**Integers** $\mathbb{Z} = \{\ldots, -3, -2, -1, 0, 1, 2, 3, \ldots\}$. The whole numbers plus the negatives. Negative numbers were also introduced in India, in the seventh century, originally for tracking debts. The Antarctic temperature $-89.2$ has the negative integers in its sign.

**Rational numbers** $\mathbb{Q} = \left\{\frac{m}{n} \mid m, n \in \mathbb{Z}, n \neq 0\right\}$. Any number that can be written as a fraction of integers. *Rational* comes from the Latin *ratio*, meaning *reckoning* or *proportion*. Every integer is rational (write $7 = \frac{7}{1}$). Every terminating decimal is rational ($0.5 = \frac{1}{2}$). Every repeating decimal is rational ($0.\overline{36} = \frac{4}{11}$). The denominator $n$ cannot be zero — division by zero is undefined.

**Irrational numbers** $\mathbb{I}$. Numbers that *cannot* be written as a ratio of two integers. They are nonterminating *and* nonrepeating in decimal form. The diagonal of a unit square is $\sqrt{2} = 1.41421356\ldots$ — the digits never settle into a pattern. The circumference of a circle divided by its diameter is $\pi = 3.14159265\ldots$ — same. A garment maker measuring the ratio of the rim of a circular cloth to its diameter would, four thousand years ago, have noticed that the ratio is *just over 3* and never lands on a clean fraction. Irrational numbers exist because some geometric ratios refuse to be rational.

**Real numbers** $\mathbb{R}$. The rationals and irrationals together. Every real number sits at exactly one point on the number line, and every point on the number line corresponds to exactly one real number — a *one-to-one correspondence*. This is the universe of numbers we will operate inside of for the rest of this book.

The hierarchy: $\mathbb{N} \subset \mathbb{W} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R}$. Each set is contained in the next.

[FIGURE: A nested-rectangle diagram showing the hierarchy of number sets. The outermost rectangle is labeled "Real numbers ($\mathbb{R}$)" and contains a horizontal split — "Rationals ($\mathbb{Q}$)" on the left and "Irrationals" on the right. Inside Rationals, nested rectangles show "Integers ($\mathbb{Z}$)" containing "Whole numbers ($\mathbb{W}$)" containing "Naturals ($\mathbb{N}$)". Sample numbers placed in each region: $\sqrt{2}$ and $\pi$ in Irrationals; $\frac{2}{3}$ and $0.\overline{36}$ in Rationals (outside Integers); $-7$ in Integers (outside Whole); $0$ in Whole (outside Naturals); $5$ inside Naturals. The student should notice that every natural is a whole is an integer is a rational is a real, but not every real is a natural.]

### Order of operations

Most arithmetic mistakes are not arithmetic mistakes. They are agreement-of-order mistakes. Two students given the same expression $24 + 6 \cdot \frac{2}{3} - 4^2$ can produce different answers if they do the operations in different orders. To prevent this, mathematicians follow a fixed convention summarized by the acronym **PEMDAS**:

1. **P**arentheses (and any grouping symbols — brackets, braces, fraction bars, radicals, absolute-value bars).
2. **E**xponents and radicals.
3. **M**ultiplication and **D**ivision, left to right.
4. **A**ddition and **S**ubtraction, left to right.

The expression $24 + 6 \cdot \frac{2}{3} - 4^2$ resolves like this:

$$\begin{aligned}
24 + 6 \cdot \frac{2}{3} - 4^2 &= 24 + 6 \cdot \frac{2}{3} - 16 && \text{exponent first} \\
&= 24 + 4 - 16 && \text{multiplication} \\
&= 12 && \text{addition and subtraction, left to right}
\end{aligned}$$

The convention is arbitrary in the sense that mathematicians could have agreed on a different one. It is not arbitrary in the sense that, having agreed, *everyone follows the same one*. PEMDAS is a social contract that lets two strangers writing the same expression mean the same thing.

### The five properties of real numbers

For any real numbers $a$, $b$, $c$, the following always hold:

**Commutative** (order doesn't matter, for $+$ and $\cdot$):
$$a + b = b + a, \qquad a \cdot b = b \cdot a$$
*Subtraction and division are not commutative*: $17 - 5 \neq 5 - 17$.

**Associative** (grouping doesn't matter, for $+$ and $\cdot$):
$$(a + b) + c = a + (b + c), \qquad (a \cdot b) \cdot c = a \cdot (b \cdot c)$$
*Subtraction and division are not associative*: $8 - (3 - 15) \neq (8 - 3) - 15$ (the first is $20$, the second is $-10$).

**Distributive** (multiplication distributes over addition):
$$a \cdot (b + c) = a \cdot b + a \cdot c$$
This is the only property that connects two different operations. It is the single most-used identity in algebra; almost every later technique either applies it or undoes it.

**Identity** (there exist 0 for addition and 1 for multiplication that leave numbers unchanged):
$$a + 0 = a, \qquad a \cdot 1 = a$$

**Inverse** (every number has an opposite for addition; every nonzero number has a reciprocal for multiplication):
$$a + (-a) = 0, \qquad a \cdot \frac{1}{a} = 1 \text{ for } a \neq 0$$

These five rules look modest. They are. They are also what allow you to rearrange, regroup, and simplify any algebraic expression you will meet for the rest of college algebra and beyond. Every move in algebra is, at bottom, an application of one of these rules.

### Worked example — simplify a real-number expression

Simplify $\left(-\frac{23}{5}\right) \cdot \left[11 \cdot \left(-\frac{5}{23}\right)\right]$.

Notice the structure. Inside the brackets we have $11 \cdot (-\frac{5}{23})$. The whole expression multiplies that by $-\frac{23}{5}$. We can rearrange.

$$\begin{aligned}
\left(-\frac{23}{5}\right) \cdot \left[11 \cdot \left(-\frac{5}{23}\right)\right]
&= \left(-\frac{23}{5}\right) \cdot \left[\left(-\frac{5}{23}\right) \cdot 11\right] && \text{commutative property} \\
&= \left[\left(-\frac{23}{5}\right) \cdot \left(-\frac{5}{23}\right)\right] \cdot 11 && \text{associative property} \\
&= 1 \cdot 11 && \text{multiplicative inverse: } -\tfrac{23}{5} \cdot -\tfrac{5}{23} = 1 \\
&= 11 && \text{multiplicative identity}
\end{aligned}$$

Without the properties, you would multiply through and grind; with the properties, you spot that two factors cancel and the answer falls out. *The properties are how you do less work, not more.* That is the trade-off this concept names: a few abstract rules to memorize, paid back many times over in computational shortcuts.

### Trade-off

Naming and following these rules makes math precise and shareable across people. The cost is that they are rules — you cannot improvise. You cannot decide that $5 - 2$ should mean $-3$ today; you cannot rearrange $a^{b+c}$ as $a^b + a^c$ because *the distributive property does not apply that way*. The discipline is to learn which moves are licensed and which are not. The benefit is that, having learned, every two students working the same problem produce the same answer.

### Common misconceptions

**"Subtraction and division should commute."** They don't. $7 - 3 \neq 3 - 7$. The way to handle subtraction in algebra is often to *rewrite it as adding the opposite*: $a - b = a + (-b)$. Once you do that, you can use the commutative property of addition.

**"PEMDAS means addition before subtraction."** It doesn't. Addition and subtraction sit at the same level; you do them left to right. Same for multiplication and division. The "MD" and "AS" pairings are equal-priority partners, not orderings.

**"Zero divided by anything is zero, anything divided by zero is also zero."** Half right. $\frac{0}{5} = 0$. But $\frac{5}{0}$ is **undefined** — it has no value. Any expression with zero in a denominator is broken until you fix it. We will return to this in concept 3 with rational expressions.

---

## 3. Concept 2 — Exponents and Radicals

A single bacterial cell, given enough food, divides into two. Twenty minutes later, those two divide into four. Twenty minutes after that, eight. Then 16, 32, 64, 128, 256, 512, 1,024. After ten divisions — about three hours and twenty minutes — one cell has become $1,024 = 2^{10}$. After twenty divisions, $2^{20}$, just over a million. After thirty, more than a billion. *The growth is not arithmetic; it is exponential.* The number $2^{30}$ is the kind of number that forces you to invent shorthand.

The shorthand is *exponential notation*: $a^n$ means $a$ multiplied by itself $n$ times. Exponents are not a separate kind of arithmetic; they are *repeated multiplication*, packaged so we can talk about it without writing out the factors. From this single packaging trick, a small set of rules follows mechanically — and those rules govern not just bacterial growth, but compound interest, distances in space, the brightness of earthquakes, and the pH of your blood. This concept is about those rules.

### The five rules of exponents

For any real numbers $a$ and $b$ (with restrictions noted), and integers $m$ and $n$:

**Product rule** — when you multiply same-base powers, *add the exponents*:
$$a^m \cdot a^n = a^{m+n}$$
Why? Because $a^m \cdot a^n = (\underbrace{a \cdot a \cdots a}_{m \text{ factors}}) \cdot (\underbrace{a \cdot a \cdots a}_{n \text{ factors}}) = \underbrace{a \cdot a \cdots a}_{m+n \text{ factors}} = a^{m+n}$.

**Quotient rule** — when you divide same-base powers, *subtract the exponents*:
$$\frac{a^m}{a^n} = a^{m-n} \quad (a \neq 0)$$

**Power rule** — when you raise a power to a power, *multiply the exponents*:
$$(a^m)^n = a^{mn}$$
Reason: $(a^m)^n = a^m \cdot a^m \cdots a^m$ ($n$ times) $= a^{m+m+\cdots+m} = a^{mn}$.

**Zero exponent**:
$$a^0 = 1 \quad (a \neq 0)$$
This is forced by the quotient rule: $\frac{a^m}{a^m}$ equals $1$ (a number divided by itself), but the quotient rule says it also equals $a^{m-m} = a^0$. So $a^0$ must equal $1$.

**Negative exponent**:
$$a^{-n} = \frac{1}{a^n} \quad (a \neq 0)$$
Same logic: $\frac{a^0}{a^n} = \frac{1}{a^n}$, but by the quotient rule it equals $a^{0-n} = a^{-n}$. So $a^{-n}$ must equal $\frac{1}{a^n}$.

Two derived rules cover products and quotients raised to powers:

$$(ab)^n = a^n b^n \qquad \left(\frac{a}{b}\right)^n = \frac{a^n}{b^n} \quad (b \neq 0)$$

### Scientific notation — the practical payoff

The five exponent rules earn their place in every scientific calculation because of one consequence: they make absurdly large and absurdly small numbers tractable. The mass of an electron is approximately

$$0.0000000000000000000000000000009109 \text{ kg}$$

Try multiplying that by anything in the form above. You can't, without losing track of zeros. Now write it as

$$9.109 \times 10^{-31} \text{ kg}$$

Same number. Now multipliable. The notation $a \times 10^n$, where $1 \leq |a| < 10$ and $n$ is an integer, is called *scientific notation*. The exponent rules govern arithmetic in this notation directly:

$$(a \times 10^m)(b \times 10^n) = (ab) \times 10^{m+n}$$
$$\frac{a \times 10^m}{b \times 10^n} = \frac{a}{b} \times 10^{m-n}$$

The Earth-Sun distance is about $1.496 \times 10^{11}$ meters. The mass of the Sun is about $1.989 \times 10^{30}$ kg. Both are real measurements. Both are usable in calculations precisely because they have been put into scientific notation. *Without exponents, science could not record what it measures.*

### Radicals — the inverse of exponents

If $b^2 = a$, then $b$ is a *square root* of $a$. The notation $\sqrt{a}$ refers to the *principal* (non-negative) square root. So $\sqrt{25} = 5$, even though $(-5)^2 = 25$ as well — when we write $\sqrt{25}$, we mean only the positive root.

The same idea generalizes: $\sqrt[n]{a}$ is the $n$th root of $a$, the number whose $n$th power is $a$. So $\sqrt[3]{8} = 2$ because $2^3 = 8$.

The connection to exponents is more than analogy. Radicals *are* exponents — exponents that are fractions:

$$\sqrt{a} = a^{1/2}, \qquad \sqrt[n]{a} = a^{1/n}, \qquad \sqrt[n]{a^m} = a^{m/n}$$

This identification is one of the pivots of algebra. Once you accept that $\sqrt{a} = a^{1/2}$, all five exponent rules apply to radicals — you do not have to memorize a separate set.

**Product rule for radicals** (from the product rule for exponents):
$$\sqrt{a \cdot b} = \sqrt{a} \cdot \sqrt{b} \quad (a, b \geq 0)$$

This rule is what lets you simplify radicals. To simplify $\sqrt{50}$, factor 50 into a perfect square times something: $50 = 25 \cdot 2$. Then

$$\sqrt{50} = \sqrt{25 \cdot 2} = \sqrt{25} \cdot \sqrt{2} = 5\sqrt{2}$$

The expression $5\sqrt{2}$ is the *simplified* form of $\sqrt{50}$ — same value, written more cleanly.

**Quotient rule for radicals**:
$$\sqrt{\frac{a}{b}} = \frac{\sqrt{a}}{\sqrt{b}} \quad (a \geq 0, b > 0)$$

**Rationalizing the denominator**. Convention prefers radicals in numerators rather than denominators. To rewrite $\frac{2}{\sqrt{3}}$, multiply top and bottom by $\sqrt{3}$:

$$\frac{2}{\sqrt{3}} = \frac{2}{\sqrt{3}} \cdot \frac{\sqrt{3}}{\sqrt{3}} = \frac{2\sqrt{3}}{3}$$

The same value, written so that the denominator is rational. We will use this move repeatedly in later chapters.

### Worked example — simplify with exponents and radicals

Simplify $\left(\frac{x^3 y^{-2}}{x^{-1} y^4}\right)^{2}$ assuming $x \neq 0$ and $y \neq 0$.

Apply the quotient rule to each base:
$$\frac{x^3}{x^{-1}} = x^{3 - (-1)} = x^4, \qquad \frac{y^{-2}}{y^4} = y^{-2 - 4} = y^{-6}$$

So the expression inside the parentheses becomes $x^4 y^{-6}$. Now apply the power rule:
$$(x^4 y^{-6})^2 = x^{4 \cdot 2} y^{-6 \cdot 2} = x^8 y^{-12}$$

Convert the negative exponent to a positive one:
$$x^8 y^{-12} = \frac{x^8}{y^{12}}$$

Done. The final form has no negative exponents and no parentheses. *Each step was a single rule applied honestly.* That is what fluency looks like: each move named, each move legal.

### Trade-off

Exponential notation makes large and small numbers manageable; the cost is that the rules of arithmetic look different in this notation than they do for ordinary numbers. The student who tries to add exponents when multiplying *bases* — writing $(x + y)^2 = x^2 + y^2$, for instance — gets wrong answers. (The correct expansion is $x^2 + 2xy + y^2$, which we will derive in Concept 3.) The discipline is to *only apply the exponent rules where the structure justifies them*. They apply when bases are the same and the operation is multiplication or division. They do *not* generally apply across addition or subtraction.

### Common misconceptions

**"$(a+b)^2 = a^2 + b^2$."** False. $(a+b)^2 = a^2 + 2ab + b^2$. The cross term $2ab$ comes from the distributive property, which we'll see in Concept 3.

**"$a^{-n} = -a^n$."** False. $a^{-n} = \frac{1}{a^n}$. The negative exponent means *reciprocal*, not *opposite*.

**"$\sqrt{a + b} = \sqrt{a} + \sqrt{b}$."** False. Test it: $\sqrt{9 + 16} = \sqrt{25} = 5$, but $\sqrt{9} + \sqrt{16} = 3 + 4 = 7$. The product rule for radicals applies to *multiplication inside the radical*, not addition.

**"$\sqrt{x^2} = x$."** Half right. $\sqrt{x^2} = |x|$, the absolute value of $x$. If $x = -3$, then $\sqrt{x^2} = \sqrt{9} = 3 = |-3|$, not $-3$.

---

## 4. Concept 3 — Polynomials, Factoring, and Rational Expressions

Picture a rectangular garden with one side $x$ feet long and the other side $x + 3$ feet long. Its area, in square feet, is $x(x + 3) = x^2 + 3x$. That expression — $x^2 + 3x$ — is a *polynomial*. Most of the algebra you will do for the rest of college algebra (and most of pre-calculus, and most of a first calculus course) involves polynomials and the rational expressions you build by dividing them. This concept teaches you to add, subtract, and multiply polynomials; to factor them; and to use that factoring to simplify rational expressions.

### What a polynomial is

A *polynomial* in $x$ is a sum of terms of the form $a_n x^n$, where each $a_n$ is a real number (the *coefficient*) and each $n$ is a non-negative integer (the *exponent*). The general form:

$$a_n x^n + a_{n-1} x^{n-1} + \cdots + a_1 x + a_0$$

The largest exponent that appears is the *degree* of the polynomial. The coefficient on the highest-degree term is the *leading coefficient*. Examples:

- $4x^3 - 2x + 7$: degree 3, leading coefficient 4.
- $x^2 + 5$: degree 2, leading coefficient 1.
- $-6$: degree 0, leading coefficient $-6$ (a constant polynomial).
- $\frac{1}{x}$ is *not* a polynomial — the exponent on $x$ is $-1$, which is negative.
- $\sqrt{x} = x^{1/2}$ is *not* a polynomial — the exponent is $1/2$, not an integer.

The terminology used informally:

- A polynomial with one term is a *monomial*: $5x^2$.
- Two terms: *binomial*: $x + 3$.
- Three terms: *trinomial*: $x^2 + 5x + 6$.

### Adding, subtracting, and multiplying polynomials

**Addition and subtraction** combine *like terms* — terms with the same variable and same exponent.

$$(3x^2 + 2x - 5) + (x^2 - 4x + 7) = 4x^2 - 2x + 2$$

Subtraction first distributes the minus sign:

$$(3x^2 + 2x - 5) - (x^2 - 4x + 7) = 3x^2 + 2x - 5 - x^2 + 4x - 7 = 2x^2 + 6x - 12$$

**Multiplication** uses the distributive property repeatedly. To multiply $(2x + 3)(x - 4)$, distribute each term of the first factor across the second:

$$(2x + 3)(x - 4) = 2x \cdot x + 2x \cdot (-4) + 3 \cdot x + 3 \cdot (-4)$$
$$= 2x^2 - 8x + 3x - 12 = 2x^2 - 5x - 12$$

For binomials, the mnemonic **FOIL** — *First, Outer, Inner, Last* — names the four products in the order they typically appear. *FOIL is just the distributive property applied to two binomials*; it is not a separate rule.

**Special products** worth memorizing:

$$(a + b)^2 = a^2 + 2ab + b^2 \qquad \text{(perfect square)}$$
$$(a - b)^2 = a^2 - 2ab + b^2 \qquad \text{(perfect square)}$$
$$(a + b)(a - b) = a^2 - b^2 \qquad \text{(difference of squares)}$$

These three identities will appear constantly. Verify the first one yourself: $(a+b)^2 = (a+b)(a+b) = a \cdot a + a \cdot b + b \cdot a + b \cdot b = a^2 + 2ab + b^2$.

### Factoring — undoing multiplication

*Factoring* is the reverse process: given a polynomial, write it as a product of simpler polynomials. The reason factoring matters is that it converts addition into multiplication, and multiplication is what lets you find zeros, simplify rational expressions, solve equations, and graph curves. Most of the techniques in algebra route through a factoring step.

The standard moves:

**Greatest common factor (GCF).** Pull out what every term has in common.
$$6x^3 + 9x^2 - 3x = 3x(2x^2 + 3x - 1)$$

**Factoring trinomials with leading coefficient 1.** For $x^2 + bx + c$, look for two numbers that multiply to $c$ and add to $b$.
$$x^2 + 5x + 6 = (x + 2)(x + 3) \quad (\text{since } 2 \cdot 3 = 6 \text{ and } 2 + 3 = 5)$$

**Factoring trinomials with leading coefficient $\neq 1$.** Several methods exist; the most reliable is *factoring by grouping*. For $2x^2 + 7x + 3$, find two numbers that multiply to $2 \cdot 3 = 6$ and add to $7$. They are $1$ and $6$. Split the middle term:
$$2x^2 + 7x + 3 = 2x^2 + x + 6x + 3 = x(2x + 1) + 3(2x + 1) = (2x + 1)(x + 3)$$

**Difference of squares** (the inverse of the special product):
$$a^2 - b^2 = (a + b)(a - b)$$
So $x^2 - 9 = (x + 3)(x - 3)$, and $4x^2 - 25 = (2x + 5)(2x - 5)$.

**Perfect square trinomials**:
$$a^2 + 2ab + b^2 = (a + b)^2, \qquad a^2 - 2ab + b^2 = (a - b)^2$$
So $x^2 + 6x + 9 = (x + 3)^2$.

**Sum and difference of cubes**:
$$a^3 + b^3 = (a + b)(a^2 - ab + b^2)$$
$$a^3 - b^3 = (a - b)(a^2 + ab + b^2)$$
So $x^3 - 8 = (x - 2)(x^2 + 2x + 4)$.

There are no other techniques you need for this chapter. Every polynomial you meet in college algebra factors using some combination of these.

### Rational expressions

A *rational expression* is a polynomial divided by another polynomial. The simplest cases:

$$\frac{x^2 - 9}{x + 3}, \qquad \frac{x^2 + 5x + 6}{x + 2}, \qquad \frac{x + 1}{x^2 - 4}$$

Each looks complicated until you factor. The first becomes:
$$\frac{x^2 - 9}{x + 3} = \frac{(x + 3)(x - 3)}{x + 3} = x - 3 \quad \text{(provided } x \neq -3\text{)}$$

The cancellation is just division: any common factor in numerator and denominator can be removed, *with one important constraint* — the cancellation is only valid where the original denominator was nonzero. The simplified form $x - 3$ has the same value as the original *for all $x$ except $x = -3$*, where the original is undefined and the simplified version is $-6$.

This is one of the most important caveats in algebra. *Simplification preserves value where the original is defined; it does not extend the domain.* We carry the restriction as a note: $\frac{x^2 - 9}{x+3} = x - 3$ for $x \neq -3$.

**Operations on rational expressions** mirror operations on fractions.

*Multiply* — multiply tops, multiply bottoms, then simplify by canceling common factors:
$$\frac{x + 2}{x - 1} \cdot \frac{x - 1}{x + 3} = \frac{(x + 2)(x - 1)}{(x - 1)(x + 3)} = \frac{x + 2}{x + 3} \quad (x \neq 1, -3)$$

*Divide* — multiply by the reciprocal:
$$\frac{a}{b} \div \frac{c}{d} = \frac{a}{b} \cdot \frac{d}{c}$$

*Add or subtract* — find a common denominator first:
$$\frac{1}{x} + \frac{1}{x+1} = \frac{x+1}{x(x+1)} + \frac{x}{x(x+1)} = \frac{2x + 1}{x(x+1)}$$

### Worked example — simplify a rational expression

Simplify $\dfrac{x^2 + 5x + 6}{x^2 - 9}$.

Factor numerator and denominator:
$$x^2 + 5x + 6 = (x + 2)(x + 3) \quad (\text{trinomial factoring})$$
$$x^2 - 9 = (x + 3)(x - 3) \quad (\text{difference of squares})$$

Substitute:
$$\frac{x^2 + 5x + 6}{x^2 - 9} = \frac{(x + 2)(x + 3)}{(x + 3)(x - 3)}$$

Cancel the common factor $(x + 3)$ — valid where $x + 3 \neq 0$, i.e. $x \neq -3$:
$$= \frac{x + 2}{x - 3} \quad (x \neq -3, 3)$$

The restrictions $x \neq -3, 3$ come from the original denominator, which is zero at both values. The simplified form is much easier to work with — and to graph, when chapter 3 introduces functions.

### Trade-off

Polynomials are powerful precisely because they have a small, regular structure (sum of $a_n x^n$ terms). The cost of that simplicity is that they cannot represent every possible relationship — they cannot capture exponential growth (which needs $a^x$, not $x^n$), nor periodic motion (which needs sines and cosines). Most of the rest of this book is about the function families that *complement* polynomials: rational functions, exponentials, logarithms, trigonometric functions. Polynomials are the foundation on which those richer families are built.

### Common misconceptions

**"You can cancel terms across addition."** No. $\frac{x + 5}{x + 3} \neq \frac{5}{3}$. You can only cancel *factors*, not *terms*. The expression $\frac{x + 5}{x + 3}$ does not simplify because nothing in the numerator factors out a copy of $x + 3$.

**"$(x + y)^2 = x^2 + y^2$."** False. The correct expansion has a middle term: $(x + y)^2 = x^2 + 2xy + y^2$.

**"After simplifying $\frac{x^2 - 9}{x + 3}$ to $x - 3$, the function values match everywhere."** No. They match where both are defined, but $x = -3$ is a hole in the original. We carry the restriction.

---

## 5. Integration — One Worked Example, All Three Concepts

Suppose you are setting up a small rectangular vegetable patch. The width is $x$ feet. The length is 3 feet more than twice the width. You want to lay weed-blocking fabric that costs $\$2.50$ per square foot. Express the cost as a function of $x$, simplify, and find the cost when $x = 4$.

**Step 1 — Set up the algebraic expression** (Concept 1 — real numbers and properties).

Length = $2x + 3$. Area = length × width = $x(2x + 3)$. Cost = $2.50 \times \text{area}$.

$$C = 2.50 \cdot x(2x + 3)$$

**Step 2 — Simplify using the distributive property** (Concept 1) and exponent rules (Concept 2).

$$C = 2.50 \cdot x(2x + 3) = 2.50(2x^2 + 3x) = 5x^2 + 7.5x$$

The simplified form is a polynomial in $x$ (Concept 3). It is degree 2, leading coefficient 5.

**Step 3 — Evaluate at $x = 4$** (Concept 1 — substituting and using order of operations).

$$C(4) = 5(4)^2 + 7.5(4) = 5 \cdot 16 + 30 = 80 + 30 = 110$$

The cost is $\$110$.

**Step 4 — Now suppose costs change**. If the fabric is on sale at half price for week one and full price for week two, and you split your fabric purchase 60/40 between the two weeks, the effective cost per square foot is

$$0.6 \cdot 1.25 + 0.4 \cdot 2.50 = 0.75 + 1.00 = 1.75$$

Cost at $x = 4$ becomes $1.75 \cdot 4(2 \cdot 4 + 3) = 1.75 \cdot 4 \cdot 11 = 77$. The point isn't the savings; it is that the algebraic structure $x(2x + 3)$ doesn't change. Once you have built the expression in terms of $x$, replacing the price coefficient is one substitution. *The polynomial form lets you change one input without rebuilding the calculation.* That portability is the design philosophy of algebra in miniature: *separate the structure from the values, so you can substitute either one freely.*

[FIGURE: A small rectangle diagram showing the garden — labeled $x$ on the short side and $2x+3$ on the long side, with the area $x(2x+3)$ filled in inside. Below the rectangle, a one-line equation chain: $C = 2.50 \cdot x(2x+3) = 2.50(2x^2 + 3x) = 5x^2 + 7.5x$. The student should notice that the geometry produces the polynomial directly, and that the polynomial form is what lets the cost coefficient change without redrawing the rectangle.]

### Design philosophy of the field

College algebra has a single underlying claim: *most quantitative relationships in the physical, financial, and engineering world can be expressed as functions, most of which are built from polynomials, rational expressions, exponentials, logarithms, and trigonometric functions.* The chapter you have just read is the lowest layer of the construction — the numbers, the rules for combining them, the polynomials and rational expressions that name basic relationships. Every later chapter adds another family of function or another structure built from these pieces. You are not learning thirteen disconnected topics; you are learning thirteen layers of one architecture.

---

## 6. Exercises

### Warm-up

**Exercise 1.1.** *Tests Learning Objective 1.* Classify each number as natural, whole, integer, rational, or irrational. (a) $-7$ (b) $\frac{4}{9}$ (c) $\sqrt{16}$ (d) $\sqrt{17}$ (e) $0.\overline{6}$ (f) $\pi$. Difficulty: low.

**Exercise 1.2.** *Tests Learning Objective 2.* Evaluate using the order of operations. (a) $20 - 3(2)^2$ (b) $\frac{30 - 6}{4 + 2}$ (c) $|3 - 8| + 2(5 - 1)$. Difficulty: low.

**Exercise 1.3.** *Tests Learning Objective 3.* Simplify each expression using exponent rules, leaving no negative exponents. (a) $x^4 \cdot x^{-2}$ (b) $\frac{y^7}{y^3}$ (c) $(2a^3)^2$ (d) $\left(\frac{x^2}{y}\right)^{-1}$. Difficulty: low.

### Application

**Exercise 1.4.** *Tests Learning Objective 2.* Identify which property justifies each step:
$$3(x + 5) + 2 = 3x + 15 + 2 = 3x + 17$$
Difficulty: medium.

**Exercise 1.5.** *Tests Learning Objective 3.* The Earth-Moon distance averages $3.844 \times 10^8$ meters. Light travels at $2.998 \times 10^8$ m/s. How long does light take to travel from the Moon to Earth? Give your answer in scientific notation. Difficulty: medium.

**Exercise 1.6.** *Tests Learning Objective 3.* Simplify $\sqrt{72} + \sqrt{18}$ to a single radical. Difficulty: medium.

**Exercise 1.7.** *Tests Learning Objective 4.* Multiply $(2x - 3)(x^2 + 4x - 1)$ and simplify. Difficulty: medium.

**Exercise 1.8.** *Tests Learning Objective 5.* Factor each polynomial completely. (a) $x^2 - 8x + 15$ (b) $4x^2 - 25$ (c) $x^3 + 27$ (d) $6x^2 + 11x - 10$. Difficulty: medium.

### Synthesis

**Exercise 1.9.** *Tests Learning Objectives 4 and 5.* Simplify $\dfrac{x^2 - 4}{x^2 + 4x + 4}$ and state the restrictions on $x$. Difficulty: medium-high.

**Exercise 1.10.** *Tests Learning Objectives 3 and 4.* A square has side length $\sqrt{75} - \sqrt{12}$. Express its area in simplest radical form. Difficulty: medium-high.

**Exercise 1.11.** *Tests Learning Objectives 2 and 5.* The volume of a rectangular box with square base of side $x$ and height $h$ is $V = x^2 h$. Suppose the box's height is $3$ feet less than twice its base side. Write the volume as a polynomial in $x$ alone, then factor that polynomial. Difficulty: medium-high.

### Challenge

**Exercise 1.12.** *Tests all learning objectives.* A photograph of dimensions $L \times W$ is set in a mat of uniform width $w$. The total area (mat plus photo) is $A = (L + 2w)(W + 2w)$. (a) Expand $A$ as a polynomial in $w$. (b) Identify the leading coefficient and degree. (c) Compute $A$ when $L = 24$ in, $W = 18$ in, $w = 3$ in. (d) Express the *area of the mat alone* (excluding the photo) as a simplified polynomial in $w$. Difficulty: high.

**Exercise 1.13.** *Tests Learning Objectives 3, 4, 5.* A square of side $a$ has a smaller square of side $b$ removed from one corner. Show, by both factoring and direct computation, that the remaining area equals $(a + b)(a - b)$. Difficulty: high.

---

## 7. Chapter Summary

You can do something now you may not have been able to do an hour ago. You can take any number — Antarctic temperature, mass of an electron, your phone bill total — and place it in the right slot of the real number hierarchy. You can take an algebraic expression with multiple operations and simplify it correctly because PEMDAS and the five properties of real numbers are now tools you reach for, not rules you have to look up. You can read $a^n$ as repeated multiplication, manipulate it using five rules, and convert between standard and scientific notation without losing zeros. You can multiply two binomials using the distributive property, factor a polynomial using a small set of techniques (GCF, trinomial, grouping, perfect squares, difference of squares, sum/difference of cubes), and use that factoring to simplify a rational expression while remembering to track restrictions on the variable.

The single idea that matters most: **algebra is a small set of rules applied consistently across many surface forms.** Every move you will make in chapters 2 through 13 is built from the moves you just learned — the distributive property unfolding, the exponent rules combining, polynomials being factored and recombined. The volume of material in later chapters is large; the underlying machinery is what you have right here.

The common mistake to watch for: confusing *the surface form of an expression* with *the values it takes*. Two expressions can look different and represent the same value (the whole point of simplification); two expressions can look similar and represent different values (the trap of "$(x+y)^2 = x^2 + y^2$"). The discipline is to stay close to the rules — apply only what is licensed, restrict where the original was undefined, check by substituting numbers when you are uncertain.

If you want a test of your understanding: take a friend's phone number, treat the digits as coefficients of a polynomial, factor it (or note that it doesn't factor cleanly), then simplify a rational expression built from it. If the moves feel mechanical, you have the fluency. If they feel uncertain, the part you stumble on is the part to revisit.

---

## 8. Connections Forward

This chapter built the algebraic raw material — numbers, exponents, polynomials, rational expressions. The next chapter — Equations and Inequalities — turns these expressions into *equations*: statements that two expressions are equal, with one or more unknowns to solve for. Solving equations is the central activity of college algebra, and every technique for it depends on the simplification moves you just learned. Linear equations are the simplest case; quadratic equations require factoring or the quadratic formula (which is itself a worked-out factoring); rational and radical equations require careful tracking of the domain restrictions you began here. The expressions you can simplify, you will soon be solving. Read on.

---

### Sources (from chapter source files)

- *College Algebra* with Co-Requisite Skills, source modules m51239 through m51248 (OpenStax-derived).
