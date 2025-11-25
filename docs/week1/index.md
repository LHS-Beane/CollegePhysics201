# 🧭 Week 1 — Units, Dimensions, & 1D Kinematics (with Calculus)

Welcome to **Week 1** of College Physics 201!  
This module is built so you can **fully learn the content on your own**, with explanations, intuition, practice, and hidden solutions.

---

# 🎯 Learning Objectives

By the end of Week 1, you will be able to:

- Convert and analyze physical quantities using units & dimensions  
- Understand the relationship between position, velocity, and acceleration  
- Use **derivatives** to find velocity/acceleration  
- Use **integrals** to find velocity/position  
- Interpret motion graphs  
- Solve free-fall and constant-acceleration problems  
- Recognize real-world applications of calculus in motion  

---

# 📘 1. Units & Dimensions

??? info "1.1 SI Base Units (click to expand)"
    | Quantity | Unit | Symbol |
    |---------|------|--------|
    | Length | meter | m |
    | Mass | kilogram | kg |
    | Time | second | s |
    | Temperature | kelvin | K |
    | Electric current | ampere | A |

---

??? note "1.2 Dimensions (What They Mean and Why They Matter)"
    Dimensions describe **the type** of physical quantity.

    \[
    \text{Velocity}: [L][T^{-1}]
    \]

    \[
    \text{Acceleration}: [L][T^{-2}]
    \]

    \[
    \text{Force}: [M][L][T^{-2}]
    \]

    ### Why this matters  
    - If dimensions don’t match on both sides of an equation → the equation is **wrong**.  
    - This is one of the fastest ways to check your work.  
    - Physicists use this to guess formulas before deriving them.

    ### Example — Invalid Equation  
    \[
    v = 3t + 7x
    \]

    - LHS: \([L/T]\)  
    - RHS: \(3t → [T]\), \(7x → [L]\)

    ❌ You can’t add time to length, so this equation is invalid.

---

??? example "1.3 Unit Conversion (Factor-Label Method)"
    Convert 60 mph → m/s

    \[
    60 \frac{\text{mi}}{\text{hr}}
    \cdot
    \frac{1609\ \text{m}}{1\ \text{mi}}
    \cdot
    \frac{1\ \text{hr}}{3600\ \text{s}}
    =
    26.8\ \text{m/s}
    \]

---

# 📘 2. Position, Velocity, and Acceleration

\[
v(t) = \frac{dx}{dt}
\qquad
a(t) = \frac{dv}{dt}
\]

These are the **calculus definitions** of motion.

---

## 🧩 Concept → Example → Try It

=== "Concept"
    - **Position** \(x(t)\): where the object is  
    - **Velocity** \(v(t)\): how fast position changes  
    - **Acceleration** \(a(t)\): how fast velocity changes  
    - In real life, nothing moves at constant speed  
      → calculus handles changing, real-world motion

=== "Example"
    Given:
    \[
    x(t)=t^3 - 4t + 2
    \]

    \[
    v(t) = 3t^2 - 4
    \]

    \[
    a(t) = 6t
    \]

    **Interpretation:**
    - Velocity increases quadratically  
    - Acceleration increases linearly  
    - This describes an object pushed harder over time

=== "Try It"
    \[
    x(t)=5t^2 - 3t + 8
    \]

    ??? success "Show Solution"
        \[
        v(t)=10t - 3
        \]
        \[
        a(t)=10
        \]

---

??? note "Deep Explanation — Why Derivatives Describe Motion"
    Physics uses derivatives because motion is **never perfectly constant**.

    - Your position changes → velocity  
    - Your velocity changes → acceleration  
    - Your acceleration might change → jerk (used in engineering)

    **Real-world example:**  
    A car’s speedometer approximates  
    \[
    v(t)=\frac{dx}{dt}
    \]
    in real time.

---

# 📘 3. Integrals in Kinematics

Integration *rebuilds* motion from rate-of-change information.

---

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
    v(t) = 2t^2 + C
    \]

=== "Free Fall"
    \[
    a = g = 9.8\ \text{m/s}^2
    \]

    \[
    v(t)=gt + v_0
    \]

    \[
    x(t)=x_0 + v_0 t + \frac{1}{2}gt^2
    \]

---

??? note "Deep Explanation — Why Integrals Matter"
    If derivatives “zoom in,” integrals “zoom out.”

    - Integrating acceleration shows how small changes add up to velocity  
    - Integrating velocity shows how motion accumulates over time  

    **Graphically:**  
    - Area under velocity curve = displacement  
    - Area under acceleration curve = change in velocity  

---

# 📘 4. Reading Motion Graphs

??? info "Graph Interpretation (click to expand)"
    - **Slope of position graph = velocity**  
    - **Slope of velocity graph = acceleration**  
    - **Area under velocity = displacement**  
    
    Motion graphs are stories:
    - Position tells *where you are*
    - Velocity tells *how fast you move*
    - Acceleration tells *why your motion changes*

---

# 🎓 5. Worked Examples

??? example "Example 1 — From \(x(t)\) to \(v(t)\) and \(a(t)\)"
    **Given:**
    \[
    x(t)=4t^3 - 2t
    \]

    **Velocity:**
    \[
    v(t)=12t^2 - 2
    \]

    **Acceleration:**
    \[
    a(t)=24t
    \]

    **Interpretation:**
    - Velocity is quadratic → speed grows more quickly  
    - Acceleration is linear → push gets stronger over time  

---

??? example "Example 2 — Dropped Object"
    Released from height 20 m.

    \[
    v_0=0,\quad x_0=20,\quad g=9.8\ \text{m/s}^2
    \]

    **Velocity after 2 s:**
    \[
    v = gt = 19.6\ \text{m/s}
    \]

    **Position after 2 s:**
    \[
    x = 20 - \frac{1}{2}(9.8)(4) = 0.4\ \text{m}
    \]

    **Interpretation:**  
    Quadratic position function reveals *rapid acceleration* near the ground.

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

??? question "1. Given \(x(t)=2t^3 - 5t^2 + 7\), find \(v(t)\) and \(a(t)\)"
    ??? success "Show Answer"
        \[
        v(t)=6t^2 - 10t
        \]
        \[
        a(t)=12t - 10
        \]

---

??? question "2. A car accelerates from rest at 4 m/s² for 5 s"
    ??? success "Show Answer"
        \[
        x = \frac{1}{2}at^2 = 50\ \text{m}
        \]

---

??? question "3. A ball is thrown upward at 12 m/s"
    ??? success "Show Answer"
        \[
        h=\frac{v_0^2}{2g}=7.35\ \text{m}
        \]

---

??? question "4. Convert 45 mph to m/s"
    ??? success "Show Answer"
        \[
        45\ \text{mph} \approx 20.1\ \text{m/s}
        \]

---

??? question "5. If \(v(t)=6t\) and \(x(0)=0\), find \(x(t)\)"
    ??? success "Show Answer"
        \[
        x(t)=3t^2
        \]

---

# 🎉 7. Summary Sheet

\[
v=\frac{dx}{dt}
\qquad 
a=\frac{dv}{dt}
\]

\[
v=v_0+at
\qquad
x=x_0 + v_0 t + \frac{1}{2}at^2
\]

---

<div align="center">

# 🎓 Week 1 Complete!  

</div>
