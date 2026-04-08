<<<<<<< HEAD
# 3x3 Matrix Determinant Solver

## Student Information
- **Name**: Miranda, John Paul Benedict G.
- **Course**: Math 101 – Linear Algebra
- **School**: University of Perpetual Help System DALTA, Molino Campus
- **Assignment**: Programming Assignment 1 – 3x3 Matrix Determinant Solver
- **Date Completed**: April 7, 2024

## Assigned Matrix
The matrix assigned for this project is:
```
┌               ┐
│   4   3   6  │
│   2   5   1  │
│   3   4   2  │
└               ┘
```

## Solution Method
This program computes the determinant of the assigned 3×3 matrix using **cofactor expansion** along the first row. The formula is:

$$ \text{det}(A) = a_{11}C_{11} + a_{12}C_{12} + a_{13}C_{13} $$

Where $C_{ij} = (-1)^{i+j}M_{ij}$ and $M_{ij}$ are the 2×2 minors obtained by removing row `i` and column `j`.

Each minor is calculated using the 2×2 determinant formula: $\text{det} = ad - bc$.

### Step-by-Step Calculation:
1.  **Step 1 – Minor M₁₁**: Remove row 1 and column 1
    - `det([5,1],[4,2]) = (5×2) - (1×4) = 10 - 4 = 6`
2.  **Step 2 – Minor M₁₂**: Remove row 1 and column 2
    - `det([2,1],[3,2]) = (2×2) - (1×3) = 4 - 3 = 1`
3.  **Step 3 – Minor M₁₃**: Remove row 1 and column 3
    - `det([2,5],[3,4]) = (2×4) - (5×3) = 8 - 15 = -7`

### Cofactor Terms:
- **C₁₁** = `(+1) × 4 × 6 = 24`
- **C₁₂** = `(-1) × 3 × 1 = -3`
- **C₁₃** = `(+1) × 6 × -7 = -42`

### Final Determinant:
- **det(M)** = `24 + (-3) + (-42) = -21`

## How to Run

### Java Program
1.  Navigate to the project directory.
2.  Compile the Java file:
    ```sh
    javac DeterminantSolver.java
    ```
3.  Run the compiled class:
    ```sh
    java DeterminantSolver
    ```

### JavaScript Program
1.  Requires Node.js to be installed.
2.  Navigate to the project directory.
3.  Run the script:
    ```sh
    node determinat_solver.js
    ```

## Sample Output
Both programs produce the identical console output, showing a clear, step-by-step solution:
```
====================================================
  3x3 MATRIX DETERMINANT SOLVER
  Student: Miranda, John Paul Benedict G.
  Assigned Matrix:
====================================================
┌               ┐
│   4   3   6  │
│   2   5   1  │
│   3   4   2  │
└               ┘
====================================================
  Step 1 — Minor M₁₁: det([5,1],[4,2]) = (5×2)-(1×4) = 6
  Step 2 — Minor M₁₂: det([2,1],[3,2]) = (2×2)-(1×3) = 1
  Step 3 — Minor M₁₃: det([2,5],[3,4]) = (2×4)-(5×3) = -7

  Cofactor C₁₁ = (+1) × 4 × 6 = 24
  Cofactor C₁₂ = (-1) × 3 × 1 = -3
  Cofactor C₁₃ = (+1) × 6 × -7 = -42
----------------------------------------------------
  Determinant = 24 + (-3) + -42 = -21
====================================================
```

## Final Result
The determinant of the assigned matrix is **-21**.

Since the determinant is non-zero (-21 ≠ 0), the matrix is **invertible (non-singular)**.

## Files Included
- `DeterminantSolver.java` – Java implementation of the determinant solver.
- `determinat_solver.js` – JavaScript (Node.js) implementation of the solver.
- `README.md` – This documentation file.
=======
# Prog2-9302-AY225
Repository of Programming 2 section 9302-AY225
>>>>>>> 728392ffb455f3cb10d3578a93f70f310e18cb36
