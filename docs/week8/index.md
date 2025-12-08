# 📘 Week 8 — Oscillations  
*College Physics 201 — Calculus-Based Physics*

Oscillations show up everywhere in physics: springs, pendulums, atoms, circuits, buildings, and bridges.  
This week you’ll learn how to describe **simple harmonic motion (SHM)** mathematically, connect it to **energy** and **pendulums**, and understand **damping** and **resonance** in real systems.

Use these collapsible sections to work through the ideas at your own pace.

---

# 🔵 Simple Harmonic Motion (SHM)

???+ example "Simple Harmonic Motion (SHM)"
    ## ⭐ Core Idea  

    A system undergoes **simple harmonic motion** when the restoring force is proportional to displacement and points toward equilibrium:

    $$
    F = -kx
    $$

    This produces sinusoidal motion:

    $$
    x(t) = A\cos(\omega t + \phi)
    $$

    - **\(A\)** — amplitude (maximum displacement)  
    - **\(\omega\)** — angular frequency  
    - **\(\phi\)** — phase constant  
    - **\(x(t)\)** — displacement as a function of time  

    ![Mass–spring oscillator](/week8/media/week8_images_pdf/week8_img_0_I621.jpg)

    ---
    ### Key quantities

    - **Period \(T\)** — time for one complete cycle (seconds)  
    - **Frequency \(f\)** — cycles per second (Hz)  
    - **Angular frequency \(\omega\)** — relates to \(T\) and \(f\):

      $$
      \omega = 2\pi f = \frac{2\pi}{T}
      $$

    For a mass–spring system:

    $$
    \omega = \sqrt{\frac{k}{m}}, \quad
    T = 2\pi\sqrt{\frac{m}{k}}, \quad
    f = \frac{1}{2\pi}\sqrt{\frac{k}{m}}
    $$

    ---

    ## 🌟 Deeper Reasoning  

    SHM is defined not just by the displacement but by the **acceleration**:

    $$
    a(t) = \frac{d^2 x}{dt^2} = -\omega^2 x(t)
    $$

    That is:
    - acceleration is **always directed toward equilibrium**, and  
    - its magnitude is proportional to how far you are from equilibrium.

    This is the mathematical fingerprint of SHM.

    The **velocity** and **acceleration** follow from derivatives of \(x(t)\):

    $$
    v(t) = \frac{dx}{dt} = -A\omega \sin(\omega t + \phi)
    $$
    $$
    a(t) = \frac{dv}{dt} = -A\omega^2 \cos(\omega t + \phi) = -\omega^2 x(t)
    $$

    ![SHM position, velocity, and acceleration vs time](/week8/media/week8_images_pdf/week8_img_1_I622.jpg)

    Notice:
    - \(x(t)\) and \(a(t)\) are in phase (both cosines, opposite sign).  
    - \(v(t)\) is shifted by 90° (a sine).

    ---

    ## 🎓 Advanced Concept — Initial Conditions and Phase  

    The **phase constant \(\phi\)** is set by the initial conditions.

    At \(t = 0\):

    $$
    x(0) = A\cos\phi, \qquad
    v(0) = -A\omega\sin\phi
    $$

    You can solve these for \(A\) and \(\phi\) if you know \(x(0)\) and \(v(0)\).

    Example patterns:
    - Released from rest at **+A** → \(x(0) = +A\), \(v(0) = 0\) → \(\phi = 0\)  
    - Released from rest at **−A** → \(x(0) = −A\), \(v(0) = 0\) → \(\phi = \pi\)  
    - Passing through equilibrium with maximum positive speed → \(\phi = -\frac{\pi}{2}\)

    ---

    ### 🔶 *Worked Example: Finding the SHM Equation*

    ???+ example "Worked Example: SHM from Initial Conditions"
        A 0.50 kg mass oscillates on a spring. The amplitude is \(A = 0.12 \text{ m}\).  
        The mass is at \(x(0) = +0.06 \text{ m}\) and moving to the **left** with speed \(v(0) = 0.30 \text{ m/s}\).  
        The spring constant is \(k = 8.0 \text{ N/m}\). Find the function \(x(t)\).

        **Step 1 — Find \(\omega\)**  

        $$
        \omega = \sqrt{\frac{k}{m}} = \sqrt{\frac{8.0}{0.50}} = \sqrt{16} = 4.0 \text{ rad/s}
        $$

        **Step 2 — Use \(x(0)\) to relate \(A\) and \(\phi\)**  

        $$
        x(0) = A\cos\phi = 0.06
        $$

        With \(A = 0.12\):

        $$
        \cos\phi = \frac{0.06}{0.12} = 0.50 \Rightarrow \phi = \pm \frac{\pi}{3}
        $$

        **Step 3 — Use \(v(0)\) to choose the correct sign**  

        $$
        v(0) = -A\omega \sin\phi = - (0.12)(4.0)\sin\phi = -0.48\sin\phi
        $$

        We’re told the mass is moving **left**, so \(v(0) < 0\):

        $$
        -0.48\sin\phi = -0.30 \Rightarrow \sin\phi = 0.625
        $$

        Sin is positive and cos is positive → \(\phi\) is in quadrant I → \(\phi \approx \frac{\pi}{3}\) is correct.

        **Final Answer:**

        $$
        x(t) = 0.12\cos(4.0t + \frac{\pi}{3})
        $$

