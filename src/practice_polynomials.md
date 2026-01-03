# ✍️ Practice Set: Polynomial Challenges

Test your skills using the **Horner Method**, **Remainder Theorem**, and **Factor Theorem**. Try to solve these on paper first, then click the "Solution" toggle to check your work.

---

### 🟢 Level 1: The Basics
**Problem 1:** Use the Horner Method to find the quotient and remainder of $(x^3 - 4x^2 + 2x + 5) \div (x - 3)$.

<details>
<summary><b>Click to see Solution</b></summary>

**Horner Table:**
| | 1 | -4 | 2 | 5 |
| :--- | :--- | :--- | :--- | :--- |
| **(3)** | ↓ | 3 | -3 | -3 |
| | **1** | **-1** | **-1** | **(2)** |

* **Quotient:** $x^2 - x - 1$
* **Remainder:** $2$
</details>

---

### 🟡 Level 2: The Missing Term
**Problem 2:** Find the remainder of $(2x^4 - 5x^2 + 6) \div (x + 2)$. 
*Hint: Don't forget the placeholders for $x^3$ and $x$!*

<details>
<summary><b>Click to see Solution</b></summary>

**Coefficients:** $2, 0, -5, 0, 6$  
**$k$ value:** $-2$

**Horner Table:**
| | 2 | 0 | -5 | 0 | 6 |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **(-2)**| ↓ | -4 | 8 | -6 | 12 |
| | **2** | **-4** | **3** | **-6** | **(18)** |

* **Remainder:** $18$
</details>

---

### 🟠 Level 3: The Factor Theorem
**Problem 3:** Is $(x - 1)$ a factor of $P(x) = x^3 + 2x^2 - x - 2$? Prove it using the Factor Theorem.

<details>
<summary><b>Click to see Solution</b></summary>

According to the Factor Theorem, if $P(1) = 0$, then $(x-1)$ is a factor.

$$P(1) = (1)^3 + 2(1)^2 - (1) - 2$$
$$P(1) = 1 + 2 - 1 - 2$$
$$P(1) = 0$$

**Conclusion:** Yes, $(x-1)$ is a factor because the remainder is zero.
</details>

---

### 🔴 Level 4: Solving for $k$
**Problem 4:** The polynomial $P(x) = x^3 + kx^2 - 4x + 1$ has a remainder of $5$ when divided by $(x - 2)$. Find the value of $k$.

<details>
<summary><b>Click to see Solution</b></summary>

Use the Remainder Theorem: $P(2) = 5$.

$$(2)^3 + k(2)^2 - 4(2) + 1 = 5$$
$$8 + 4k - 8 + 1 = 5$$
$$4k + 1 = 5$$
$$4k = 4$$
**$k = 1$**
</details>

---

### 🟣 Level 5: Horner-Kino Challenge
**Problem 5:** Divide $P(x) = x^4 - 3x^3 + 5x^2 - 2x + 1$ by $(x^2 - x - 2)$.

<details>
<summary><b>Click to see Solution</b></summary>

**Multipliers:** $m_1 = 1, m_2 = 2$ (derived from $x^2 - x - 2$).

**Quotient Result:** $x^2 - 2x + 5$  
**Remainder Result:** $-x + 11$

*(This uses the two-row multiplication method discussed in the Horner-Kino section.)*
</details>