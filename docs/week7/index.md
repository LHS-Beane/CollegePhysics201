# 📘 Week 7 — Rotational Motion  
*College Physics 201 — Calculus-Based Physics*

Rotational motion extends all the concepts studied so far — displacement, velocity, acceleration, Newton’s laws, energy, momentum — into circular and rigid-body motion.  
This is one of the most powerful and mathematically rich topics in physics.

Use these collapsible sections to explore each idea:

---

# 🔵 Rotational Kinematics

???+ example "Rotational Kinematics"
    ## ⭐ Core Idea
    Rotational motion uses three primary angular variables:

    $$
    \theta,\qquad \omega = \frac{d\theta}{dt},\qquad \alpha = \frac{d\omega}{dt}
    $$

    - **θ** — angular position (radians)  
    - **ω** — angular velocity  
    - **α** — angular acceleration  

    Radians are dimensionless, making calculus and physical relations clean.

    ![intro](media/week7_images/College_Physics_-_Chapter_10_Book_p0_img0.png)

    ---

    ## 🌟 Deeper Reasoning
    Hewitt notes that rotational motion is simply *"motion that turns about an axis."*

    As an object rotates through an angle θ, a point at radius r moves through arc length:

    $$
    s = r\theta
    $$

    This leads directly to the linear ↔ rotational relationships:

    $$
    v = r\omega
    $$
    $$
    a_t = r\alpha
    $$
    $$
    a_c = \omega^2 r
    $$

    - **Tangential acceleration** changes speed.  
    - **Centripetal acceleration** changes direction.

    ![circular](media/week7_images/College_Physics_-_Chapter_10_Book_p13_img0.png)

    ---

    ## 🎓 Advanced Concept
    Rotational kinematics parallels linear kinematics exactly:

    | Linear | Rotational |
    |--------|------------|
    | \(x\) | \(\theta\) |
    | \(v=\frac{dx}{dt}\) | \(\omega=\frac{d\theta}{dt}\) |
    | \(a=\frac{dv}{dt}\) | \(\alpha=\frac{d\omega}{dt}\) |

    This analogy is the foundation of rotational dynamics and energy.

    ---

    ### 🔶 *Worked Example: Finding Angular Velocity*
    ???+ example "Worked Example: Constant Angular Acceleration"
        A wheel starts from rest and accelerates at \( \alpha = 3 \text{ rad/s}^2 \).  
        Find \( \omega \) after 4 seconds.

        **Step 1 — Use definition**  
        $$
        \omega = \omega_0 + \alpha t
        $$

        **Step 2 — Plug values**  
        $$
        \omega = 0 + (3)(4) = 12 \text{ rad/s}
        $$

        **Answer:**  
        \(\omega = 12 \text{ rad/s}\)

---

# 🔵 Torque

???+ example "Torque"
    ## ⭐ Core Idea
    Torque measures how effectively a force causes rotation:

    $$
    \tau = rF\sin\theta
    $$

    ![torque](media/week7_images/College_Physics_-_Chapter_10_Book_p5_img0.png)

    ---

    ## 🌟 Deeper Reasoning
    Torque depends on:
    - force magnitude  
    - lever arm length  
    - angle of application  

    Hewitt: *"Only the perpendicular part of the force twists the object."*

    Direction is given by the **right-hand rule**:

    ![rhr](media/week7_images/College_Physics_-_Chapter_11_Book_p3_img0.png)

    ---

    ## 🎓 Advanced Concept
    Key definitions:
    - **Lever arm (r):** distance from pivot to force line  
    - **Effective force:** \(F_\perp = F\sin\theta\)  
    - **Net torque:** sum of all clockwise (−) and counterclockwise (+) torques  

    ---

    ### 🔶 *Worked Example: Torque at an Angle*
    ???+ example "Worked Example: Single Torque"
        A 0.40 m bar experiences a 15 N force at \(60^\circ\).

        **Compute torque:**
        $$
        \tau = rF\sin\theta = (0.40)(15)\sin 60^\circ
        $$

        $$
        \tau = 6 \times 0.866 = 5.20 \text{ N·m}
        $$

        **Answer:**  
        \( \tau = 5.2\text{ N·m} \)

    ### 🔶 *Worked Example: Competing Torques*
    ???+ example "Worked Example: Net Torque"
        A bar has two forces:
        - 20 N at 0.30 m (CCW)
        - 15 N at 0.50 m (CW)

        $$
        \tau_{CCW} = (0.30)(20) = 6.0
        $$
        $$
        \tau_{CW} = (0.50)(15) = 7.5
        $$

        $$
        \tau_{net} = 6.0 - 7.5 = -1.5 \text{ N·m}
        $$

        **Clockwise rotation.**

