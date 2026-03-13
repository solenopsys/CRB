

**Launch System**

**1. Acceleration profile**
CRB is designed for 100g peak acceleration. At this profile the rocket crosses the Kármán line in under 45 seconds. The dense atmosphere (0–15 km) is traversed in approximately 10 seconds — faster than the thermal inertia of the structure, making dedicated heat shielding unnecessary. The aerodynamic nose cone handles stagnation heating; the body behind it remains in the shock shadow throughout ascent.

**2. Launch installation**
The launch complex is a 0.5 m steel tube set in concrete in the ground with three peripheral guides to stabilize the rocket during initial acceleration. No launch tower, no service structure, no complex ground support. Total infrastructure cost is lower than the rocket itself. The tube is reusable. The installation can be deployed in any flat terrain — desert, steppe, barge — making mobile and distributed launch operations feasible without dedicated spaceport infrastructure.

**3. Ignition system**
Ignition is achieved in two stages. A high-frequency oscillator first ionizes the air gap between a ceramic igniter disk and the base of the rocket matrix, establishing thousands of conductive plasma channels — one per micro-chamber — simultaneously. A capacitor bank then discharges through timed thyristors, driving simultaneous arc strikes across all 2,000–3,000 chamber inlets in microseconds. Chamber pressure rises from zero to 300 bar across the full cross-section synchronously. No mechanical contact, no moving parts, no sequential ignition wave.

 

**CRB — Integrated Flight Profile**

| Altitude | Time | Velocity | Mach | Accel | Chamber pressure | Body length | L/d | Stability |
|----------|------|----------|------|-------|-----------------|-------------|-----|-----------|
| 0 km | 0 s | 0 m/s | 0 | 10g | 18 bar | 12.0 m | 30 | risk* |
| 2 km | 6 s | 626 m/s | 1.9 | 10g | 15 bar | 9.9 m | 25 | stable |
| 5 km | 10 s | 990 m/s | 3.1 | 10g | 13 bar | 8.6 m | 22 | stable |
| 8 km | 13 s | 1,253 m/s | 4.1 | 10g | 12 bar | 7.7 m | 19 | stable |
| 10 km | 14 s | 1,401 m/s | 4.7 | 10g | 11 bar | 7.2 m | 18 | stable |
| 15 km | 18 s | 1,716 m/s | 5.8 | 10g | 9 bar | 6.2 m | 15 | stable |
| 20 km | 20 s | 2,426 m/s | 8.2 | 30g | 24 bar | 5.4 m | 13 | excellent |
| 30 km | 23 s | 3,431 m/s | 11.4 | 30g | 19 bar | 4.2 m | 11 | excellent |
| 50 km | 28 s | 4,852 m/s | 15.4 | 30g | 12 bar | 2.6 m | 7 | excellent |
| 70 km | 32 s | 5,943 m/s | 18.2 | 30g | 6 bar | 1.4 m | 4 | excellent |
| 100 km | 36 s | 7,278 m/s | 21.1 | 30g | 1 bar | 0.5 m | 1 | excellent |

*At launch: buckling risk is eliminated by launch tube lateral guides and internal pressure stabilization.

**Three properties no conventional rocket shares:**

**1. Structure becomes more stable as it flies.** The body burns from the base up. By the time peak acceleration begins at 15 km, the column is already 6 m shorter than at liftoff — L/d drops from 30 to 15, moving well clear of the Euler buckling threshold. At 50 km the remaining structure is 2.6 m long. At 70 km it is 1.4 m. The rocket is most stable precisely when it is working hardest.

**2. Working pressure is a fraction of structural capacity.** Chamber pressure during flight ranges from 9 to 24 bar across the ascent profile. The matrix is rated to 300+ bar. The structure operates at 10–30× below its pressure limit at all times. There is no red line in this flight envelope.

**3. Gravity losses are 5% of orbital velocity.** A conventional rocket accelerating at 1.5g spends 200+ seconds fighting gravity, losing 30–40% of its total delta-V before clearing the atmosphere. CRB reaches the Kármán line in 36 seconds. Gravity losses amount to ~357 m/s — under 5% of the 7,800 m/s needed for LEO. The rest goes directly into orbital velocity. This is not an optimization. It is a structural consequence: a rocket that is almost entirely propellant with no dead mass accelerates fast by definition, and a rocket that accelerates fast wastes almost nothing on gravity.


Вот два раздела:

---

###  Fractal Combustion Architecture

In CRB, the distinction between combustion chamber and nozzle is not spatial in the conventional sense — there is no fixed chamber upstream and fixed nozzle downstream. Instead, every cell in the matrix passes through a defined lifecycle:

