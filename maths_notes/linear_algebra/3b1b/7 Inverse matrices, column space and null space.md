
[link](https://www.youtube.com/@3blue1brown)
### Inverse Matrices and Linear Systems

- Inverse matrices are transformations that **undo** the effect of the original transformation.
- Linear algebra helps us solve **systems of linear equations**, often written as:
$$ A\vec{x} = \vec{v} $$
- We are looking for a vector $\vec{x}$ such that, after applying transformation $A$, it lands on vector $\vec{v}$.
- If $\det(A) \ne 0$, there is **exactly one solution**, and we can write:
$$ \vec{x} = A^{-1} \vec{v} $$
- If $\det(A) = 0$, the transformation **squishes** space into a lower dimension, and **no inverse** exists — but a solution **may still exist**.
---
### Determinants, Rank, and Dimensions

- When a transformation **squishes** space:

    - The **rank** of the resulting matrix is smaller than that of the original.

    - The **determinant** is zero.

- A **3D transformation** with:

	- Full rank (rank = 3) means it fills all of 3D space (det $\ne 0$).
    
    - Rank = 2 means all vectors land on a 2D plane.
    
    - Rank = 1 means all vectors land on a line.
    
    - Squishing into a **point** (degenerate case) is also possible.

- For a **2×2 matrix**:

    - Rank = 2 means full rank.
    
    - Rank = 1 means the transformation squishes space onto a line.

- In general, when **rank = number of columns**, the matrix is said to be **full rank**.

---
### Column Space and Null Space

- The **column space** (or image) of a matrix $A$ is the set of all possible outputs $\vec{v}$ from $A\vec{x}$.

    - It is the **span of the columns** of $A$.
    
    - The **rank** is the number of dimensions in the column space.
    
    - The **zero vector** is always included in the column space.

- The **null space** (or kernel) of a matrix is the set of all vectors $\vec{x}$ such that:
$$ A\vec{x} = \vec{0} $$
- It includes all vectors that land on the origin after the transformation.

- In 3D:

    - If the transformation squishes space into a plane, the null space is a **line**.
        
    - If it squishes space onto a line, the null space is a **plane**.
    
- For matrices that are **not full rank**, many different vectors can land on zero.
---
### Why These Spaces Matter

- The **column space** tells us **when a solution exists** (i.e., is $\vec{v}$ in the column space?).

- The **null space** tells us **what the set of all possible solutions looks like**.
