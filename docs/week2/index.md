# 🧭 Week 2 — Vectors & 2D Motion  
### *(Fully Illustrated — Tiered Mastery Edition)*

This module teaches you everything you need about **vectors**, **components**, **2D motion**, **projectiles**, and **relative velocity** — even if you missed class.  
Every section includes:

- **Core Idea** (must-know)
- **Deeper Reasoning** (why it works)
- **Advanced Application** (real physics + calculus)
- **Illustrations** from your textbook
- **Concept Checks**
- **Examples & Practice**

---

# ⭐ 0. HOW TO USE THIS MODULE
??? note "Click to expand"

    ### What this module gives you:
    - Complete lesson on Vectors + 2D Motion  
    - Diagrams from your uploaded Chapters 2 and 4  
    - Beginner-friendly explanations  
    - Practice with hidden answers  
    - Scaffolding from intuition → mastery  

    ### How to learn efficiently:
    - Expand each collapsible section  
    - Do concept checks BEFORE revealing solutions  
    - Work practice problems on paper first  
    - Review the summary sheet before the quiz  

---

# ⭐ 1. WHAT IS A VECTOR?

??? info "1.1 Understanding Vectors (Core → Deeper → Advanced)"

    === "Core Idea"
    A **vector** has both:
    - **magnitude** (how much)
    - **direction** (which way)

    Common vectors:
    - displacement  
    - velocity  
    - acceleration  
    - force  

    ![Vector arrow](media/week2_images/College_Physics_-_Chapter_2_Book_p0_img0.png)

    === "Deeper Reasoning"
    Scalars answer *“how much?”*.  
    Vectors answer *“how much + which direction?”* — direction changes physics.

    A 10 N push north ≠ a 10 N push east.

    === "Advanced Application"
    Component form:

    \[
    \vec{A} = \langle A_x, A_y \rangle
    \]

    Unit vector form:

    \[
    \vec{A} = A_x\hat{i} + A_y\hat{j}
    \]

    Magnitude:

    \[
    |\vec{A}|=\sqrt{A_x^2 + A_y^2}
    \]

    Direction:

    \[
    \theta = \tan^{-1}\left(\frac{A_y}{A_x}\right)
    \]

---

# ⭐ 2. WHY VECTOR COMPONENTS MATTER

??? example "2.1 Components (Core → Deeper → Advanced)"

    === "Core Idea"
    Any vector can be broken into **horizontal** and **vertical** parts:

    \[
    A_x = A\cos\theta,\qquad A_y = A\sin\theta
    \]

    ![Components diagram](media/week2_images/College_Physics_-_Chapter_2_Book_p2_img0.png)

    === "Deeper Reasoning"
    The key idea:

    > **A 2D motion problem is really just two separate 1D problems happening at the same time.**

    - Gravity affects **only vertical** motion  
    - Horizontal motion is independent  
    - Calculus and kinematics become easy in components  

    === "Advanced Application"
    Example:

    A \(12\text{ m}\) vector at \(60^\circ\):

    \[
    A_x=12\cos60^\circ=6
    \]

    \[
    A_y=12\sin60^\circ=10.39
    \]

---

# ⭐ 3. VECTOR ADDITION & SUBTRACTION

??? info "3.1 Adding and Subtracting Vectors"

    === "Core Idea"
    Add vectors **component-wise**:

    \[
    \vec{A}+\vec{B}=\langle A_x+B_x,\ A_y+B_y\rangle
    \]

    Geometric version (tip-to-tail):

    ![Tip to tail](media/week2_images/College_Physics_-_Chapter_2_Book_p3_img0.png)

    === "Deeper Reasoning"
    The geometric and algebraic methods give identical results.

    Subtraction:

    \[
    \vec{A}-\vec{B}=\vec{A}+(-\vec{B})
    \]

    === "Advanced Application"
    Example:

    \[
    \vec{A}=\langle 3,4\rangle,\quad \vec{B}=\langle -2,5\rangle
    \]

    \[
    \vec{A}+\vec{B}=\langle 1,9\rangle
    \]

---

# ⭐ 4. DOT PRODUCT (MEASURES ALIGNMENT)

??? note "4.1 Dot Product (Core → Deeper → Advanced)"

    === "Core Idea"
    Component definition:

    \[
    \vec{A}\cdot\vec{B}=A_xB_x + A_yB_y
    \]

    Geometric definition:

    \[
    \vec{A}\cdot\vec{B}=|\vec{A}||\vec{B}|\cos\theta
    \]

    ![Dot product](media/week2_images/College_Physics_-_Chapter_2_Book_p6_img0.png)

    === "Deeper Reasoning"
    Dot product tells you *how aligned two vectors are*:

    - positive → same direction  
    - zero → perpendicular  
    - negative → opposite  

    === "Advanced Application"
    Angle between vectors:

    \[
    \theta = \cos^{-1}\left(\frac{\vec{A}\cdot\vec{B}}{|\vec{A}||\vec{B}|}\right)
    \]

---

# ⭐ 5. MOTION IN TWO DIMENSIONS

