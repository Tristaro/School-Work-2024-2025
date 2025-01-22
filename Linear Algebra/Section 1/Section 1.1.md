
## Section 1.1: Fields of Real Numbers (2025-01-06)
### The Real Numbers $\mathbb{R}$

- The **Real Numbers** ($\mathbb{R}$) form a _field_.
    - **Field**: A set where the usual algebraic operations (addition, subtraction, multiplication, and division) make sense.
    - **Operations**:
        - Add: $a + b$
        - Subtract: $a - b$
        - Multiply: $a \cdot b$
        - Divide: $\frac{a}{b}$ (if $b \neq 0$)

#### Field Property: Existence of Solutions

- **Fact**: For $a, b \in \mathbb{R}$, if $a \neq 0$, the equation $ax = b$ has a unique solution:
    - **Solution**: $x = \frac{b}{a}$**

---

### Vectors in the Plane $\mathbb{R}^2$

- $\mathbb{R}^2$ represents the **Cartesian Plane**, a set of ordered pairs of real numbers.
    - Points in the plane correspond to vectors in $\mathbb{R}^2$.
![[Figure 1|]]
#### Definition: Vector

A **vector** is an arrow with:

- A **tail** (initial point)
- A **head** (final point)

#### Common Representations of Vectors

- **Column Vector**: $\binom{x}{y}$
- **Row Vector**: $(x \; y)$
- **Tuple**: $(x, y)$

These represent the “head” of an arrow with the tail at the origin $\binom{0}{0}$.

---

### Examples

- Let $A = (a_x, a_y)$ and $B = (b_x, b_y)$.
- $O$ represents the **origin** $(0,0)$. 
![[Figure 2|100%x400]]
#### Standard Position of Vectors

- A vector $\vec{V}$ is in **standard position** if its tail is at the origin $O$ and the vector corresponds to a point $A \in \mathbb{R}^2$:
    - $\vec{V} = \vec{OA}$
![[Figure 3]]
#### Equivalent Vectors

- Two vectors in the plane are **equivalent** if they point in the same direction and have the same length.
    - **Fact**: Every vector in the plane is equivalent to a unique vector in standard position.

---

### Vector Addition

Let $\vec{V} = \binom{a}{b}$ and $\vec{W} = \binom{c}{d}$.

- To add vectors, add corresponding components:
    - $\vec{V} + \vec{W} = \binom{a+c}{b+d}$

#### Example:

Given points $P = (1, 1)$, $Q = (3, 2)$, and $R = (2, 3)$:

- $\vec{V} = \vec{PQ} = (3-1, 2-1) = (2, 1)$
- $\vec{W} = \vec{QR} = (2-3, 3-2) = (-1, 1)$
- $\vec{V} + \vec{W} = (2 + (-1), 1 + 1) = (1, 2)$
![[Figure 4]]
Thus, the vector $\vec{PR}$ is given by: $\vec{PR} = (2-1,3-1) - (1,2) = \vec{V} + \vec{W}$
$\therefore$ $\vec{PQ} + \vec{QR} = \vec{PR}$, which geometrically means the head of the first vector equals the tail of the second.

#### Unit Vectors in $\mathbb{R}^2$

- **Unit Vectors**:
    - $e_1 = \binom{1}{0}$
    - $e_2 = \binom{0}{1}$
![[Figure 5]]
### Properties of Vector Addition

#### Commutative Property

- Vector addition is **commutative**, meaning the order does not matter: $\vec{V} + \vec{W} = \vec{W} + \vec{V}$

#### Proofs of Commutativity:

1. **Algebraic Proof**:
    - Let $\vec{V} = \binom{a}{b}$ and $\vec{W} = \binom{c}{d}$ 
     => $a+c = c+a$ 
     => $b+d = d+b$
2. **Geometric Proof**: ![[Figure 6|]]
To Be Continued

