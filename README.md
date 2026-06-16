# Cal Poly VR SCUBA Simulator

A WebGL virtual reality SCUBA diving simulation built for K-12 education and professional underwater survey training. Developed in collaboration with the National Science Foundation and a Cal Poly marine biologist.

> **Note:** This project is maintained under the official research organization's repository. This repo documents my contributions as Project Manager and Full Stack Developer (Sep 2024 – Apr 2025).

---

## Overview

This simulation teaches two skills:
- **Underwater transect surveying** — the standard method marine biologists use to count and classify species in a defined corridor. Used by researchers and companies like Microsoft for environmental monitoring.
- **Shark encounter safety** — the correct behavioral response to a shark encounter underwater, delivered through an interactive Shark Dive game mode.

The target audience spans K-12 students experiencing ocean science for the first time and professional surveyors learning standardized field methodology.

---

## My Contributions

### Marine Species Modeling & Integration
Modeled 4 native California marine species in Blender and integrated them into the Unity environment:
- Rigged meshes with idle animation cycles
- Implemented species-specific spawning logic in C# (spawn zones, density parameters, population caps)
- Added collision volumes for survey interaction (players can "count" a species by looking at it within the transect corridor)
- Validated species appearance and behavior with a Cal Poly marine biologist across Agile sprints

### Shark Dive Game Mode
Built an entirely new game mode for shark encounter training:
- **Shark AI** — state machine controlling patrol, approach, and retreat behaviors based on player proximity and movement
- **Collision detection** — triggers safety feedback when the player violates encounter protocol (sudden movement, direct approach)
- **Safety training cutscene** — Unity Timeline sequence that plays at game mode start, demonstrating correct encounter behavior before the player takes control

### Transect Survey System
Extended the survey mechanics to support the newly modeled species:
- Wired species into the existing transect counting system
- Ensured survey data output matched real-world field data formats used in the industry

### Research Collaboration
Worked in Agile sprints with a Cal Poly marine biologist to validate:
- Species visual accuracy (coloration, scale, fin morphology)
- Behavioral plausibility (schooling patterns, depth ranges, reaction to diver presence)
- Survey methodology alignment with published transect protocols

---

## Tech Stack

| Layer | Technology |
|---|---|
| Game engine | Unity (C#) |
| 3D modeling | Blender |
| WebGL build | Unity WebGL target |
| VR support | WebXR / WebGL |
| Collaboration | Agile sprints, weekly marine biologist review |

---

## Impact

- Deployed for **K-12 classroom use** — students experience ocean science without needing access to open water
- Used for **professional surveyor onboarding** — companies including Microsoft have used the simulation for environmental survey training
- Backed by **National Science Foundation** research funding

---

## Research Context

Underwater transect surveys are the standard method for marine population assessment. Surveyors swim a defined corridor (the "transect") and count species they observe within a fixed distance on either side. This simulation replicates that methodology in VR, allowing repeatable practice without the cost or logistics of open-water dives.

The Shark Dive mode addresses a real safety gap: most divers receive no formal training on shark encounter protocol before their first open-water dive.
