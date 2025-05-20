8 Dot products and duality

[[https://youtu.be/LyGKycYT2v0?si=tc0P-RCh4vu6SNEk]]

### Basic Definition

- The **dot product** of two vectors involves:
    
    - Pairing up all the coordinates
    - Multiplying each pair together
    - Summing the results

Mathematically:

$$\vec{v} \cdot \vec{w} = v_1 w_1 + v_2 w_2 + \cdots + v_n w_n$$

### Geometric Interpretation
![[Screenshot 2025-05-20 at 22.04.06.png]]
- For vectors $\vec{v}$ and $\vec{w}$:

	- Imagine projecting $\vec{w}$ onto a line through the origin and the tip of $\vec{v}$

    - The dot product is:$$\vec{v} \cdot \vec{w} = |\vec{v}|\,|\vec{w}| \cos(\theta)$$
    - When the projection points in the **opposite direction**, the dot product is **negative**

---

## Dot Product as a Linear Transformation

### Linear Transformations to Numbers

- A linear transformation from a vector space to $\mathbb{R}$ can be expressed as a dot product.
- Dot product acts as a **linear transformation**:



### Matrix Interpretation

- Suppose a transformation sends:
    - $\vec{i}$ (unit x-vector) to $1$
    - $\vec{j}$ (unit y-vector) to $-2$
We start with the vector:
$$\vec{x} = 4\vec{i} + 3\vec{j}$$

Then apply the transformation $T$:

$$
T(\vec{x}) = 4 \cdot T(\vec{i}) + 3 \cdot T(\vec{j}) = 4 \cdot 1 + 3 \cdot (-2) = -2
$$


This is the same as matrix-vector multiplication:

$$
\begin{bmatrix}1 & -2\end{bmatrix}
\cdot
\begin{bmatrix}4 \\ 3\end{bmatrix}
= -2
$$



---

## Duality and Projections

### Duality Concept

- Any linear transformation $\vec{x} \mapsto \mathbb{R}$ corresponds to a **unique vector** $\vec{v}$ such that:
$$
T(\vec{x}) = \vec{v} \cdot \vec{x}
$$
- This is known as **duality**:
    - The **dual of a vector** is the transformation it defines

    - The **dual of a transformation** is the vector it corresponds to

### Projection Interpretation

- $\vec{u}$ is a unit vector 

![[Screenshot 2025-05-20 at 22.06.00.png]]
- Projecting onto a **diagonal line**:

    - The **y-coordinate** of $\vec{u}$ gives where $\vec{j}$ lands

    - The **x-coordinate** of $\vec{u}$ gives where $\vec{i}$ lands

- A $1 \times 2$ matrix containing the coordinates of $\vec{u}$ defines the projection transformation
    
- Applying this transformation is identical to computing:
$$
\vec{u} \cdot \vec{x}
$$
- That’s why:

    > Dotting a vector with a unit vector $\vec{u}$ is equivalent to projecting onto the span of $\vec{u}$ and taking the length


---

## Summary Insights

- The dot product measures **how aligned** two vectors are

- $\vec{v} \cdot \vec{w}$ is:

    - **Positive** when they point in similar directions
    
    - **Zero** when they are orthogonal

- The dot product serves as:

    - A **projection**
    
    - A **linear map**
    
    - A **bridge between vectors and transformations** (duality)