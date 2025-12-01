# 🌀 Week 7 — Rotational Motion  
### *(Fully Illustrated — Deep Explanations — Tiered Mastery)*

Rotational motion is one of the most difficult units in all of introductory physics.  
This module is designed to take you from what you already know — **linear motion** — and build the **rotational analogs** step by step, with diagrams, explanations, examples, and conceptual checks.

---

# ⭐ 0. How to Use This Module  
??? note "Click to Expand"

    You will see **Tiered Mastery** sections:

    - **Core Idea** → What you MUST know  
    - **Deeper Reasoning** → Why it works  
    - **Advanced Application** → Calculus, AP-level thinking  

    Each major concept includes:
    - Diagrams taken from your textbook  
    - Common misconceptions  
    - Practice problems with answers hidden  
    - Connections to earlier units (Weeks 1–6)

---

# ⭐ 1. Linear → Rotational Connections (The Foundation)

??? info "1.1 Core Idea — Rotational Motion Mirrors Linear Motion"

    Physics reuses ideas. Almost everything you already know from linear motion has a rotational counterpart.

    | Linear | Rotational | Meaning |
    |--------|------------|---------|
    | \(x\) | \(\theta\) | Position |
    | \(v\) | \(\omega\) | Velocity |
    | \(a\) | \(\alpha\) | Acceleration |
    | \(m\) | \(I\) | Resistance to motion |
    | \(F\) | \(\tau\) | Cause of acceleration |
    | \(p = mv\) | \(L = I\omega\) | Momentum |
    | \(K = \tfrac12 mv^2\) | \(K = \tfrac12 I\omega^2\) | Kinetic energy |

    These connections form the *entire structure* of rotational physics.

    ![Rotational Kinematics Overview](media/week7_images/College_Physics_-_Chapter_10_Book_p0_img0.png)

??? tip "1.2 Deeper Reasoning — Why The Analogy Exists"

    Rotational motion is just linear motion… wrapped around a circle.

    - Translational position → angular position  
    - Translational velocity → rate of sweeping angle  
    - Translational acceleration → rate of change of angular speed  
    - Newton’s 2nd Law → torque version  

    Your brain already knows this — we’re just renaming ideas.

    **Big insight:**  
    > Rotation becomes difficult only because the geometry changes.  
    > The underlying *mechanics* are identical.

??? note "1.3 Advanced Application — Calculus Interpretation"

    Just like linear motion:

    \[
    v = \frac{dx}{dt}, \qquad a = \frac{dv}{dt}
    \]

    Rotational variables behave the same:

    \[
    \omega = \frac{d\theta}{dt}, \qquad \alpha = \frac{d\omega}{dt}
    \]

    If \(\alpha\) is constant:

    \[
    \omega = \omega_0 + \alpha t
    \]
    \[
    \theta = \theta_0 + \omega_0 t + \tfrac12 \alpha t^2
    \]

---

# ⭐ 2. Angular Variables: θ, ω, α

??? info "2.1 Core Idea — Angular Position, Velocity & Acceleration"

    Angular position:
    \[
    \theta(t)
    \]

    Angular velocity:
    \[
    \omega = \frac{d\theta}{dt}
    \]

    Angular acceleration:
    \[
    \alpha = \frac{d\omega}{dt}
    \]

    ![Angular position diagram](media/week7_images/College_Physics_-_Chapter_10_Book_p2_img0.png)

??? tip "2.2 Deeper Reasoning — Why Students Struggle"

    Students often think:
    - “Angular motion is new.”  
    - “There is nothing similar to linear motion.”

    But the truth:

    > Angular variables are just *linear variables restricted to circular paths.*

    Once you see that \(\theta\) is a “curved x,” everything becomes easier.

??? note "2.3 Advanced Application — Arc Length & Tangential Speed"

    Arc length relates linear to rotational motion:

    \[
    s = r \theta
    \]

    Tangential velocity:
    \[
    v = r\omega
    \]

    Tangential acceleration:
    \[
    a_t = r\alpha
    \]

    Centripetal acceleration:
    \[
    a_c = \omega^2 r
    \]

---

# ⭐ 3. Torque — The Rotational Force

