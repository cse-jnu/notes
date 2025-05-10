# Numerical Methods Cheat Sheet

## 1. Numerical Integration

| Method               | When to Use                                      | Requirement               | Accuracy     |
|----------------------|--------------------------------------------------|----------------------------|--------------|
| **Trapezoidal Rule** | Basic estimate; works with any `n`              | Any `n`                    | Low          |
| **Simpson’s 1/3**    | Smooth functions, even `n`                      | `n` must be even           | Medium-High  |
| **Simpson’s 3/8**    | Use when `n % 3 = 0`                            | `n` must be multiple of 3  | Medium-High  |
| **Gauss-Legendre**   | High accuracy, known weight functions           | Special nodes/weights      | Very High    |

---

## 2. Numerical Differentiation

| Method                | When to Use                                      | Formula                    | Accuracy     |
|-----------------------|--------------------------------------------------|-----------------------------|--------------|
| **Forward Difference**| First-order approx, known `f(x)` at few points  | `f'(x) ≈ (f(x+h) - f(x))/h` | Low          |
| **Backward Difference**| Similar to forward but backward                 | `f'(x) ≈ (f(x) - f(x-h))/h` | Low          |
| **Central Difference**| Better accuracy; `f(x)` on both sides           | `f'(x) ≈ (f(x+h) - f(x-h))/(2h)` | Medium   |
| **Higher-Order**       | More precision, large data sets                 | Depends on derivative order | High         |

---

## 3. Root Finding Methods

| Method                 | When to Use                                   | Needs Derivative? | Speed      | Convergence     |
|------------------------|-----------------------------------------------|--------------------|------------|------------------|
| **Bisection**          | Simple, safe; guaranteed if sign change       | No                 | Slow       | Guaranteed       |
| **Regula Falsi**       | Faster than bisection                         | No                 | Medium     | Semi-guaranteed  |
| **Newton-Raphson**     | Very fast; needs good initial guess           | Yes                | Fast       | Fast (if works)  |
| **Secant Method**      | Like Newton, but no derivative                | No                 | Fast       | Less stable      |
| **Fixed-Point Iter.**  | When written as `x = g(x)`                    | No                 | Medium     | Needs check      |

---

## TL;DR Decision Tree

- **Integration:**
  - Even `n` → Use **Simpson’s 1/3**
  - Any `n` → Use **Trapezoidal**
  - High precision → Use **Gauss**

- **Differentiation:**
  - Best accuracy → Use **Central Difference**
  - One side known → Use **Forward/Backward**

- **Root Finding:**
  - No derivative → Use **Bisection** or **Secant**
  - Fast + has derivative → Use **Newton-Raphson**

---
