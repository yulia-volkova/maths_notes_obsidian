# The Determinant & Three dimensional linear transformations

chttps://youtu.be/Ip3X9LOh2dk?si=vjdTsEfEBzvECI7w)

[Three dim linear transformations link ](https://youtu.be/rHLEWRxRGiM?si=sne5ILBtV2jlcF2h)

- **Coordinates as Instructions:**  
    Each coordinate tells you how much to scale each basis vector so that, when added together, they form a new vector.

- **3D Matrix Multiplication:**  
    Essential in robotics and computer graphics. It allows complex rotations to be broken down into a composition of simpler transformations.

- **Determinant of a Transformation:**  
    A determinant is a special scaling factor. It tells how a linear transformation changes area (in 2D) or volume (in 3D).

    - **Determinant = 0:**  
        Indicates that the transformation collapses the space onto a lower dimension — such as a line, plane, or point. This means the matrix’s columns are linearly dependent.
        
    - **Negative Determinant:**  
        Means the transformation flips the orientation of the space.
        
- **Determinants in 3D:**  
    We need to think about a unit cube (1×1×1) whose edges are resting on the basis vectors.
    
    - A non-zero determinant scales the volume of that cube.
    
    - A zero determinant means the volume is flattened to zero — a degenerate transformation.
    
    - A negative determinant means that, along with the volume scaling, the space’s orientation is flipped.

- **2×2 Determinant Formula:**

$$
\text{det} = ad - bc
$$

- $a$ tells us how much $\hat{i}$ is stretched in the x-direction.
- $d$ tells us how much $\hat{j}$ is stretched in the y-direction.
- So, $a \times d$ tells the area of the rectangle that the unit square turns into.
- If one of b or c are zero you get parallelogram with base a and height d  
- If both bc are not zero it tells how much parallelogram is stretched or squished in the diagonal direction

- **Consistency Across the Grid:**  
    Whatever transformation happens to one unit square must happen to every square on the grid, regardless of its size.  
    This is because grid lines are parallel and evenly spaced — a core principle of linear transformations.