---

# 🔵 SHM and Uniform Circular Motion

???+ example "SHM and Uniform Circular Motion"
    ## ⭐ Core Idea  

    SHM can be viewed as the **shadow** of a point moving in uniform circular motion.

    Imagine a point traveling around a circle of radius \(A\) with constant angular speed \(\omega\). The projection of this point onto the x-axis follows:

    $$
    x(t) = A\cos(\omega t)
    $$

    ![Uniform circular motion and SHM projection](/week8/media/week8_images_pdf/week8_img_3_I623.jpg)

    This gives a powerful geometric interpretation of SHM.

    ---

    ## 🌟 Deeper Reasoning  

    For the circular motion:

    - Position on the circle:  
      \[
      x(t) = A\cos(\omega t), \quad y(t) = A\sin(\omega t)
      \]
    - The x-component alone behaves like SHM.

    The circular picture helps you:
    - visualize **phase** as an angle on the circle  
    - understand why SHM is sinusoidal  
    - connect SHM to wave motion later  

    ---

    ## 🎓 Advanced Concept — Phase and Initial Angle  

    If the rotating point starts at angle \(\phi\) at \(t = 0\), then:

    $$
    x(t) = A\cos(\omega t + \phi)
    $$

    The **phase constant \(\phi\)** is literally the starting angle on the reference circle.

---

# 🔵 Energy in Oscillations

???+ example "Energy in Oscillations"
    ## ⭐ Core Idea  

    For a mass–spring system in SHM (no friction):

    - **Spring potential energy:**
      $$
      U = \frac12 kx^2
      $$
    - **Kinetic energy:**
      $$
      K = \frac12 mv^2
      $$

    The **total mechanical energy** is constant:

    $$
    E = K + U = \frac12 kA^2
    $$

    ![Energy vs position in SHM](/week8/media/week8_images_pdf/week8_img_3_I624.jpg)

    At:
    - \(x = 0\) → \(U = 0\), \(K = E\)  
    - \(x = \pm A\) → \(U = E\), \(K = 0\)

    ---

    ## 🌟 Deeper Reasoning — Velocity from Energy  

    Conservation of energy provides a very useful relation:

    $$
    \frac12 mv^2 + \frac12 kx^2 = \frac12 kA^2
    $$

    Solving for \(v\):

    $$
    v(x) = \pm \sqrt{\frac{k}{m}(A^2 - x^2)} = \pm \omega \sqrt{A^2 - x^2}
    $$

    This tells you how fast the mass is moving at any position \(x\), without needing time \(t\).

    ---

    ## 🎓 Advanced Concept — Turning Points & Energy Diagrams  

    - **Turning points** occur where \(v = 0\) → all energy is potential.
    - For SHM, these are at \(x = \pm A\).  
    - On an energy vs. position graph, the total energy is a **horizontal line**, and the potential energy is a **parabola**.

    The intersection points of these curves give the maximum allowed displacement.

    ---

    ### 🔶 *Worked Example: Speed from Energy*

    ???+ example "Worked Example: Speed at a Given Position"
        A 0.40 kg block oscillates on a spring with \(k = 16\text{ N/m}\) and amplitude \(A = 0.25 \text{ m}\).

        **(a)** What is the total mechanical energy?  
        **(b)** What is the speed at \(x = 0.15 \text{ m}\)?

        **(a) Total energy**

        $$
        E = \frac12 kA^2 = \frac12(16)(0.25^2) = 8(0.0625) = 0.50 \text{ J}
        $$

        **(b) Speed at \(x = 0.15\)**  

        Energy conservation:

        $$
        \frac12 mv^2 + \frac12 kx^2 = E
        $$
        $$
        \frac12 (0.40)v^2 + \frac12(16)(0.15^2) = 0.50
        $$

        Compute the potential term:

        $$
        \frac12(16)(0.0225) = 8(0.0225) = 0.18 \text{ J}
        $$

        So:

        $$
        \frac12 (0.40)v^2 = 0.50 - 0.18 = 0.32
        $$
        $$
        0.20 v^2 = 0.32 \Rightarrow v^2 = 1.60 \Rightarrow v = 1.26 \text{ m/s}
        $$

        **Answer:** \(v \approx 1.26 \text{ m/s}\)

