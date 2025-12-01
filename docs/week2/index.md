# 🧭 Week 2 — Vectors, Components & 2D Motion  
### (*Fully Illustrated, Tiered Mastery Edition*)

In Week 2, we move beyond motion in a straight line and learn how to describe motion in **two dimensions** using **vectors**.

This module is built from:
- Your extracted images from **Chapter 2 & 4**  
- OpenStax concepts (rewritten, expanded, and illustrated)  
- Tiered mastery structure for deep understanding  
- Clean, collapsible sections  
- Perfectly formatted MathJax equations

---

## 📘 1. What is a Vector?

??? info "1.1 Vector Definition (Core → Deeper → Advanced)"

    === "Core Idea"
        A **vector** has:
        - **magnitude** (how much)
        - **direction** (which way)

        Examples of vectors:
        - displacement  
        - velocity  
        - acceleration  
        - force  

        Your textbook illustration:

        ![Basic vector depiction](media/week2_images/College_Physics_-_Chapter_2_Book_p0_img0.png)

    === "Deeper Reasoning"
        A scalar (like mass or temperature) answers **“how much?”**  
        A vector answers **“how much AND in what direction?”**

        Because vectors have direction:
        - signs matter  
        - angles matter  
        - graphs matter  

        This is why student errors often come from mixing scalars and vectors.

        Another useful visual:

        ![Vector arrow concept](media/week2_images/College_Physics_-_Chapter_2_Book_p1_img0.png)

    === "Advanced Application"
        To work with vectors mathematically, we represent them in component form:

        \[
        \vec{A} = \langle A_x,\ A_y \rangle
        \]

        Or in unit vector form:

        \[
        \vec{A} = A_x \hat{i} + A_y \hat{j}
        \]

        The magnitude is:

        \[
        |\vec{A}| = \sqrt{A_x^2 + A_y^2}
        \]

        And the direction angle:

        \[
        \theta = \tan^{-1}\left(\frac{A_y}{A_x}\right)
        \]

---

## 📘 2. Breaking a Vector into Components

??? info "2.1 Components (Core → Deeper → Advanced)"

    === "Core Idea"
        Any vector can be written as **horizontal** and **vertical** parts:

        \[
        A_x = A \cos\theta, \qquad A_y = A \sin\theta
        \]

        Must-know diagram:

        ![Components diagram](media/week2_images/College_Physics_-_Chapter_2_Book_p2_img0.png)

    === "Deeper Reasoning"
        Why do we use components?

        - Because motion in the **x** direction and **y** direction are independent.
        - Gravity acts **vertically**, not horizontally.
        - Calculus works smoothly on one dimension at a time.

        Students struggle until they memorize this truth:
        > “A 2D problem is really just two 1D problems happening at the same time.”

    === "Advanced Application"
        Example:

        A \(12\ \text{m}\) vector at \(60^\circ\):

        \[
        A_x = 12\cos60^\circ = 6\ \text{m}
        \]

        \[
        A_y = 12\sin60^\circ = 10.39\ \text{m}
        \]

        This is crucial for projectile motion.

---

## 📘 3. Vector Addition & Subtraction

??? note "3.1 Adding Vectors (Core → Deeper → Advanced)"

    === "Core Idea"
        For vectors:
        \[
        \vec{A} = \langle A_x, A_y\rangle,\quad
        \vec{B} = \langle B_x, B_y\rangle
        \]

        Then:

        \[
        \vec{A} + \vec{B} = \langle A_x + B_x,\ A_y + B_y\rangle
        \]

        Illustrated:

        ![Tip to tail method](media/week2_images/College_Physics_-_Chapter_2_Book_p3_img0.png)

    === "Deeper Reasoning"
        The “tip-to-tail” method is the geometric version of vector addition.

        Vector subtraction simply flips direction:

        \[
        \vec{A} - \vec{B} = \vec{A} + (-\vec{B})
        \]

    === "Advanced Application"
        Example:

        \[
        \vec{A}=\langle 3,4\rangle,\qquad \vec{B}=\langle -2,5\rangle
        \]

        \[
        \vec{A}+\vec{B}=\langle 1,9\rangle
        \]

---

## 📘 4. Dot Product (Scalar Product)

??? info "4.1 Dot Product (Core → Deeper → Advanced)"

    === "Core Idea"
        The dot product is:

        \[
        \vec{A}\cdot\vec{B} = A_x B_x + A_y B_y
        \]

        Or:

        \[
        \vec{A}\cdot\vec{B} = |\vec{A}|\,|\vec{B}|\cos\theta
        \]

        Figure:

        ![Dot product geometry](media/week2_images/College_Physics_-_Chapter_2_Book_p6_img0.png)

    === "Deeper Reasoning"
        The dot product measures **how aligned two vectors are**.

        - Positive → similar direction  
        - Zero → perpendicular  
        - Negative → opposite directions  

        This is the basis of **work** in physics.

    === "Advanced Application"
        Angle between vectors:

        \[
        \theta = \cos^{-1} \left(\frac{\vec{A}\cdot\vec{B}}{|\vec{A}||\vec{B}|}\right)
        \]

---

## 📘 5. Motion in Two Dimensions

??? info "5.1 Independence of Motion (Core → Deeper → Advanced)"

    === "Core Idea"
        Horizontal and vertical motions are **independent** except for time.

        Gravity acts only in the **vertical** direction:

        \[
        a_x = 0,\qquad a_y = -g
        \]

        Textbook image:

        ![2D motion diagram](media/week2_images/College_Physics_-_Chapter_4_Book_p0_img0.png)

    === "Deeper Reasoning"
        Students must understand:
        - Horizontal motion is constant velocity.
        - Vertical motion is constant acceleration.

        This makes projectile motion possible.

    === "Advanced Application"
        Use components of initial velocity:

        \[
        v_{0x} = v_0\cos\theta
        \qquad
        v_{0y} = v_0\sin\theta
        \]

        Then:

        \[
        x(t)=v_{0x}t
        \]

        \[
        y(t)=y_0+v_{0y}t - \frac{1}{2}gt^2
        \]

