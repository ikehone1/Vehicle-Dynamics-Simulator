# Vehicle Dynamics Simulator

This repository contains a series of vehicle dynamics models developed to study
vertical ride dynamics, suspension behavior, and pitch motion using numerical
integration (RK4).

The project progresses from a basic dynamics models involving friction and Euler's method of integration to a quarter-car model 
and a half car model, with an emphasis on understanding physical modeling assumptions, numerical stability,
and vehicle response to road inputs.

---

## Models Included

### Quarter-Car Model
- 2 DOF vertical model (sprung + unsprung mass)
- Spring-damper suspension and tire stiffness
- Sinusoidal road input
- Solved using 4th-order Runge–Kutta (RK4)
- Outputs:
  - Sprung/unsprung displacement
  - Suspension travel
  - Tire deflection
  - Energy response

### Half-Car Model (In Progress)
- 4+ DOF model including pitch dynamics
- Front and rear suspension modeled independently
- Includes:
  - Pitch angle and angular velocity
  - Front/rear suspension deflection
  - Weight transfer effects
- Current focus:
  - Numerical stability
  - Validation of pitch inertia (Iyy)
  - Road input expansion (random profiles)

---

## Numerical Methods
- Explicit Runge–Kutta 4th order (RK4)
- State-space formulation
- Time-domain simulation

---

## Assumptions
- Linear springs and dampers
- Small-angle pitch approximation
- Rigid vehicle body
- No longitudinal dynamics (vertical only)

---

## Roadmap / Future Work
- Researching implicit integration methods to utilize
- Random road profile generation
- Crash / flip condition detection using pitch thresholds
- Energy validation and damping verification
- Migration from notebooks to modular Python files
- Visualization improvements

---

## Motivation
This project was created as a self-directed learning exercise to strengthen
understanding of vehicle dynamics, numerical integration, and simulation-based
engineering analysis, with applications toward motorsports and automotive
engineering roles.

---

## Tools Used
- Python
- NumPy
- Matplotlib
- Google Colab