??? info "3.1 Core Idea — Torque Makes Things Rotate"

    Torque (\(\tau\)) is the rotational equivalent of force.

    \[
    \tau = rF_\perp
    \]

    - \(r\) = distance from pivot  
    - \(F_\perp\) = component of force perpendicular to the lever arm  

    ![Torque lever arm](media/week7_images/College_Physics_-_Chapter_10_Book_p5_img0.png)

??? tip "3.2 Deeper Reasoning — Why the Angle Matters"

    Torque depends on **how effectively a force can twist** an object.

    The perpendicular component is:
    \[
    F_\perp = F\sin\theta
    \]

    So:
    \[
    \tau = rF\sin\theta
    \]

    Pulling at 90° gives maximum torque — this is why you push doors sideways, not upward.

??? note "3.3 Advanced Application — Right-Hand Rule (Simple Version)"

    Rotate your fingers from \(r\) toward \(F\).  
    - Thumb into the page → clockwise torque (negative)  
    - Thumb out of the page → counterclockwise torque (positive)

    ![Right hand rule](media/week7_images/College_Physics_-_Chapter_11_Book_p3_img0.png)

---

# ⭐ 4. Moment of Inertia — Mass Distribution

??? info "4.1 Core Idea — What Is Moment of Inertia?"

    Moment of inertia (\(I\)) tells you **how hard it is to spin something.**

    \[
    I = \sum mr^2
    \]

    The farther mass is from the axis, the harder it is to rotate.

    ![Moment of inertia shapes](media/week7_images/College_Physics_-_Chapter_10_Book_p8_img0.png)

??? tip "4.2 Deeper Reasoning — Why This Concept Breaks Students"

    Students try to memorize inertia formulas without understanding:

    - A door is easier to push near the hinge? **No.**  
      It is harder — small lever arm.  

    - A tightrope walker uses a long pole?  
      Large \(r\) → larger \(I\) → more stability.

    - Figure skater pulls arms in to spin faster?  
      Smaller \(r\) → smaller \(I\) → larger \(\omega\).

    **Mass distribution is everything.**

??? note "4.3 Advanced Application — Parallel Axis Theorem"

    If you know \(I_{\text{cm}}\), the moment about a parallel axis is:

    \[
    I = I_{\text{cm}} + md^2
    \]

    Where \(d\) is distance between axes.

    Extremely important for:
    - rods pivoting at ends  
    - rotating doors  
    - physical pendulums  

---

# ⭐ 5. Newton’s 2nd Law for Rotation

??? info "5.1 Core Idea — τ = Iα"

    Equivalent to \(F = ma\):

    \[
    \tau_{\text{net}} = I\alpha
    \]

    If multiple torques act:

    \[
    \sum \tau = I\alpha
    \]

    ![Torque and rotation](media/week7_images/College_Physics_-_Chapter_11_Book_p8_img0.png)

??? tip "5.2 Deeper Reasoning — Rotational Free-Body Diagrams"

    To solve rotational problems:
    1. Draw the object  
    2. Mark pivot  
    3. Add forces  
    4. Compute each force's torque  
    5. Apply \(\sum \tau = I\alpha\)

    Students often forget:
    - only perpendicular force causes torque  
    - torques have signs → clockwise vs CCW  

??? note "5.3 Advanced Application — Pulley Systems"

    For a pulley with tension \(T\):

    \[
    \tau = Tr
    \]

    If the pulley has moment of inertia \(I\):

    \[
    Tr = I\alpha
    \]

    And since \(a = r\alpha\):

    \[
    T = \frac{Ia}{r^2}
    \]

---

# ⭐ 6. Rolling Without Slipping

??? info "6.1 Core Idea — The Condition v = rω"

    Rolling without slipping means the wheel’s bottom point is **instantaneously at rest**.

    This gives the critical relation:

    \[
    v = r\omega
    \]

    ![Rolling without slipping](media/week7_images/College_Physics_-_Chapter_10_Book_p12_img0.png)

