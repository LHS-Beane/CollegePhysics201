# 🧭 Week 2 — Vectors, Components, and 2D Motion

Welcome to **Week 2**!  
This module teaches how to represent quantities in two dimensions — a critical step for real physics.

You’ll learn vectors, components, projectiles, and how calculus applies in 2D motion.

Click on sections to expand and learn at your own pace.

---

# 🎯 Learning Objectives

By the end of Week 2, you will be able to:

- Represent physical quantities as **vectors**  
- Break vectors into **x and y components**  
- Use **unit vectors**  
- Add, subtract, and scale vectors  
- Compute dot products  
- Analyze **2D motion** using components  
- Solve **projectile motion** problems  
- Use reasoning + calculus to understand curved motion  

---

# 📘 1. Introduction to Vectors

??? info "1.1 What is a Vector?"
    A **vector** has both:

    - **magnitude** (how much)
    - **direction** (which way)

    Examples:
    - velocity  
    - acceleration  
    - displacement  
    - force  

    Scalar ≠ vector  
    - a scalar has magnitude only  
    - example: mass, temperature, energy

---

??? note "1.2 Vector Notation"
    Common notations:

    \[
    \vec{A},\quad \mathbf{A},\quad \langle A_x, A_y \rangle
    \]

    Components:
    \[
    \vec{A} = \langle A_x,\ A_y \rangle
    \]

    Magnitude:
    \[
    |\vec{A}| = \sqrt{A_x^2 + A_y^2}
    \]

    Unit vector form:
    \[
    \vec{A} = A_x \hat{i} + A_y \hat{j}
    \]

---

??? note "Deep Explanation — Why Physics Uses Components"
    Real-world motion rarely happens in a straight line.

    By breaking motion into:
    \[
    x\text{-direction} \quad \text{and} \quad y\text{-direction}
    \]
    we can:

    - treat each dimension independently  
    - solve harder problems using simple 1D equations  
    - combine them at the end to get full motion  

    Example:  
    Projectile motion has:
    - horizontal motion with **constant velocity**  
    - vertical motion with **constant acceleration**  

    Components allow us to separate these behaviors cleanly.

---

# 📘 2. Vector Components

=== "Concept"
    Any vector can be broken into x and y components:

    \[
    A_x = A\cos\theta,\qquad A_y = A\sin\theta
    \]

    This allows you to treat motion separately in each direction.

=== "Example"
    A 10 m vector at 30° above horizontal:

    \[
    A_x = 10\cos 30^\circ = 8.66
    \]
    \[
    A_y = 10\sin 30^\circ = 5
    \]

=== "Try It"
    A 12 m vector at 60°:

    ??? success "Show Solution"
        \[
        A_x = 12\cos 60^\circ = 6
        \]
        \[
        A_y = 12\sin 60^\circ = 10.39
        \]

---

# 📘 3. Vector Addition & Subtraction

??? example "Click to expand"
    For vectors:
    \[
    \vec{A} = \langle A_x, A_y \rangle,\quad
    \vec{B} = \langle B_x, B_y \rangle
    \]

    Addition:
    \[
    \vec{A} + \vec{B} = \langle A_x + B_x,\ A_y + B_y \rangle
    \]

    Subtraction:
    \[
    \vec{A} - \vec{B} = \langle A_x - B_x,\ A_y - B_y \rangle
    \]

    Geometric interpretation:  
    - Tip-to-tail method  
    - Parallelogram rule  

---

# 📘 4. Dot Product (Optional but powerful)

??? info "Understanding the Dot Product (Why it matters)"
    Definition:

    \[
    \vec{A}\cdot\vec{B} = A_x B_x + A_y B_y
    \]

    Geometric form:

    \[
    \vec{A}\cdot\vec{B} = |\vec{A}|\,|\vec{B}|\cos\theta
    \]

    Meaning:
    - Measures how much two vectors “point in the same direction”  
    - Used heavily in energy & work (Week 4)  
    - Helps find angles between vectors  

---

# 📘 5. 2D Kinematics Overview

Motion in 2 dimensions is broken into two **independent** motions:

- Horizontal (x): constant velocity  
- Vertical (y): constant acceleration  

\[
x(t)=v_{0x}t,
\qquad
y(t)=y_0 + v_{0y} t + \frac{1}{2}(-g)t^2
\]

Acceleration only affects the **vertical** motion.

---

