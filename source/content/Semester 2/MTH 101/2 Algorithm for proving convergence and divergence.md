# Algorithm for Proving Convergence or Divergence of a Sequence

## **Step 1: Define the Sequence**
1. Given a sequence $\{a_n\}$, express it as:
   $$
   a_n = f(n) \quad \text{for } n \in D
   $$
   where $D$ is usually $\mathbb{N}$ or $\mathbb{R}^+$.
2. Identify its **limit candidate** (if any) by:
   - Observing the formula of $a_n$.
   - Checking its behavior as $n \to \infty$.

---

## **Step 2: Check for Convergence**
A sequence **converges** if there exists a real number $L$ such that:
   $$
   \lim_{n \to \infty} a_n = L
   $$
This means that for every $\varepsilon > 0$, there exists an integer $N$ such that for all $n \geq N$:
   $$
   |a_n - L| < \varepsilon.
   $$

To **prove convergence**:
1. Find a candidate limit $L$.
2. Show that for any given $\varepsilon > 0$, you can find an $N$ such that the above inequality holds.

### **Common Strategies to Prove Convergence**
- **Limit Computation**: Evaluate $\lim\limits_{n \to \infty} a_n$ using:
  - Algebraic simplifications.
  - L'Hôpital's rule (for sequences defined by fractions).
  - Squeeze theorem (if bounding the sequence is possible).
- **Monotonicity & Boundedness Test**: If $\{a_n\}$ is **monotonic and bounded**, it **must converge**.

---

## **Step 3: Check for Divergence**
A sequence **diverges** if:
- $\lim\limits_{n \to \infty} a_n$ **does not exist**, or
- $\lim\limits_{n \to \infty} |a_n| = \infty$.

To **prove divergence**, check if:
1. $\{a_n\}$ **tends to $\pm\infty$**:
   - Show that for every real number $M > 0$, there exists an integer $N$ such that for all $n \geq N$:
     $$
     |a_n| > M.
     $$
   - This confirms $\lim\limits_{n \to \infty} a_n = \infty$ (or $-\infty$).
2. **The sequence oscillates** (i.e., does not settle to a single value).
   - Example: The sequence $\{(-1)^n\}$ **does not converge** because it alternates indefinitely.
   - Use the definition: if there exist two different limit points, the sequence **cannot** converge.

---

## **Step 4: Apply the Tests**
### ✅ **Convergence Examples**
1. **Example**: $\displaystyle a_n = \frac{1}{n}$
   - Candidate limit: $L = 0$.
   - For any $\varepsilon > 0$, choosing $N > \frac{1}{\varepsilon}$ ensures:
     $$
     \left| \frac{1}{n} - 0 \right| < \varepsilon.
     $$
   - Thus, $\lim\limits_{n \to \infty} \frac{1}{n} = 0$, so the sequence **converges**.

2. **Example**: $\displaystyle a_n = \frac{n}{n+1}$
   - Candidate limit: $L = 1$.
   - Compute:
     $$
     \lim_{n \to \infty} \frac{n}{n+1} = \lim_{n \to \infty} \frac{1}{1 + \frac{1}{n}} = 1.
     $$
   - The sequence **converges to 1**.

### ❌ **Divergence Examples**
1. **Example**: $\displaystyle a_n = n$
   - Clearly, $\lim\limits_{n \to \infty} n = \infty$, so it **diverges to infinity**.
2. **Example**: $\displaystyle a_n = (-1)^n$
   - The sequence oscillates between $-1$ and $1$.
   - Since it does not settle to a single value, it **does not converge**.

---

## **Generalized Approach**
1. **If $\lim\limits_{n \to \infty} a_n = L$ (finite), the sequence converges to $L$.**
2. **If $\lim\limits_{n \to \infty} a_n = \pm\infty$, the sequence diverges to infinity.**
3. **If the sequence oscillates indefinitely, it does not converge.**

---