1. **Storage** — cell is intact, PTFE-sealed, saturated with LOX
2. **Combustion chamber** — PTFE is arc-ignited, metal burns, pressure peaks locally
3. **Nozzle** — metal is consumed, cavity geometry expands, accelerates exhaust gas
4. **Regenerative cooling** — while acting as nozzle, adjacent LOX microchannels flowing toward the active combustion front simultaneously cool the nozzle walls

This lifecycle is not sequential along the axis of the rocket. It is distributed across a fractal ornamental pattern throughout the entire cross-section. At any given moment, the same transverse slice contains cells in all four states simultaneously — arranged by the fractal geometry so that every active combustion cell is always adjacent to a nozzle cell, and every nozzle cell is always adjacent to a LOX-carrying cooling channel.

The result is regenerative cooling with no tubes, no manifolds, and no pumps — an emergent property of the printed geometry. This is the same principle used in Raptor and Merlin, where fuel cools the nozzle before entering the combustion chamber. In CRB it emerges naturally from the fractal structure rather than from hundreds of hand-designed channels.

A single printed element simultaneously performs: propellant storage, combustion, nozzle expansion, regenerative cooling, and combustion front control. No existing engine architecture combines all five functions in one structure without moving parts.

---

###  AI Synthesis — Why This Cannot Be Designed by Hand

The fractal combustion architecture described in 3.4 cannot be designed by a human engineer. The number of interdependent geometric variables — cell diameter, wall thickness, channel connectivity, local porosity, PTFE coverage pattern, nozzle expansion ratio distribution — exceeds what analytical or manual CAD methods can optimize simultaneously. A structure that looks correct in cross-section may produce unstable combustion front propagation, asymmetric thrust, or nozzle wall burnthrough at full pressure. The interactions are non-linear and non-local.

The synthesis pipeline is:

**Stage 1 — Random initialization.** A genetic algorithm generates thousands of randomized fractal structures across the design space. No structure is optimal; the purpose is coverage.

**Stage 2 — Physics simulation.** Each candidate is evaluated through coupled CFD, thermodynamics, and structural mechanics — Isp, thrust profile, wall temperature, combustion front stability. Most candidates fail.

**Stage 3 — Selection and mutation.** High-performing structures are crossed and mutated. Counterintuitive patterns emerge — asymmetric ornaments, non-obvious chamber-to-channel ratios — that no human designer would have proposed.

**Stage 4 — Neural network acceleration.** A model trained on simulation results learns to predict structural performance without full CFD. Search speed increases by orders of magnitude.

**Stage 5 — Mission-specific synthesis.** For each new mission, target orbit parameters are provided as input. The system outputs an optimized geometry within hours. The file goes directly to the LPBF printer.

This pipeline transforms CRB from a rocket into a **platform**. The physical principle is fixed and disclosed. The geometry is different for every mission — synthesized, not designed. Each rocket is a unique AI-generated object compiled from a mission profile, not assembled from standard hardware.

 
###  Why the Standard Tsiolkovsky Interpretation Is Misleading for CRB

The Tsiolkovsky rocket equation applies to CRB without exception — CRB is a reaction-propelled vehicle that gains velocity by expelling mass, and the conservation of momentum is not negotiable.

What changes is the mass accounting.

In a conventional rocket, structural mass is fixed and permanent. Tanks, engine casings, feed lines, and load-bearing walls remain with the vehicle from liftoff to burnout — dead weight that must be accelerated throughout the entire flight while contributing nothing to propulsion after the first second. The rocket equation penalizes this harshly: every kilogram of inert structure requires exponentially more propellant to reach orbital velocity.

In CRB the reactive matrix is simultaneously propellant and load-bearing structure. As the vehicle operates, the material that was carrying mechanical load a moment ago is consumed and expelled as exhaust. Structure does not accumulate as dead mass — it is progressively converted into thrust.

This does not break Tsiolkovsky. It changes what the final dry mass term actually contains.

| Burned | Reactive mass remaining | Total vehicle mass |
|--------|------------------------|-------------------|
| 0% | 2,037 kg | 2,487 kg |
| 25% | 1,528 kg | 1,978 kg |
| 50% | 1,018 kg | 1,468 kg |
| 75% | 509 kg | 959 kg |
| 100% | 0 kg | 450 kg |

The residual dry mass of CRB — avionics, fins, nose cone, igniter — is approximately 300 kg on a 2,337 kg vehicle: 12.8% of total mass. In conventional single-stage architectures, structural mass fraction rarely falls below 8–12%, but that fraction includes permanent engine hardware, tank walls, and plumbing that serve no propulsive function after ignition. In CRB the structural material that performs load-bearing function during flight is the same material that is being consumed to produce thrust.

The correct framing is not "CRB escapes the rocket equation" but rather: **CRB achieves an unusually low residual inert mass fraction because most of its structural mass is consumable.** That is the architectural advantage — not a violation of classical mechanics, but a fundamentally different relationship between structure and propellant mass.
 
 
