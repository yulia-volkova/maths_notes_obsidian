## Dot Product – Concepts & Intuition

### Basic Definition

- The **dot product** of two vectors involves:
    
    - Pairing up all the coordinates
    - Multiplying each pair together
    - Summing the results


Mathematically:

v⃗⋅w⃗=v1w1+v2w2+⋯+vnwn\vec{v} \cdot \vec{w} = v_1 w_1 + v_2 w_2 + \cdots + v_n w_nv⋅w=v1​w1​+v2​w2​+⋯+vn​wn​

### Geometric Interpretation

- For vectors $\vec{v}$ and $\vec{w}$:

	- Imagine projecting $\vec{w}$ onto a line through the origin and the tip of $\vec{v}$

    - The dot product is:
    
        v⃗⋅w⃗=∣v⃗∣∣w⃗∣cos⁡(θ)\vec{v} \cdot \vec{w} = |\vec{v}| |\vec{w}| \cos(\theta)v⋅w=∣v∣∣w∣cos(θ)
    - When the projection points in the **opposite direction**, the dot product is **negative**

---

## Dot Product as a Linear Transformation

### Linear Transformations to Numbers

- A linear transformation from a vector space to $\mathbb{R}$ can be expressed as a dot product.
- Dot product acts as a **linear transformation**:
    T(x⃗)=a⃗⋅x⃗T(\vec{x}) = \vec{a} \cdot \vec{x}T(x)=a⋅x

### Matrix Interpretation

- Suppose a transformation sends:
    - $\vec{i}$ (unit x-vector) to $1$
    - $\vec{j}$ (unit y-vector) to $-2$
- For $\vec{x} = \langle 4, 3 \rangle$, decompose as:
    x⃗=4i⃗+3j⃗\vec{x} = 4 \vec{i} + 3 \vec{j}x=4i+3j​
- Then:
    T(x⃗)=4⋅T(i⃗)+3⋅T(j⃗)=4⋅1+3⋅(−2)=−2T(\vec{x}) = 4 \cdot T(\vec{i}) + 3 \cdot T(\vec{j}) = 4 \cdot 1 + 3 \cdot (-2) = -2T(x)=4⋅T(i)+3⋅T(j​)=4⋅1+3⋅(−2)=−2
- This is the same as:
    [1−2]⋅[43]\begin{bmatrix}1 & -2\end{bmatrix} \cdot \begin{bmatrix}4 \\ 3\end{bmatrix}[1​−2​]⋅[43​]

---

## Duality and Projections

### Duality Concept

- Any linear transformation $\vec{x} \mapsto \mathbb{R}$ corresponds to a **unique vector** $\vec{v}$ such that:
    T(x⃗)=v⃗⋅x⃗T(\vec{x}) = \vec{v} \cdot \vec{x}T(x)=v⋅x
- This is known as **duality**:
    - The **dual of a vector** is the transformation it defines
    
    - The **dual of a transformation** is the vector it corresponds to

### Projection Interpretation

- Projecting onto a **diagonal line**:
    
    - The **y-coordinate** of $\vec{u}$ gives where $\vec{j}$ lands

    - The **x-coordinate** of $\vec{u}$ gives where $\vec{i}$ lands

- A $1 \times 2$ matrix containing the coordinates of $\vec{u}$ defines the projection transformation
    
- Applying this transformation is identical to computing:
    
    u⃗⋅x⃗\vec{u} \cdot \vec{x}u⋅x
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