---

# 🔵 Moment of Inertia

???+ example "Moment of Inertia"
    ## ⭐ Core Idea
    Moment of inertia is rotational mass:

    $$
    I = \sum m r^2
    $$

    ![inertia](media/week7_images/College_Physics_-_Chapter_11_Book_p10_img0.png)

    ---

    ## 🌟 Deeper Reasoning
    Knight emphasizes:  
    *"An object's resistance to rotation depends WHERE its mass is located."*

    | Object | Moment of Inertia |
    |--------|------------------|
    | Solid disk | \( \frac12 MR^2 \) |
    | Hoop | \( MR^2 \) |
    | Rod (center) | \( \frac{1}{12} ML^2 \) |
    | Rod (end) | \( \frac{1}{3} ML^2 \) |

    ![table](media/week7_images/College_Physics_-_Chapter_10_Book_p22_img0.png)

    ---

    ## 🎓 Advanced Concept
    **Parallel-Axis Theorem:**

    $$
    I = I_{cm} + Md^2
    $$

    Used when rotating about any axis NOT through the center.

    ![pat](media/week7_images/College_Physics_-_Chapter_11_Book_p30_img0.png)

    ---

    ### 🔶 *Worked Example: Using Parallel-Axis*
    ???+ example "Worked Example: Rod About One End"
        A rod of mass 2.0 kg and length 1.0 m rotates about one end.

        **Center moment:**
        $$
        I_{cm} = \frac{1}{12}ML^2 = \frac{1}{12}(2)(1)^2 = 0.167
        $$

        **Shift to end:**
        $$
        I = I_{cm} + Md^2 = 0.167 + 2(0.5)^2
        $$

        $$
        I = 0.167 + 0.5 = 0.667 \text{ kg·m}^2
        $$

---

# 🔵 Rotational Dynamics (τ = Iα)

???+ example "Rotational Dynamics"
    ## ⭐ Core Idea
    $$
    \tau_{net} = I\alpha
    $$

    The rotational form of Newton’s 2nd Law.

    ---

    ## 🌟 Deeper Reasoning
    - Larger torque → larger α  
    - Larger inertia → smaller α  
    - Direction of α determined by direction of τ  

    ![dyn](media/week7_images/College_Physics_-_Chapter_11_Book_p36_img0.png)

    ---

    ## 🎓 Advanced Concept
    Pulley systems combine:
    - translation of masses  
    - rotation of pulleys  

    ![pulley](media/week7_images/College_Physics_-_Chapter_10_Book_p18_img0.png)

    ---

    ### 🔶 *Worked Example: Rotating Disk*
    ???+ example "Worked Example: Tangential Force"
        Disk: \(m=2.0\text{ kg}, r=0.20\text{ m}\)  
        Tangential force: \(10\text{ N}\)

        **Torque:**
        $$
        \tau = rF = 2.0 \text{ N·m}
        $$

        **Inertia:**
        $$
        I = \frac12 mr^2 = 0.04
        $$

        **Acceleration:**
        $$
        \alpha = \frac{\tau}{I} = 50
        $$

---

# 🔵 Rolling Without Slipping

