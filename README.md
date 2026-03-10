# Cigarette Rocket Booster (CRB) — Concept Disclosure

**Date of Disclosure:** March 10, 2026  
**Author:** Aleksei Shtorm / Solenopsys  
**License:** CERN Open Hardware Licence Strongly Reciprocal v2 (CERN OHL-S v2)  
**Purpose:** Public disclosure to establish priority date and prevent future patent trolling.

---

## Abstract

A rocket propulsion system where the structural body of the rocket itself serves as the fuel.  
The rocket consists of a 3D-printed porous metal matrix (magnesium alloy) which is simultaneously:
- The combustion chamber
- The fuel
- The nozzle array

There are **no moving parts**, no separate fuel tanks, no turbopumps, no valves.  
The entire rocket is consumed during flight, leaving only the payload module.

This is not a reusable launch vehicle competing with Falcon 9. This is a **disposable launch unit** — the aerospace equivalent of a lighter. Print, load, fire, done.

---

## 1. Field

Aerospace propulsion. Additive manufacturing of rocket systems.  
AI-optimized structural design for ballistic and orbital applications.  
Target application: dedicated microsatellite launches, 100–200 kg to LEO.

---

## 2. Problem Statement

Conventional rockets suffer from:
- High structural dead weight (tanks, pumps, plumbing ~85-90% of mass)
- Complex assembly from thousands of parts
- Long manufacturing and integration cycles
- High cost per launch driven by labor, not materials

**Goal:** Reduce cost per kg to LEO by an order of magnitude through radical manufacturing simplification. Not by reusability — by eliminating complexity entirely.

---

## 3. Core Invention

The rocket is not built around a conventional engine. **The rocket body itself is the engine, the fuel, and the combustion architecture.**

It is manufactured as a 3D-printed porous reactive metal matrix — for example a magnesium alloy structure — whose internal geometry contains a very large number of distributed micro-combustion cells, channels, and nozzle-like passages.

The system does not rely on one main chamber and one main nozzle. Instead, thrust is produced by the combined action of thousands or millions of microscopic reactive elements distributed throughout the body.

The key principle is not perfect stability of each individual cell, but **macroscopic stability emerging from the statistical behavior of the whole matrix**. Local irregularities, local erosion, or local failure of individual cells do not destroy propulsion — total thrust is the averaged result of a very large population of micro-reactive structures.

The structural body is progressively consumed during operation. This consumption is not random burn-through — **it is programmed into the geometry itself.**

Porosity, channel density, wall thickness, connectivity, and reactive mass distribution vary along the body so that burn progression, thrust development, and mass reduction are encoded directly into the printed structure.

**The rocket is not merely designed in CAD. It is computationally synthesized.**

Its geometry is generated through iterative simulation and AI-assisted optimization — because the internal architecture is too complex to be manually designed at full fidelity by a human engineer.

The mission profile is therefore physically compiled into the rocket body:
- the structure carries load
- the structure stores reactive mass
- the structure forms distributed combustion zones
- the structure determines how propulsion evolves during flight

Each rocket is printed as a **mission-specific object** rather than assembled as a standard vehicle with fixed engine hardware. Different orbit = different geometry = reprint.

### 3.1 Manufacturing Method — Stationary Printer / Descending Build

Key manufacturing innovation:

- Print head is **stationary**, fixed at one height
- Build platform descends continuously as layers are added
- Enables fabrication of arbitrarily long cylindrical bodies (10–12+ meters) without height-limited build chambers
- Single printer, single material, single process
- No assembly, no post-processing, no human integration steps

### 3.2 Oxidizer Loading

The porous matrix is saturated with liquid oxidizer (LOX or equivalent) prior to or at the launch site. The specific loading method is not constrained by this disclosure — viable approaches include pressure infiltration, vacuum-assisted flooding, or staged cryogenic filling at the launch stand.

Both open-ended and sealed-base configurations are considered. In the sealed-base variant, ignition may be initiated by a high-energy pulse (explosive or pyrotechnic initiator) that simultaneously ruptures the base seal and initiates combustion across the matrix face.

The absence of fill lines, valves, or pumps in the propulsion path is the key property — not the specific loading procedure.

### 3.3 Flight Control

Three hybrid fin/thruster assemblies mounted on payload module:
- **In atmosphere:** Aerodynamic control surfaces
- **Above atmosphere:** Gas-dynamic vanes in exhaust stream
- **Fine correction:** Micro cold-gas thrusters
- **Primary stabilization:** Gyroscopic spin from helical surface ribs printed integrally — passive, no actuators

### 3.4 Payload Module

The payload module (satellite bus) is not a separate launch component. It is manufactured by the same LPBF process from the same material family, snaps onto the rocket body, and remains on orbit as a functional spacecraft after the propulsion body is consumed. Its cost is attributed to the satellite, not to the launch vehicle.