---

# 🔵 Pendulums

???+ example "Pendulums"
    ## ⭐ Core Idea — Simple Pendulum  

    A **simple pendulum** is a point mass \(m\) on a massless string of length \(L\), swinging under gravity.  

    For **small angles** (\(\theta \lesssim 10^\circ\)), the motion is approximately SHM with period:

    $$
    T = 2\pi \sqrt{\frac{L}{g}}
    $$

    ![Simple pendulum geometry](/week8/media/week8_images_pdf/week8_img_4_I625.jpg)

    Key points:
    - Period does **not** depend on mass.  
    - Period increases with length.  
    - Period decreases if gravity is stronger.

    ---

    ## 🌟 Deeper Reasoning — Small-Angle Approximation  

    The tangential component of gravity is:

    $$
    F_t = -mg\sin\theta
    $$

    For small angles, \(\sin\theta \approx \theta\) (in radians), so:

    $$
    F_t \approx -mg\theta
    $$

    The resulting angular equation of motion has the same form as SHM:

    $$
    \ddot{\theta} + \frac{g}{L}\theta = 0
    $$

    Giving:

    $$
    \omega = \sqrt{\frac{g}{L}}, \quad T = 2\pi\sqrt{\frac{L}{g}}
    $$

    ---

    ## 🎓 Advanced Concept — Physical Pendulum  

    A **physical pendulum** is any rigid body swinging about a pivot.

    For small oscillations, the period is:

    $$
    T = 2\pi\sqrt{\frac{I}{mgd}}
    $$

    Where:
    - \(I\) — moment of inertia about the pivot  
    - \(d\) — distance from pivot to center of mass  

    ![Physical pendulum example](/week8/media/week8_images_pdf/week8_img_4_I626.jpg)

    ---

    ### 🔶 *Worked Example: Simple Pendulum Period*

    ???+ example "Worked Example: Pendulum on Earth"
        A simple pendulum has length \(L = 1.10 \text{ m}\).  

        **Find its period on Earth (\(g = 9.80 \text{ m/s}^2\)).**

        $$
        T = 2\pi \sqrt{\frac{L}{g}} = 2\pi\sqrt{\frac{1.10}{9.80}}
        $$

        $$
        \frac{1.10}{9.80} \approx 0.1122,\quad \sqrt{0.1122} \approx 0.335
        $$

        $$
        T \approx 2\pi(0.335) \approx 2.10 \text{ s}
        $$

        **Answer:** \(T \approx 2.1\text{ s}\)

---

# 🔵 Damping

???+ example "Damping"
    ## ⭐ Core Idea  

    Real oscillators lose energy over time due to friction or drag.  
    The amplitude of motion **decreases** with time — this is called **damping**.

    Types of damping:
    - **Underdamped** — oscillates with decreasing amplitude  
    - **Critically damped** — returns to equilibrium as fast as possible without oscillating  
    - **Overdamped** — returns slowly, no oscillations  

    ![Damped oscillation envelopes](/week8/media/week8_images_pdf/week8_img_5_I627.jpg)

    ---

    ## 🌟 Deeper Reasoning — Exponential Decay  

    For a lightly damped oscillator, the amplitude obeys:

    $$
    A(t) = A_0 e^{-\frac{b}{2m} t}
    $$

    where \(b\) is the damping constant.

    The motion looks like SHM with a slowly shrinking envelope.

    ---

    ## 🎓 Advanced Concept — Damped Frequency  

    Without derivation, the **damped angular frequency** is:

    $$
    \omega_d = \sqrt{\omega_0^2 - \left(\frac{b}{2m}\right)^2}
    $$

    where \(\omega_0 = \sqrt{\frac{k}{m}}\) is the undamped natural frequency.

    For light damping, \(\omega_d \approx \omega_0\).

---

# 🔵 Driven Oscillations & Resonance

???+ example "Driven Oscillations & Resonance"
    ## ⭐ Core Idea  

    If an oscillator is subjected to a **periodic driving force**:

    $$
    F(t) = F_0 \sin(\omega t)
    $$

    it eventually oscillates at the **driving frequency**. The **amplitude** of steady-state oscillation depends on how close the driving frequency is to the system’s **natural frequency**.

    When these match, the system is in **resonance** and the amplitude can become very large.

    ![Resonance curves with different damping](/week8/media/week8_images_pdf/week8_img_6_I628.jpg)

    ---

    ## 🌟 Deeper Reasoning  

    - If the driving frequency is **far** from the natural frequency → small response.  
    - If the driving frequency is **near** the natural frequency → big response.  
    - Lower damping → **taller & narrower** resonance peak.  
    - Higher damping → **shorter & wider** resonance peak.

    Real-world relevance:
    - Bridges and buildings (wind, earthquakes)  
    - Musical instruments  
    - Radio circuits (tuning)  
    - MRI machines  

    ---

    ## 🎓 Advanced Concept — Qualitative Equation  

    The full driven, damped oscillator equation is:

    $$
    m\ddot{x} + b\dot{x} + kx = F_0 \sin(\omega t)
    $$

    We **do not** solve this in this course, but we use its qualitative behavior:
    - driving term → sets the steady-state frequency  
    - damping term → limits amplitude and broadens resonance  

