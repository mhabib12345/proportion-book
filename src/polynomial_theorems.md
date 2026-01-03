# 🧮 Polynomial Operations & Theorems

Before we can use advanced theorems, we must understand how to combine polynomial terms.

## 1. Adding and Subtracting: "Like Terms"
You can only add or subtract terms that have the **same variable** and the **same exponent**.

**Example:** $(3x^2 + 5x - 7) + (x^2 - 2x + 1)$
1. Group the $x^2$ terms: $3x^2 + 1x^2 = 4x^2$
2. Group the $x$ terms: $5x - 2x = 3x$
3. Group the constants: $-7 + 1 = -6$
**Result:** $4x^2 + 3x - 6$



---

## 2. The Remainder Theorem
This theorem is a massive time-saver. Instead of performing long division, you can find the remainder of a polynomial division instantly.

> **The Theorem:** If you divide a polynomial $P(x)$ by $(x - c)$, the remainder is simply $P(c)$.

**Example:** Find the remainder when $P(x) = x^3 - 2x^2 + 3$ is divided by $(x - 2)$.
* Instead of dividing, just plug in $2$ for $x$:
* $P(2) = (2)^3 - 2(2)^2 + 3$
* $P(2) = 8 - 8 + 3 = 3$
* **The Remainder is 3.**

---

## 3. The Factor Theorem
The Factor Theorem is a special case of the Remainder Theorem. It helps us find the "roots" or "zeros" of a polynomial.

> **The Theorem:** $(x - c)$ is a **factor** of $P(x)$ if and only if $P(c) = 0$.

### Why is this useful?
If $P(c) = 0$, it means the division has **no remainder**, so the polynomial passes exactly through the x-axis at that point.



**Example:** Is $(x - 1)$ a factor of $P(x) = x^2 - 3x + 2$?
1. Plug in $1$: $P(1) = (1)^2 - 3(1) + 2$
2. Calculate: $1 - 3 + 2 = 0$
3. **Yes!** Because the result is $0$, $(x - 1)$ is a factor.

---

## 4. Synthetic Division: The Shortcut
To apply these theorems quickly, we often use **Synthetic Division**, a shorthand method of polynomial division.



---

## 💡 Pro-Tip for your Book
When graphing these, remember:
* If $(x - c)$ is a factor, the graph **crosses** the x-axis at $c$.
* If the remainder is positive, the graph is **above** the axis at that point.