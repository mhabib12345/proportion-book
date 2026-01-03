## 📝 Worked Example: The Horner Method

Let's solve a problem step-by-step to see how the numbers move through the "Bagan Horner."

**Problem:** Find the quotient and remainder when:
$$P(x) = x^4 - 3x^2 + 2x - 5$$ 
is divided by $(x - 2)$.

---

### 1. Identify the Coefficients
Before starting, look for "missing" powers of $x$. In this polynomial, there is no $x^3$ term. You **must** use **0** as a placeholder.

* **Coefficients:** 1 ($x^4$), 0 ($x^3$), -3 ($x^2$), 2 ($x$), -5 (constant)
* **Divisor ($k$):** Since we divide by $(x - 2)$, our $k = 2$.

---

### 2. The Horner Table Setup



| | $x^4$ | $x^3$ | $x^2$ | $x^1$ | $x^0$ |
| :--- | :--- | :--- | :--- | :--- | :--- |
| | **1** | **0** | **-3** | **2** | **-5** |
| **(2)** | ↓ | 2 | 4 | 2 | 8 |
| | **1** | **2** | **1** | **4** | **(3)** |

#### Step-by-Step Calculation:
1. **Drop:** Bring the first coefficient (**1**) straight down.
2. **Multiply & Add:** $1 \times 2 = 2$. Add to $0 \rightarrow$ **2**.
3. **Multiply & Add:** $2 \times 2 = 4$. Add to $-3 \rightarrow$ **1**.
4. **Multiply & Add:** $1 \times 2 = 2$. Add to $2 \rightarrow$ **4**.
5. **Multiply & Add:** $4 \times 2 = 8$. Add to $-5 \rightarrow$ **3**.

---

### 3. Interpreting the Result
The final number in the row is your **Remainder**, and the preceding numbers are the coefficients of the **Quotient**. 

> **Important:** The degree of the quotient is always one less than the original. Since we started with $x^4$, our result starts with $x^3$.

* **Quotient ($Q(x)$):** $1x^3 + 2x^2 + 1x + 4$
* **Remainder ($R$):** $3$

---

### 4. Verification (Remainder Theorem)
To ensure the Horner Method worked correctly, we can plug $x=2$ into the original equation:
$$P(2) = (2)^4 - 3(2)^2 + 2(2) - 5$$
$$P(2) = 16 - 12 + 4 - 5$$
$$P(2) = 3$$

The results match! 

---

### ⚠️ Common Pitfall: The "Zero" Placeholder
If you forget to include the **0** for the $x^3$ term, the entire calculation shifts:
* **Wrong:** $[1, -3, 2, -5]$ ❌
* **Correct:** $[1, 0, -3, 2, -5]$ ✅

Always double-check that your coefficients represent every power from the highest degree down to the constant.