---

# 🧩 Worked Examples (Summary)

???+ example "Worked Examples (Summary)"
    **Covered above:**
    - SHM from initial conditions  
    - Speed at a position using energy  
    - Simple pendulum period  
    - Physical pendulum concept  
    - Identifying damping and resonance behavior  

    Use these as models when working through the practice problems.

---

# 📝 Practice Problems

???+ example "Practice Problems"
    1. **Mass–Spring Frequency**  
       A 0.30 kg mass is attached to a spring with \(k = 12 \text{ N/m}\).  
       (a) Find \(\omega\), \(T\), and \(f\).  
       (b) If \(A = 0.080 \text{ m}\), write \(x(t)\) assuming release from rest at \(x = +A\).

    2. **Speed at a Position**  
       A 0.50 kg mass oscillates with amplitude \(0.10\text{ m}\) on a spring whose natural frequency is \(\omega = 6.0 \text{ rad/s}\).  
       Find the speed at \(x = 0.06 \text{ m}\).

    3. **Energy and Turning Points**  
       A mass–spring system has total energy \(E = 0.40 \text{ J}\) and spring constant \(k = 20 \text{ N/m}\).  
       (a) Find the amplitude.  
       (b) At what displacement is the kinetic energy half of the total energy?

    4. **Pendulum on Earth vs. Moon**  
       A 1.00 m simple pendulum has period \(T_E\) on Earth.  
       (a) Find \(T_E\).  
       (b) On a moon where \(g_{\text{moon}} = 1.6 \text{ m/s}^2\), find its new period.

    5. **Damping Type Identification**  
       Given three displacement vs. time graphs:  
       - Graph A: quickly returns to equilibrium, no oscillations.  
       - Graph B: oscillations with slowly shrinking amplitude.  
       - Graph C: very slow return, no oscillations.  
       Label each as underdamped, critically damped, or overdamped.

    6. **Resonance Concept**  
       Explain why a lightly damped system can be dangerous if driven near its natural frequency. Give one real-world example.

???+ example "Solutions (Sketch Only)"
    1. **Mass–Spring Frequency**
       - (a)  
         $$
         \omega = \sqrt{\frac{12}{0.30}} = \sqrt{40} \approx 6.32\text{ rad/s}
         $$
         $$
         T = \frac{2\pi}{\omega} \approx \frac{2\pi}{6.32} \approx 0.995\text{ s}, \quad
         f \approx 1.00\text{ Hz}
         $$
         (b) Release from rest at \(+A\) → \(\phi = 0\):
         $$
         x(t) = 0.080\cos(6.32t)
         $$

    2. **Speed at a Position**
       $$
       v(x) = \omega\sqrt{A^2 - x^2} = 6.0\sqrt{0.10^2 - 0.06^2}
       $$
       $$
       = 6.0\sqrt{0.01 - 0.0036} = 6.0\sqrt{0.0064} = 6.0(0.080) = 0.48\text{ m/s}
       $$

    3. **Energy and Turning Points**
       - (a)
         $$
         E = \frac12 kA^2 \Rightarrow 0.40 = \frac12(20)A^2 = 10A^2
         $$
         $$
         A^2 = 0.04 \Rightarrow A = 0.20\text{ m}
         $$
       - (b) Half kinetic → \(K = E/2 = 0.20\), so \(U = 0.20\):
         $$
         U = \frac12 kx^2 = \frac12(20)x^2 = 10x^2 = 0.20
         $$
         $$
         x^2 = 0.02 \Rightarrow x \approx 0.141\text{ m}
         $$

    4. **Pendulum on Earth vs. Moon**
       - (a)
         $$
         T_E = 2\pi\sqrt{\frac{1.00}{9.80}} \approx 2.01\text{ s}
         $$
       - (b)
         $$
         T_{\text{moon}} = 2\pi\sqrt{\frac{1.00}{1.6}} \approx 4.97\text{ s}
         $$

    5. **Damping Types**
       - Graph A → critically damped  
       - Graph B → underdamped  
       - Graph C → overdamped  

    6. **Resonance Concept**
       - Lightly damped systems have large amplitudes when driven near their natural frequency.
       - Example: a bridge oscillating due to periodic wind or marching soldiers; a wine glass shattering under a singer’s resonant note.

---