???+ example "Rolling Without Slipping"
    ## ⭐ Core Idea
    Condition:

    $$
    v = r\omega
    $$

    ![rolling](media/week7_images/College_Physics_-_Chapter_10_Book_p21_img0.png)

    ---

    ## 🌟 Deeper Reasoning
    Hewitt:  
    *"Rolling is walking forward while spinning around."*

    The bottom point is instantaneously at rest.

    Static friction provides the link — but **does no work**.

    ---

    ## 🎓 Advanced Concept
    - Bottom moves at 0  
    - Center moves at v  
    - Top moves at 2v  

---

# 🔵 Rotational Energy

???+ example "Rotational Energy"
    ## ⭐ Core Idea
    Total kinetic energy:

    $$
    K = \frac12 mv^2 + \frac12 I\omega^2
    $$

    ---

    ## 🌟 Deeper Reasoning
    A hoop accelerates slower than a disk.  
    A sphere accelerates faster than both.

    Because I determines how KE is split.

    ---

    ## 🎓 Advanced Concept
    ![energy](media/week7_images/College_Physics_-_Chapter_10_Book_p27_img1.png)

---

# 🔵 Angular Momentum

???+ example "Angular Momentum"
    ## ⭐ Core Idea
    $$
    L = I\omega
    $$

    ---

    ## 🌟 Deeper Reasoning
    Hewitt:  
    *"Angular momentum is the rotational 'oomph' of an object."*

    It depends on:
    - how fast it’s spinning  
    - how mass is distributed  

    ![spin](media/week7_images/College_Physics_-_Chapter_11_Book_p23_img0.png)

    ---

    ## 🎓 Advanced Concept
    Vector form:
    $$
    \vec{L} = \vec{r} \times \vec{p}
    $$

    Direction: right-hand rule.

---

# 🔵 Conservation of Angular Momentum

???+ example "Conservation of Angular Momentum"
    ## ⭐ Core Idea
    $$
    L_i = L_f
    $$  
    $$
    I_i \omega_i = I_f \omega_f
    $$

    ---

    ## 🌟 Deeper Reasoning
    Figure skaters: bring arms in → spin faster.

    Stars collapse → rotate rapidly.

    ---

    ## 🎓 Advanced Concept
    - No external torque → angular momentum fixed  
    - Internal changes (like shifting mass) affect ω  

---

# 🔵 Gyroscopes & Precession

???+ example "Gyroscopes & Precession"
    ## ⭐ Core Idea
    Precession occurs when torque acts **perpendicular** to angular momentum.

    ![gyro](media/week7_images/College_Physics_-_Chapter_11_Book_p32_img0.png)

    ---

    ## 🌟 Deeper Reasoning
    Hewitt:  
    *“A gyroscope doesn’t fall — it changes direction.”*

    Because:
    $$
    \vec{\tau} = \frac{d\vec{L}}{dt}
    $$

    ---

    ## 🎓 Advanced Concept
    Applications:
    - Bicycles  
    - Rockets  
    - Navigation systems  
    - Fidget spinners  

---

# 🧩 Worked Examples (Summary)

???+ example "Worked Examples (Summary)"
    - Torque at angle  
    - Net torque  
    - Disk rotation  
    - Parallel-axis shifts  
    - Rolling acceleration  

---

# 📝 Practice Problems

???+ example "Practice Problems"
    1. Compute \( \omega \) after 3 s with \( \alpha = 4 \text{ rad/s}^2 \).  
    2. A 15 N force at \(60^\circ\) on 0.40 m bar. Find τ.  
    3. Hoop inertia for \(m=2,r=0.5\).  
    4. Skater halves I. What happens to ω?  
    5. Sphere vs cylinder down a ramp.

???+ example "Solutions"
    1. \(12\text{ rad/s}\)  
    2. \(5.2\text{ N·m}\)  
    3. \(0.5\text{ kg·m}^2\)  
    4. ω doubles  
    5. Sphere accelerates faster


