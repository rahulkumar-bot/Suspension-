# Suspension System — CAD Project

A suspension system is what connects the wheels
of a vehicle to its body. It absorbs bumps from
the road so the ride stays smooth and the wheels
stay in contact with the ground.

In this project, I designed the full suspension
geometry in 3D — including the control arms,
knuckle, and spring-damper setup. Everything
is modeled as it would work in a real vehicle.

<img width="409" height="511" alt="Suspention" src="https://github.com/user-attachments/assets/142b1424-01f7-4604-900d-9548bc0a760e" />

# Suspension Damper Assembly
A parametric CAD model of a coilover (coil-spring-over-damper) suspension unit, featuring a telescoping shock absorber body, helical compression spring, adjustable spring perch, and dual mounting eyelets.

## Overview

This repository contains the 3D CAD design of a **coilover suspension unit**, commonly used in automotive and motorsport suspension systems to combine damping and spring-rate control into a single assembly. The design demonstrates:

- Concentric spring-over-damper packaging
- A threaded, adjustable spring perch for ride-height / preload tuning
- Rod-end (eyelet) mounts at both ends for chassis and control-arm attachment
- Standard coil spring geometry seated on upper and lower spring cups

| Component (color in render) | Description |
|---|---|
| Damper body / piston rod (green) | Houses the hydraulic/gas damping mechanism; the rod extends/retracts under load |
| Coil spring (red) | Helical compression spring providing the suspension's spring rate |
| Adjustable spring perch (blue) | Threaded collar that sets spring preload and ride height |
| Lower mounting eyelet (yellow) | Rod-end bushing/bearing interface to the lower control arm or axle |
| Locking rings / jam nuts (black) | Lock the perch position after adjustment |

## Specifications

> Fill in actual values from your model / design intent before publishing.

| Parameter | Value |
|---|---|
| Overall extended length | `45 mm` |
| Overall compressed length | `45 mm` |
| Stroke length | `180 mm` |
| Spring free length | `100 mm` |
| Spring wire diameter | `7.2 mm` |
| Spring outer diameter | `38.6 mm` |
| Material — damper body | `6061-T6 Aluminum` |
| Material — spring | `Silicon Chromium Steel)` |

## Why I made this

I wanted to understand how suspension geometry
affects the way a vehicle handles. Instead of
just reading about it, I decided to actually
design one myself.

This project helped me learn:
- How double wishbone / MacPherson suspension works
- How to model moving parts and joints in CAD
- How camber, caster, and toe angles are set
- How to think like a mechanical engineer

## Repository Structure

```
Suspension-cad/
├── README.md
├── LICENSE
├── CAD/
│   ├── native/              # Editable source files (.stl, .dwg, .f3d, .ipt, .iam, etc.)
│   ├── step/                # Neutral exchange format (.step / .stp) — for anyone without your CAD license
│   ├── parasolid/           # Optional (.x_t / .x_b)
│   └── drawings/            # 2D engineering drawings (.pdf / .dwg)
├── assets/
│   ├── renders/             # High-quality isometric / exploded renders (like the one above)
│   ├── screenshots/         # Quick-reference views (front, section, BOM callouts)
│   └── gifs/                # Optional: assembly animation, motion study
├── docs/
│   ├── BOM.md                # Bill of materials
│   ├── design_notes.md       # Design rationale, load cases, calculations
│   └── FEA/                  # Simulation results, stress plots, reports (if performed)
└── .gitignore
```
---

## Bill of Materials (BOM)

| # | Part Name | Qty | Material | Notes |
|---|---|---|---|---|
| 1 | Damper Body | 1 | Aluminum 6061-T6 | Houses piston/rod assembly |
| 2 | Piston Rod | 1 | Chromed Steel | Telescoping shaft |
| 3 | Coil Spring | 1 | Spring Steel (Chrome Silicon) | Compression spring |
| 4 | Adjustable Spring Perch | 1 | Steel / Aluminum | Threaded, sets preload |
| 5 | Upper/Lower Spring Cups | 2 | Steel | Seats spring ends |
| 6 | Lower Mounting Eyelet | 1 | Steel | Rod-end / bushing bore |
| 7 | Upper Mounting Stud/Eyelet | 1 | Steel | Chassis mount |
| 8 | Locking Ring / Jam Nut | 1–2 | Steel | Locks perch after adjustment |

## Tools & Software I used

-**Fusion 360** — for 3D modeling and assembly
-**GitHub** — to save and track my work

> No special tools needed to view the design.
> Just open the .STL file on GitHub and it shows
> a 3D preview right in your browser.

## What I learned

The hardest part was getting the geometry right.
Small changes in the control arm angles make a
big difference to how the suspension moves.

I also learned that in real vehicles, every
dimension is carefully calculated — nothing
is random. This project gave me a much better
understanding of how cars are actually engineered.

## Current status

🔧 Work in progress — still refining the geometry
and adding more detail to the assembly.

This is a private learning project.
Not intended for commercial use.