---

## 4. Key Claims (Prior Art)

The following combinations are claimed as novel prior art:

1. Rocket where **structural body = fuel** (magnesium matrix consumed during flight)
2. **AI-synthesized fractal nozzle matrix** where burn profile encodes trajectory
3. **Stationary print head / descending build** for arbitrarily long rocket bodies
4. **Porous matrix oxidizer loading** without valves or fill lines in propulsion path
5. **Explosive base ignition** of sealed porous reactive metal matrix
6. **Spin stabilization via helical surface features** printed integrally with rocket body
7. **Mission-specific geometry** — each rocket printed with unique AI-optimized structure for target orbit
8. **Payload module as structural continuation** of rocket body, manufactured in same process

---

## 5. Approximate Parameters

| Parameter | Value |
|-----------|-------|
| Length | 12 m |
| Diameter | 0.4–0.5 m |
| Matrix material | Mg alloy AZ31 or similar |
| Oxidizer | LOX |
| Matrix porosity | ~65% |
| Mg matrix mass | ~919 kg |
| LOX mass | ~1,118 kg |
| Total propellant mass | ~2,037 kg |
| Estimated Isp | 280–310 s |
| Target payload | 100–200 kg |
| Target orbit | LEO 400–600 km |

*Single-stage orbital capability depends on AI-optimized burn profile and achieved Isp. Two-stage variant — two printed tubes, second stage smaller diameter — is baseline fallback.*

---

## 6. Economics

### 6.1 Per-Unit Cost Breakdown

| Item | Cost |
|------|------|
| Mg alloy powder LPBF grade ~919 kg × $30/kg | $27,500 |
| LOX ~1,118 kg × $0.12/kg | $135 |
| Machine time ~150 hrs × $10/hr amortized | $1,500 |
| Avionics + fins + initiator | $8,000–12,000 |
| **Total per unit (serial production)** | **$37,000–41,000** |

At scale with in-house powder production: **$20,000–25,000** per unit is a realistic target.

### 6.2 Cost per kg to LEO

| Scenario | Unit Cost | Launch Price | Payload | $/kg LEO |
|----------|-----------|--------------|---------|----------|
| Conservative | $40k | $200k | 100 kg | $2,000 |
| Baseline | $30k | $150k | 150 kg | $1,000 |
| Serial production | $20k | $100k | 200 kg | $500 |

### 6.3 CRB vs Existing Systems

| Parameter | Falcon 9 | Rocket Lab Electron | **CRB** |
|-----------|----------|---------------------|----------|
| Payload to LEO | 22,800 kg | 300 kg | 100–200 kg |
| Launch price | ~$70M | ~$8M | **~$50-100k** |
| $/kg LEO | ~$2,700 | ~$7,000 | **$500** |
| Parts count | ~100,000 | ~10,000 | **~1** |
| Assembly required | Months | Weeks | **None** |
| Moving parts in propulsion | Yes | Yes | **Zero** |
| Manufacturing process | Multi-step manual | Multi-step manual | **Single LPBF print** |
| Post-processing | Extensive | Extensive | **None** |
| Human labor per unit | High | High | **Near zero** |
| Time from order to launch | Months | Months | **Days** |
| Reusability | Partial | No | **Not applicable** |

The competitive advantage is not reusability or peak performance. It is **radical manufacturing simplicity**. The entire production pipeline is:

**digital model → LPBF printer → oxidizer loading → launch**

No assembly. No post-processing. No moving parts to inspect or certify. Fully automated from file to flight.

Target market: microsatellite operators needing dedicated low-cost launches on short notice — not shared rideshare slots on large vehicles scheduled 18 months out.

---

## 7. What This Is Not

- This is not a complete engineering design
- This is not a tested system
- This is a concept disclosure for prior art purposes

---

## 8. Open Questions for Research

- Actual Isp achievable in porous Mg+LOX matrix combustion
- Minimum pore size for stable combustion vs capillary retention of LOX
- MgO slag accumulation effects on thrust profile
- AI optimization convergence for trajectory-encoded geometry
- Numerical simulation of continuously-consuming structural mass (non-standard Tsiolkovsky)

---

---

## License

**CERN Open Hardware Licence Strongly Reciprocal v2 (CERN OHL-S v2)**

Copyright (c) 2026 Aleksei Shtorm / Solenopsys

You may use, copy, modify and distribute this work and derivatives freely, including for commercial purposes, under the following conditions:
- All derivative works must be released under the same CERN OHL-S v2 license
- All modifications must be publicly documented
- You may not use patents or trade secrets to restrict use of this work or its derivatives

Full license text: https://ohwr.org/cern_ohl_s_v2.txt

**This publication establishes prior art. Any patent filed after March 10, 2026 covering the above claims is invalid under prior art doctrine.**
