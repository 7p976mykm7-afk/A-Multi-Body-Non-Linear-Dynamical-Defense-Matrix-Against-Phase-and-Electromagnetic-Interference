# Three-Body Chaotic Defense Matrix

An open-source, physical-layer security framework engineered to neutralize phase-spoofing, data-injection, and electromagnetic (EM) interference vectors using macroscopic non-linear resonators.

## Overview

Software-based cryptography remains vulnerable to physical-layer hardware injection and directed electromagnetic wave propagation. This repository provides the mathematical engine and hardware calibration blueprints for a physical defense matrix. 

By mapping the chaotic, non-harmonic, stick-slip acoustic profiles of micro-fractured resonators (such as cracked town bells) into a Circular Restricted Three-Body Problem (CR3BP) coordinate space, the system generates high-entropy, deterministic phase-scrambling fields. These fields blind external interception tracking while allowing authorized nodes to extract pristine data streams using geometric invariants.

## Repository Structure

* `/core/engine.py` - Non-dimensionalized analytical framework calculating effective potential gradients.
* `/hardware/calibration.py` - High-frequency piezoelectric data processing and active validation loop.
* `/docs/whitepaper.md` - Complete technical manifesto detailing proofs of Lyapunov divergence and Jacobi invariants.
* `LICENSE.md` - Licensed under the First-Principles Humanity Commons License.

## Mathematical Core

The system models the defense envelope inside a non-inertial reference frame rotating at structural velocity ($\omega$). The primary clashing masses of the fractured boundary serve as primary attractors ($m_1, m_2$), driving the coordinate transformation of the target phase vector ($x, y, z$):

$$\ddot{x} - 2\omega\dot{y} = \frac{\partial \Omega}{\partial x}$$
$$\ddot{y} + 2\omega\dot{x} = \frac{\partial \Omega}{\partial y}$$

Where the effective potential field is evaluated as:
$$\Omega(x, y, z) = \frac{1}{2}\omega^2(x^2 + y^2) + \frac{1-\mu}{r_1} + \frac{\mu}{r_2}$$

## Installation & Testing

The core engine is built strictly using dependencies-free standard mathematical libraries to ensure long-term firmware stability and compilation portability.

### Executing Local Verification Metrics
To initialize the validation matrix and test the stability of the Jacobi invariant ($C$) on a local terminal:

```bash
python core/engine.py
```

## Licensing

This project is permanently dedicated to the preservation of human infrastructure and the open availability of protective technology. It is published under the **First-Principles Humanity Commons License**, the text of which is located in the accompanying `LICENSE.md` file. Commercial or state monopolization of this defensive mathematical methodology is strictly prohibited.