??? note "Deep Explanation — Why x and y Motion Are Independent"
    Gravity only pulls downward.

    That means:
    - it changes **vertical** motion  
    - it does NOT affect horizontal motion  

    This is why a bullet dropped and a bullet fired horizontally  
    hit the ground at **the same time**.

---

# 📘 6. Projectile Motion

=== "Concept"
    A projectile has:
    - horizontal motion with constant velocity  
    \[
    x(t)=v_{0x} t
    \]
    - vertical motion with constant acceleration  
    \[
    y(t)=y_0 + v_{0y} t - \frac{1}{2}gt^{2}
    \]

=== "Example"
    A ball is launched at \(20\ \text{m/s}\) at 40°.

    Components:
    \[
    v_{0x} = 20\cos 40^\circ = 15.32
    \]
    \[
    v_{0y} = 20\sin 40^\circ = 12.86
    \]

=== "Try It"
    Launch speed \(15\ \text{m/s}\) at 30°.

    ??? success "Show Solution"
        \[
        v_{0x} = 15\cos 30^\circ = 12.99
        \]
        \[
        v_{0y} = 15\sin 30^\circ = 7.5
        \]

---

# 🎓 7. Worked Examples

??? example "Example 1 — Range of a Projectile"
    A ball is launched at \(25\ \text{m/s}\) at 35° from ground level.

    Components:
    \[
    v_{0x} = 25\cos 35^\circ = 20.48
    \]
    \[
    v_{0y} = 25\sin 35^\circ = 14.34
    \]

    Time of flight:
    \[
    t = \frac{2v_{0y}}{g} = 2.93\ \text{s}
    \]

    Range:
    \[
    R=v_{0x}t = 59.97\ \text{m}
    \]

---

??? example "Example 2 — Maximum Height"
    Using:
    \[
    v_y^2 = v_{0y}^2 - 2g(y - y_0)
    \]

    Max height occurs when:
    \[
    v_y = 0
    \]

    Solve:
    \[
    h = \frac{v_{0y}^2}{2g}
    \]

---

??? example "Example 3 — Relative Velocity"
    A boat moves 5 m/s east in a river flowing 3 m/s north.

    \[
    \vec{v} = \langle 5,\ 3 \rangle
    \]

    Magnitude:
    \[
    |\vec{v}| = \sqrt{5^2 + 3^2} = 5.83\ \text{m/s}
    \]

---

# 📝 8. Practice Problems

??? question "1. A 12 m vector is at 25° above horizontal. Find components."
    ??? success "Show Answer"
        \[
        A_x = 12\cos 25^\circ = 10.88
        \]
        \[
        A_y = 12\sin 25^\circ = 5.07
        \]

---

??? question "2. A projectile is launched at 18 m/s at 45°."
    Find its horizontal and vertical components.

    ??? success "Show Answer"
        \[
        v_{0x} = 18\cos 45^\circ = 12.73
        \]
        \[
        v_{0y} = 18\sin 45^\circ = 12.73
        \]

---

??? question "3. Find the range of a projectile launched at 20 m/s at 30°."
    ??? success "Show Answer"
        \[
        v_{0x}=17.32,\quad v_{0y}=10
        \]
        \[
        t = \frac{2v_{0y}}{g} = 2.04\ \text{s}
        \]
        \[
        R = v_{0x} t = 35.3\ \text{m}
        \]

---

??? question "4. A ball is thrown horizontally at 8 m/s from 10 m height."
    ??? success "Show Answer"
        Time to fall:
        \[
        t = \sqrt{\frac{2h}{g}} = 1.43\ \text{s}
        \]

        Horizontal distance:
        \[
        x = v_x t = 11.4\ \text{m}
        \]

---

??? question "5. A boat moves 4 m/s east in a 3 m/s north current."
    ??? success "Show Answer"
        \[
        \vec{v}=\langle 4,\ 3 \rangle
        \]
        \[
        |\vec{v}| = 5\ \text{m/s}
        \]

---

# 🎉 9. Summary Sheet

\[
A_x = A\cos\theta,\quad A_y = A\sin\theta
\]

\[
x(t)=v_{0x}t
\]

\[
y(t)=y_0 + v_{0y}t - \frac{1}{2}gt^2
\]

\[
|\vec{A}|=\sqrt{A_x^2 + A_y^2}
\]

---

<div align="center">

# 🎓 Week 2 Complete!  

</div>

