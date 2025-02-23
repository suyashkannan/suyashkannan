

# Algorithm for Finding $\inf(A)$ and $\sup(A)$

## Step 1: Identify the Set and Its Behavior
1. Express the set $A$ as:
   $$
   A = \{ f(n) \mid n \in D \}
   $$
   where $D$ is the domain (e.g., $\mathbb{N}$ or $\mathbb{R}^+$).
2. Analyze the behavior of $f(n)$:
   - Find what happens as $n \to \infty$.
   - Find what happens as $n \to 1$ (or other relevant boundaries).
3. Identify **upper and lower bounds**.

---

## Step 2: Finding the Infimum $\inf(A)$
1. **Find a candidate lower bound** $L$:
   - If $f(n)$ is decreasing and approaches $L$, then $L$ is a candidate.
   - Show that $f(n) \geq L$ for all $n$.
2. **Prove that $L$ is the greatest lower bound**:
   - For any $x > L$, find an $n$ such that:
     $$
     f(n) < x
     $$
   - This shows that $x$ **is not a lower bound**.
   - Conclude that:
     $$
     \inf(A) = L
     $$

---

## Step 3: Finding the Supremum $\sup(A)$
1. **Find a candidate upper bound** $U$:
   - If $f(n)$ is increasing and approaches $U$, then $U$ is a candidate.
   - Show that $f(n) \leq U$ for all $n$.
2. **Prove that $U$ is the least upper bound**:
   - For any $y < U$, find an $n$ such that:
     $$
     f(n) > y
     $$
   - This shows that $y$ **is not an upper bound**.
   - Conclude that:
     $$
     \sup(A) = U
     $$

---

## Lastly:
1. Show that the sequence is decreasing for inf and increasing for sup.
2. In order to do that, simply show that $x_{n}\leq x_{n+1}$ for increasing sequence and vice versa for decreasing sequence.