??? tip "6.2 Deeper Reasoning — Three Velocities at Once"

    For any rolling wheel:

    - Center moves at \(v\)  
    - Top moves at \(2v\)  
    - Bottom moves at \(0\)  

    Because rotation adds to translational motion at the top and subtracts at the bottom.

    Students love this diagram:

    ![Rolling velocities](media/week7_images/College_Physics_-_Chapter_10_Book_p13_img0.png)

??? note "6.3 Advanced Application — Total Kinetic Energy"

    Rolling energy is the sum of:
    - translational KE  
    - rotational KE  

    \[
    K = \tfrac12 mv^2 + \tfrac12 I\omega^2
    \]

    Using \(v = r\omega\):

    \[
    K = \tfrac12 mv^2 + \tfrac12 I\left(\frac{v}{r}\right)^2
    \]

---

# ⭐ 7. Worked Examples (Fully Guided)

??? example "Example 1 — Torque on a Wrench"

    A 0.25 m wrench feels a 120 N force at 90°.

    \[
    \tau = rF = (0.25)(120)=30\ \text{N·m}
    \]

    If applied at 30°:

    \[
    \tau = rF\sin30^\circ = (0.25)(120)(0.5)=15\ \text{N·m}
    \]

    ![Wrench torque](media/week7_images/College_Physics_-_Chapter_10_Book_p5_img0.png)

---

??? example "Example 2 — Rolling Cylinder"

    A cylinder (I = ½mr²) rolls without slipping at v = 4 m/s.

    \[
    \omega = \frac{v}{r} = \frac{4}{r}
    \]

    KE:

    \[
    K = \frac12 mv^2 + \frac12 I\omega^2
    \]
    \[
    K = \frac12 mv^2 + \frac12\left(\frac12 mr^2\right)\left(\frac{v}{r}\right)^2
    \]
    \[
    K = \frac12 mv^2 + \frac14 mv^2 = \frac34 mv^2
    \]

---

??? example "Example 3 — Rotational Acceleration"

    A 2 kg, 20 cm radius disk accelerates from rest under a 10 N tangential force.

    Tangential torque:
    \[
    \tau = rF = (0.20)(10) = 2\ \text{N·m}
    \]

    Moment of inertia of disk:
    \[
    I = \frac12 mr^2 = \frac12(2)(0.20^2)=0.04\ \text{kg·m^2}
    \]

    Angular acceleration:
    \[
    \alpha = \frac{\tau}{I}=\frac{2}{0.04}=50\ \text{rad/s}^2
    \]

---

# ⭐ 8. Practice Problems (With Hidden Solutions)

??? question "Try Before Revealing"

    1. A 15 N force at 45° acts 0.40 m from pivot. Find torque.  
    2. A disk (I = ½mr²) rolls at 3 m/s. Find ω.  
    3. A rod pivots at end. Use parallel-axis theorem: \(I = I_\text{cm}+md^2\).  
       Rod: m=2 kg, length=1.2 m. Find I_end.  
    4. A wheel accelerates from 2 to 8 rad/s in 3 s. Find α.  
    5. A 6 kg cylinder rolls without slipping. Find total KE at 5 m/s.

    ??? success "Solutions"

        1. \[
           \tau = rF\sin\theta = (0.40)(15)(\sin45^\circ)=4.24\ \text{N·m}
           \]

        2. \[
           \omega = \frac{v}{r}
           \]

        3. \[
           I_\text{cm} = \frac{1}{12}mL^2 = \frac{1}{12}(2)(1.2^2)=0.24
           \]
           \[
           I_\text{end} = I_\text{cm}+md^2 = 0.24 + 2(0.6^2)=0.96
           \]

        4. \[
           \alpha = \frac{\Delta\omega}{t} = \frac{8-2}{3}=2\ \text{rad/s}^2
           \]

        5. \[
           K = \frac12 mv^2 + \frac12 I\omega^2
           \]

---

# ⭐ 9. Summary Sheet — Exam Essentials

\[
\tau = rF\sin\theta
\]
\[
I = \sum mr^2
\]
\[
\tau = I\alpha
\]
\[
v = r\omega,\qquad a_t = r\alpha,\qquad a_c=\omega^2 r
\]
\[
K = \tfrac12 mv^2 + \tfrac12 I\omega^2
\]

---

<div align="center">



</div>

