# Geometric Transformations

# Projective

- A projective transformation (also known as a projective mapping) is a type of transformation in geometry that maps points from one projective plane to another.
  
$$ 
 x' = H.x 
$$

$$ 
\begin{bmatrix}
x' \\ 
y'  \\ 
1 
\end{bmatrix} 
= \begin{bmatrix}
h_{11} & h_{12} & h_{13} \\ 
h_{21} & h_{22} & h_{23} \\ 
h_{31} & h_{32} & h_{33} 
\end{bmatrix}
\begin{bmatrix}
x \\ 
y  \\ 
1 
\end{bmatrix}  
$$

-Preserves: Concurrency, colinearity, order of contact (intersection, tangency, inflection, ...), cross ratio

- Subsets of projective transformations are: Affine Transformations, Similarity Transformations, Euclidean Transformation, Isometry Transformations

  
## Translation
- A translation transformation is a geometric transformation that moves every point of an object or space by the same distance in a specified direction. It is one of the simplest and most fundamental types of transformations, commonly used in computer graphics, robotics, physics, and mathematics.
- A 2D translation has 2 degrees of freedom (one for the x-direction and one for the y-direction).
- A 3D translation has 3 degrees of freedom (one for the x-direction, one for the y-direction, and one for the z-direction).
- To solve for a 2D translation, you need at least 1 point correspondence (PC).
    Why? One point gives you two equations (one for x and one for y), which is sufficient to solve for the two unknowns ($t_x$​ and $t_y$​).
- To solve for a 3D translation, you need at least 1 point correspondence.

    Why? One point gives you three equations (one for x, one for y, and one for z), which is sufficient to solve for the three unknowns ($t_x$​, $t_y$​, and $t_z$​).
  
$$ 
\begin{bmatrix}
x' \\ 
y'  \\ 
1 
\end{bmatrix} 
= \begin{bmatrix}
1 & 0 & tx \\ 
0 & 1 & ty \\ 
0 & 0 & 1 
\end{bmatrix}
\begin{bmatrix}
x \\ 
y  \\ 
1 
\end{bmatrix}  
$$

# Affine 
-An affine transformation is a geometric transformation that preserves collinearity (points lying on a straight line remain on a straight line) and ratios of distances (the midpoint of a line segment remains the midpoint after transformation). 
-  It includes translation, rotation, scaling, and shearing.
- 2D Affine Transformation:

    Linear Transformation (Rotation, Scaling): 4 DOF 

    Translation: 2 DOF (translation in x and y directions, $t_x$​ and $t_y$​).

Total DOF in 2D:
4+2=6 degrees of freedom.

- 3D Affine Transformation:

    Linear Transformation (Rotation, Scaling, Shearing): 9 DOF 

    Translation: 3 DOF (translation in x, y, and z directions, $t_x$​, $t_y$​, and $t_z$​).

Total DOF in 3D:
9+3=12 degrees of freedom.

- Number of PC: 3
- Invariants: All - (length, angle, ratio of length)
- Preserves: ratio of areas, ratio of parralel lines, parallelism
  
$$ 
\begin{bmatrix}
x' \\ 
y'  \\ 
1 
\end{bmatrix} 
= \begin{bmatrix}
a_{11} & a_{12} & tx \\ 
a_{21} & a_{22} & ty \\ 
0 & 0 & 1 
\end{bmatrix}
\begin{bmatrix}
x \\ 
y  \\ 
1 
\end{bmatrix}  
$$

# Similarity 
- A similarity transformation is a geometric transformation that preserves the shape of an object but may alter its size, orientation, and position. It combines scaling, rotation, and translation into a single transformation.
- A subset of affine transformations
- 2D Similarity Transformation:

    Scaling: 1 DOF (uniform scaling factor s).

    Rotation: 1 DOF (rotation angle θ).

    Translation: 2 DOF (translation in x and y directions, $t_x$ and $t_y$​).

Total DOF in 2D:
1+1+2=4 degrees of freedom.

- Number of PC: 2
- Invariants: All - length
- Preserves: ratio of lengths, ratio of areas, angle

  
$$ 
\begin{bmatrix}
x' \\ 
y'  \\ 
1 
\end{bmatrix} 
= \begin{bmatrix}
s\cos\theta & -s\sin\theta & tx \\ 
\sin\theta & \cos\theta & ty \\ 
0 & 0 & 1 
\end{bmatrix}
\begin{bmatrix}
x \\ 
y  \\ 
1 
\end{bmatrix}  
$$



# Isometry 
- An isometry is a geometric transformation that preserves the distances between all pairs of points. In other words, it is a distance-preserving transformation.
-  A subset of similarity transformations
- Isometry = similarity + uniform scaling
-  2D Isometry:

    Rotation: 1 DOF (rotation angle θ).

    Translation: 2 DOF (translation in x and y directions, $t_x$​ and $t_y$​).

Total DOF in 2D:
1+2=3 degrees of freedom.
- 3D Isometry:

    Rotation: 3 DOF (rotation angles around the x, y, and z axes, often represented as Euler angles or a rotation matrix).

    Translation: 3 DOF (translation in x, y, and z directions, $t_x$​, $t_y$​, and $t_z$​).

Total DOF in 3D:
3+3=6 degrees of freedom.

- Invariants: 


$$ 
\begin{bmatrix}
x' \\ 
y'  \\ 
1 
\end{bmatrix} 
= \begin{bmatrix}
\epsilon\cos\theta & -\sin\theta & tx \\ 
\epsilon\sin\theta & \cos\theta & ty \\ 
0 & 0 & 1 
\end{bmatrix}
\begin{bmatrix}
x \\ 
y  \\ 
1 
\end{bmatrix}  
$$

$$\epsilon=\mp1$$


# Euclidean 
- A Euclidean transformation is a geometric transformation that preserves the shape, size, and angles of an object. It includes rotation and translation but does not include scaling. It combines rotation, and translation into a single transformation.
- A Euclidean transformation is a type of isometry
- 2D Euclidean Transformation:

    Rotation: 1 DOF (rotation angle θ).

    Translation: 2 DOF (translation in x and y directions, $t_x$​ and $t_y$​).

Total DOF in 2D:
1+2=3 degrees of freedom.

- 3D Euclidean Transformation:

    Rotation: 3 DOF (rotation angles around the x, y, and z axes, often represented as Euler angles or a rotation matrix).

    Translation: 3 DOF (translation in x, y, and z directions, $t_x$​, $t_y$​, and $t_z$​).

Total DOF in 3D:
3+3=6 degrees of freedom.

- Number of PC: 2
- Invariants: All (length, angle, ratio of lengths, parallelism, includes cross ratio)

  
$$ 
\begin{bmatrix}
x' \\ 
y'  \\ 
1 
\end{bmatrix} 
= \begin{bmatrix}
\cos\theta & -\sin\theta & tx \\ 
\sin\theta & \cos\theta & ty \\ 
0 & 0 & 1 
\end{bmatrix}
\begin{bmatrix}
x \\ 
y  \\ 
1 
\end{bmatrix}  
$$