??? info "5.1 Independence of x- and y-motion"

    === "Core Idea"
    Key principle:

    - Horizontal and vertical motions are **independent**  
    - Time links them  
    - Gravity affects only vertical direction  

    ![2D motion](media/week2_images/College_Physics_-_Chapter_4_Book_p0_img0.png)

    \[
    a_x=0,\qquad a_y=-g
    \]

    === "Deeper Reasoning"
    Physics becomes simple when you realize:

    - The **x-motion** behaves like constant velocity  
    - The **y-motion** behaves like free fall  
    - Combine the motions → you get a **parabola**

    === "Advanced Application"
    Break initial velocity into components:

    \[
    v_{0x}=v_0\cos\theta
    \]

    \[
    v_{0y}=v_0\sin\theta
    \]

---

# ⭐ 6. PROJECTILE MOTION

??? example "6.1 Full Projectile Motion Model"

    === "Core Idea"
    Horizontal motion:

    \[
    x(t)=v_{0x}t
    \]

    Vertical motion:

    \[
    y(t)=y_0 + v_{0y}t - \frac{1}{2}gt^2
    \]

    ![Projectile](media/week2_images/College_Physics_-_Chapter_4_Book_p1_img0.png)

    === "Deeper Reasoning"
    The path is a **parabola** because:

    - Horizontal: constant velocity  
    - Vertical: constant acceleration  

    Eliminating \(t\) gives:

    \[
    y = x \tan\theta - \frac{g}{2v_0^2\cos^2\theta}\,x^2
    \]

    === "Advanced Application"
    Time of flight:

    \[
    T=\frac{2v_{0y}}{g}
    \]

    Range:

    \[
    R = \frac{v_0^2\sin(2\theta)}{g}
    \]

    Maximum height:

    \[
    h_{\max} = \frac{v_{0y}^2}{2g}
    \]

---

# ⭐ 7. RELATIVE VELOCITY

??? info "7.1 Motion from Different Reference Frames"

    === "Core Idea"
    Relative velocity formula:

    \[
    \vec{v}_{A/B}=\vec{v}_A - \vec{v}_B
    \]

    ![Relative motion](media/week2_images/College_Physics_-_Chapter_4_Book_p5_img0.png)

    === "Deeper Reasoning"
    Situations using relative velocity:

    - boats in current  
    - planes in wind  
    - cars passing  
    - walking on a moving walkway  

    === "Advanced Application"
    Example:

    Plane: \(80\text{ m/s}\) north  
    Wind: \(30\text{ m/s}\) east  

    \[
    \vec{v}=\langle 30,\ 80\rangle
    \]

    \[
    |\vec{v}|=\sqrt{30^2+80^2}=85.4\text{ m/s}
    \]

---

# ⭐ 8. WORKED EXAMPLES

??? example "Example 1 — Vector Components"

    10 m vector at 30°:

    \[
    A_x=10\cos30^\circ=8.66
    \]

    \[
    A_y=10\sin30^\circ=5
    \]

    ![components](media/week2_images/College_Physics_-_Chapter_2_Book_p2_img0.png)

---

??? example "Example 2 — Projectile Launched at Angle"

    Launch at 20 m/s, 40°:

    \[
    v_{0x} = 20\cos40^\circ
    \]

    \[
    v_{0y} = 20\sin40^\circ
    \]

    ![projectile](media/week2_images/College_Physics_-_Chapter_4_Book_p1_img0.png)

---

??? example "Example 3 — Relative Velocity"

    Car A: 30 m/s east  
    Car B: 20 m/s west  

    \[
    \vec{v}_{A/B}=\langle30,0\rangle - \langle -20,0\rangle
    \]

    \[
    \vec{v}_{A/B}=\langle50,0\rangle
    \]

---

# ⭐ 9. PRACTICE PROBLEMS

??? question "Try these before revealing answers"

    **1.** Components of a 25 m vector at 53°.  
    **2.** Launch at 15 m/s, 30°. Find flight time.  
    **3.** Boat east 4 m/s, current north 3 m/s. Resultant speed?  
    **4.** \(\vec{A}=\langle2,3\rangle\), \(\vec{B}=\langle-1,4\rangle\). Find \(\vec{A}+\vec{B}\).  
    **5.** Ball thrown horizontally at 8 m/s from 12 m high. Range?

    ??? success "Solutions"
        1.  
        \[
        A_x=25\cos53^\circ\approx15
        \]
        \[
        A_y=25\sin53^\circ\approx20
        \]

        2.  
        \[
        T=\frac{2v_{0y}}{g}=\frac{2(15\sin30^\circ)}{9.8}=1.53\text{ s}
        \]

        3.  
        \[
        |\vec{v}|=\sqrt{4^2+3^2}=5\text{ m/s}
        \]

        4.  
        \[
        \langle2,3\rangle+\langle-1,4\rangle=\langle1,7\rangle
        \]

        5.  
        \[
        t=\sqrt{\frac{2h}{g}}=\sqrt{\frac{24}{9.8}}=1.56\text{ s}
        \]
        \[
        x=vt=8(1.56)=12.5\text{ m}
        \]

---

# ⭐ 10. SUMMARY SHEET (Exam Essentials)

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
R=\frac{v_0^2\sin2\theta}{g}
\]

\[
\vec{v}_{A/B}=\vec{v}_A - \vec{v}_B
\]

---

<div align="center">

</div>