---

## 📘 6. Projectile Motion

??? note "6.1 Full Projectile Model (Core → Deeper → Advanced)"

    === "Core Idea"
        Projectiles follow a **parabolic path**.

        Image:

        ![Projectile trajectory](media/week2_images/College_Physics_-_Chapter_4_Book_p1_img0.png)

        Horizontal motion:
        \[
        x(t)=v_{0x}t
        \]

        Vertical motion:
        \[
        y(t)=v_{0y}t - \frac{1}{2}gt^2
        \]

    === "Deeper Reasoning"
        Why parabola?

        Because:
        - Horizontal acceleration is zero
        - Vertical acceleration is constant
        - Combining them yields the parametric form of a parabola

        Eliminate \(t\):

        \[
        y = x \tan\theta - \frac{g}{2v_0^2\cos^2\theta}x^2
        \]

    === "Advanced Application"
        Flight time:

        \[
        T = \frac{2v_{0y}}{g}
        \]

        Range:

        \[
        R = \frac{v_0^2\sin2\theta}{g}
        \]

        Maximum height:

        \[
        h_{\max} = \frac{v_{0y}^2}{2g}
        \]

---

## 📘 7. Relative Velocity

??? info "7.1 Relative Motion (Core → Deeper → Advanced)"

    === "Core Idea"
        Relative velocity:

        \[
        \vec{v}_{A/B} = \vec{v}_A - \vec{v}_B
        \]

        Illustrated:

        ![Relative velocity diagram](media/week2_images/College_Physics_-_Chapter_4_Book_p5_img0.png)

    === "Deeper Reasoning"
        Relative motion answers:
        - “How fast is object A moving relative to object B?”

        This is essential for:
        - boats in rivers  
        - airplanes in wind  
        - cars on a highway  

    === "Advanced Application"
        Example: A boat moves east at 5 m/s relative to the water.  
        The water moves north at 3 m/s relative to the ground.

        \[
        \vec{v}_{B/G} = \langle 5,\ 3\rangle
        \]

        \[
        |\vec{v}| = \sqrt{5^2+3^2} = 5.83\ \text{m/s}
        \]

---

## 📘 8. Worked Examples

??? example "Example 1 — Vector Components"

    A 10 m vector at \(30^\circ\):

    \[
    A_x = 10\cos30^\circ = 8.66
    \]
    \[
    A_y = 10\sin30^\circ = 5
    \]

    ![Vector component figure](media/week2_images/College_Physics_-_Chapter_2_Book_p2_img0.png)

---

??? example "Example 2 — Projectile Motion"

    Ball launched at 20 m/s at \(40^\circ\):

    \[
    v_{0x} = 20\cos40^\circ = 15.32
    \]
    \[
    v_{0y} = 20\sin40^\circ = 12.86
    \]

    Illustrated:

    ![Projectile visual](media/week2_images/College_Physics_-_Chapter_4_Book_p1_img0.png)

---

??? example "Example 3 — Relative Velocity"

    Plane moves 80 m/s north.  
    Wind blows 30 m/s east.

    \[
    \vec{v}=\langle 30,80\rangle
    \]

    \[
    |\vec{v}| = \sqrt{30^2+80^2} = 85.4\ \text{m/s}
    \]

---

## 📘 9. Practice Problems

??? question "Try these before revealing the answers"

    **1.** Find components of a 25 m vector at \(53^\circ\).  
    **2.** A projectile is launched at 15 m/s at \(30^\circ\). Find flight time.  
    **3.** A boat moves 4 m/s east in a 3 m/s north current. Find resultant magnitude.  
    **4.** If \(\vec{A}=\langle 2,3\rangle\) and \(\vec{B}=\langle -1,4\rangle\), compute \(\vec{A}+\vec{B}\).  
    **5.** A ball is thrown horizontally at 8 m/s from 12 m high. How far does it land?

    ??? success "Solutions"
        1.  
        \[
        A_x = 25\cos53^\circ \approx 15,\ 
        A_y = 25\sin53^\circ \approx 20
        \]

        2.  
        \[
        T = \frac{2v_{0y}}{g} =
        \frac{2(15\sin30^\circ)}{9.8} = 1.53\ \text{s}
        \]

        3.  
        \[
        |\vec{v}|=\sqrt{4^2+3^2}=5\ \text{m/s}
        \]

        4.  
        \[
        \langle 2,3\rangle+\langle -1,4\rangle=\langle 1,7\rangle
        \]

        5.  
        Time:
        \[
        t = \sqrt{\frac{2h}{g}} = \sqrt{\frac{24}{9.8}} = 1.56\ \text{s}
        \]
        Distance:
        \[
        x = v t = 8(1.56)=12.5\ \text{m}
        \]

---

## 📘 10. Summary Sheet (Exam Essentials)

\[
A_x = A\cos\theta,\qquad A_y = A\sin\theta
\]

\[
x(t)=v_{0x}t
\]

\[
y(t)=y_0 + v_{0y}t - \frac{1}{2}gt^2
\]

\[
R = \frac{v_0^2\sin2\theta}{g}
\]

\[
\vec{v}_{A/B} = \vec{v}_A - \vec{v}_B
\]

---

<div align="center">


</div>
