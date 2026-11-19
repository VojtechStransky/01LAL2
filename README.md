# 01LAL2

> **Coursework.** Programming tasks written in 2023 for the course 01LAL2
> *Linear Algebra 2* at the Faculty of Nuclear Sciences and Physical
> Engineering, CTU in Prague.

Three small interactive C++ programs. Each asks for a matrix on the keyboard,
number by number, and prints the result.

| File | Task | Method |
|---|---|---|
| `Solutions/inverse.cpp` | inverse of a square matrix | Gauss–Jordan elimination applied to the matrix and to an identity matrix at once |
| `Solutions/inverse1.cpp` | determinant, inverse and the solution of **A x = b** | determinant by elimination, inverse from the adjugate matrix, Cramer's rule |
| `Solutions/gsorto.cpp` | orthogonal basis from given vectors | Gram–Schmidt process with the inner product **uᵀ G v**; first checks that **G** is symmetric and positive definite and that the vectors are independent |

## Build and run

Needs a C++17 compiler.

```bash
g++ -std=c++17 Solutions/inverse.cpp -o inverse
./inverse
```

The programs read integers: first the size of the matrix, then its members
row by row.
