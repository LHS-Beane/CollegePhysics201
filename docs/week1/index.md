# 🧭 Week 1 — Units, Dimensions, & 1D Kinematics (with Calculus)

Welcome to Week 1!  
This module is designed so that you can **teach yourself physics** even if you missed class — or want to build a stronger foundation for the rest of the course.

By the end of Week 1, you’ll understand:

- Units, dimensions, and physical meaning  
- Position, velocity, acceleration  
- Derivatives in motion  
- Integrals in motion  
- Free fall  
- Graph interpretation  
- Real-world problem solving  

---

# 🎯 Learning Objectives

By the end of this module, you will be able to:

- Convert units and analyze dimensions  
- Use calculus to transition between position, velocity, and acceleration  
- Interpret motion graphs  
- Solve constant and non-constant acceleration problems  
- Model real motion with integrals and derivatives  
- Apply free-fall equations correctly  

---

# 📘 1. Units, Dimensions, and Basic Concepts

## SI Base Units

| Quantity | Unit | Symbol |
|---------|------|--------|
| Length | meter | m |
| Mass | kilogram | kg |
| Time | second | s |
| Temperature | kelvin | K |
| Electric current | ampere | A |

---

## Dimensions

Dimensions express the *type* of quantity.

Examples:

\[
\text{Velocity}: [L][T^{-1}]
\]

\[
\text{Acceleration}: [L][T^{-2}]
\]

\[
\text{Force}: [M][L][T^{-2}]
\]

📌 **If dimensions don’t match on both sides of an equation, the equation is wrong.**

---

## ✨ Example: Dimensional Analysis

Is  
\[
v = 3t + 7x
\]  
valid?

- Left side: \([L/T]\)  
- Right side: \(3t \rightarrow [T]\), \(7x \rightarrow [L]\)

❌ **Invalid.** Units don’t match, so this equation cannot describe motion.

---

## 🔧 Unit Conversions (Factor-Label Method)

Example:

Convert 60 mph → m/s

\[
60\frac{\text{mi}}{\text{hr}}
\cdot
\frac{1609\ \text{m}}{1\ \text{mi}}
\cdot
\frac{1\ \text{hr}}{3600\ \text{s}}
=
26.8\ \text{m/s}
\]

Unit consistency = physics success.

---

# 📘 2. Position, Velocity, and Acceleration

## Definitions

\[
v(t) = \frac{dx}{dt}
\]

\[
a(t) = \frac{dv}{dt}
\]

These come directly from calculus.

- **Velocity** = rate of change of position  
- **Acceleration** = rate of change of velocity  

---

## 🔎 Example Function

Let:

\[
x(t) = t^3 - 4t + 2
\]

Then:

\[
v(t) = 3t^2 - 4
\]

\[
a(t) = 6t
\]

Interpretation:

- Velocity changes quadratically  
- Acceleration increases linearly → motion speeds up faster over time  

---

# 📘 3. Derivatives in Kinematics

Derivatives describe **instantaneous** rates of change.

### Example (Try This!)

\[
x(t) = 5t^2 - 3t + 8
\]

**Velocity:**

\[
v(t) = 10t - 3
\]

**Acceleration:**

\[
a(t) = 10
\]

Acceleration is constant → parabola position + linear velocity.

---

# 📘 4. Integrals in Kinematics

Integrals reconstruct motion when velocity or acceleration is known.

## If acceleration is known:

\[
v(t) = \int a(t)\, dt
\]

## If velocity is known:

\[
x(t) = \int v(t)\, dt
\]

---

## 🌟 Constant Acceleration (Very Important)

If acceleration \(a\) is constant:

\[
v(t) = v_0 + at
\]

\[
x(t) = x_0 + v_0 t + \frac{1}{2}at^2
\]

These will appear **everywhere** in physics.

---

## 🌟 Non-Constant Acceleration

Example:

\[
a(t) = 4t
\]

\[
v(t) = \int 4t\,dt = 2t^2 + C
\]

Use initial conditions to solve for \(C\).

---

# 📘 5. Free Fall

In free fall, acceleration is constant:

\[
a = g = 9.8\ \text{m/s}^2
\]

Velocity:

\[
v(t) = gt + v_0
\]

Position:

\[
x(t) = x_0 + v_0 t + \frac{1}{2}gt^2
\]

If dropped:  
\[
v_0 = 0
\]

---

# 📘 6. Graph Interpretation

Understanding graphs is one of the MOST important physics skills.

## 📈 Position → Velocity  
Velocity = slope of position graph.

## 📉 Velocity → Acceleration  
Acceleration = slope of velocity graph.

## 🧭 Velocity → Displacement  
Displacement = area under velocity graph.

---

# 🎓 7. Worked Examples

## Example 1 — Derivatives from Position

\[
x(t) = 4t^3 - 2t
\]

\[
v(t) = 12t^2 - 2
\]

\[
a(t) = 24t
\]

---

## Example 2 — Dropped Object

A ball is dropped from 20 m.

### Velocity after 2 s:

\[
v = gt = 9.8(2) = 19.6\ \text{m/s}
\]

### Position:

\[
x = 20 - \frac{1}{2}(9.8)(2^2) = 0.4\ \text{m}
\]

Just above the ground.

---

## Example 3 — Integrating Non-Constant Acceleration

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

# 📝 8. Practice Problems

Try these before checking solutions:

---

### **1.**  
\[
x(t)=2t^3 - 5t^2 + 7
\]  
Find \(v(t)\) and \(a(t)\).

---

### **2.**  
A car starts from rest and accelerates at 4 m/s² for 5 seconds.  
Find the distance traveled.

---

### **3.**  
A ball is thrown upward at 12 m/s.  
Find its max height.

---

### **4.**  
Convert 45 mph to m/s.

---

### **5.**  
If \(v(t)=6t\) and \(x(0)=0\), find \(x(t)\).

---

# 🧪 9. Mini Quiz (Check Your Understanding)

**1.** If velocity is the derivative of position, acceleration is the…  
▶ derivative of velocity  

**2.** True or False: velocity can be zero while acceleration is nonzero.  
▶ True  

**3.** A ball dropped has initial velocity…  
▶ \(0\ \text{m/s}\)  

**4.** If \(a(t)=10\), velocity is what type of function?  
▶ Linear  

---

# 🧩 10. Summary Sheet

### Must-Know Formulas

\[
v(t)=\frac{dx}{dt}
\]

\[
a(t)=\frac{dv}{dt}
\]

\[
v(t)=v_0 + at
\]

\[
x(t)=x_0 + v_0 t + \frac{1}{2}at^2
\]

### Must-Know Skills

- Read position/velocity/acceleration graphs  
- Perform derivatives & integrals in motion  
- Apply free-fall equations  
- Check dimensional consistency  
- Convert units reliably  

---

# 🎉 Excellent Work!

You’ve completed Week 1 — the foundation of all motion in physics.  
You're ready for Week 2: **Vectors, Components, and 2D Motion.**

[➡️ Continue to Week 2](../week2/index.md){ .md-button .md-button--primary }
