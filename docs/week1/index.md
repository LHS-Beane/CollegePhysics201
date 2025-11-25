# 🧭 Week 1 — Units, Dimensions, & 1D Kinematics (with Calculus)

Welcome to Week 1! This module teaches the foundations of motion using both **physics** and **calculus**.  
Click sections to expand — you don’t need to scroll everything at once.

---

# 🎯 Learning Objectives

- Convert units and analyze dimensions  
- Use derivatives and integrals to describe motion  
- Interpret motion graphs  
- Solve constant- and non-constant-acceleration problems  
- Apply free-fall equations  

---

# 📘 1. Units, Dimensions, and Analysis

??? info "1.1 SI Base Units (click to expand)"
    | Quantity | Unit | Symbol |
    |---------|------|--------|
    | Length | meter | m |
    | Mass | kilogram | kg |
    | Time | second | s |
    | Temperature | kelvin | K |
    | Electric current | ampere | A |

---

??? note "1.2 Dimensions (click to expand)"
    Dimensions describe the *type* of quantity.

    \[
    \text{Velocity}: [L][T^{-1}]
    \]

    \[
    \text{Acceleration}: [L][T^{-2}]
    \]

    **Invalid equation example:**  
    \[
    v = 3t + 7x \quad \text{(units don’t match)}
    \]

---

??? example "1.3 Unit Conversion Example (click)"
    Convert 60 mph → m/s:

    \[
    60 \frac{\text{mi}}{\text{hr}}
    \cdot
    \frac{1609\ \text{m}}{1\ \text{mi}}
    \cdot
    \frac{1\ \text{hr}}{3600\ \text{s}}
    = 26.8\ \text{m/s}
    \]

---

# 📘 2. Position, Velocity, and Acceleration

We use:

\[
v(t)=\frac{dx}{dt} \qquad a(t)=\frac{dv}{dt}
\]

---

## 🧩 Concept → Example → Try It

=== "Concept"
    Position \(x(t)\), velocity \(v(t)\), and acceleration \(a(t)\) are linked through calculus.

=== "Example"
    Given:
    \[
    x(t) = t^3 - 4t + 2
    \]

    \[
    v(t) = 3t^2 - 4
    \]

    \[
    a(t) = 6t
    \]

=== "Try It"
    Find \(v(t)\) and \(a(t)\) if:
    \[
    x(t)=5t^2 - 3t + 8
    \]

    ??? success "Show Solution"
        \[
        v(t)=10t-3
        \]
        \[
        a(t)=10
        \]

---

# 📘 3. Integrals in Kinematics

=== "Constant Acceleration"
    \[
    v(t)=v_0 + at
    \]
    \[
    x(t)=x_0 + v_0 t + \frac{1}{2}at^2
    \]

=== "Non-Constant Acceleration"
    Example:
    \[
    a(t)=4t
    \]
    \[
    v(t)=2t^2 + C
    \]

=== "Free Fall"
    \[
    a=g=9.8\ \text{m/s}^2
    \]
    \[
    v(t)=gt + v_0
    \]
    \[
    x(t)=x_0 + v_0 t + \frac{1}{2}gt^2
    \]

---

# 📘 4. Graph Interpretation  
Graphs are essential.

??? info "How to read motion graphs (click to expand)"
    - Position slope → velocity  
    - Velocity slope → acceleration  
    - Area under velocity curve → displacement  

---

# 🎓 5. Worked Examples

??? example "Example 1 — From x(t) to v(t) and a(t)"
    \[
    x(t)=4t^3 - 2t
    \]
    \[
    v(t)=12t^2 - 2
    \]
    \[
    a(t)=24t
    \]

---

??? example "Example 2 — Dropped Object"
    A ball is dropped from height 20 m.

    **Velocity after 2 s:**
    \[
    v=gt=9.8(2)=19.6\ \text{m/s}
    \]

    **Position:**
    \[
    x=20 - \frac{1}{2}(9.8)(2^2)=0.4\ \text{m}
    \]

---

??? example "Example 3 — Integrating Non-Constant Acceleration"
    \[
    a(t)=6t,\quad v(0)=3
    \]

    \[
    v(t)=3t^2 + 3
    \]

    \[
    x(t)=t^3 + 3t
    \]

---

# 📝 6. Practice Problems

??? question "Practice Problem 1"
    Given:
    \[
    x(t)=2t^3 - 5t^2 + 7
    \]
    Find \(v(t)\) and \(a(t)\).

    ??? success "Show Answer"
        \[
        v(t)=6t^2 - 10t
        \]
        \[
        a(t)=12t - 10
        \]

---

??? question "Practice Problem 2"
    A car starts from rest and accelerates at 4 m/s² for 5 seconds.
    
    ??? success "Show Answer"
        \[
        x=\frac{1}{2}at^2 = \frac{1}{2}(4)(25)=50\ \text{m}
        \]

---

??? question "Practice Problem 3"
    A ball is thrown upward at 12 m/s. Find its max height.
    
    ??? success "Show Answer"
        \[
        h=\frac{v_0^2}{2g}=\frac{144}{19.6}=7.35\ \text{m}
        \]

---

??? question "Practice Problem 4"
    Convert 45 mph to m/s.

    ??? success "Show Answer"
        \[
        45\ \text{mph}=20.1\ \text{m/s}
        \]

---

??? question "Practice Problem 5"
    If \(v(t)=6t\) and \(x(0)=0\), find \(x(t)\).

    ??? success "Show Answer"
        \[
        x(t)=3t^2
        \]

---

# 🎉 7. Summary Sheet

\[
v=\frac{dx}{dt} \qquad a=\frac{dv}{dt}
\]

\[
v=v_0+at \qquad x=x_0 + v_0t + \frac{1}{2}at^2
\]

---

<div align="center">

# 🎓 Week 1 Complete!  
[Continue to Week 2 →](../week2/index.md){ .md-button .md-button--primary }

</div>

