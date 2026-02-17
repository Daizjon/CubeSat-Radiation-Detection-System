# CubeSat Radiation Detection System

A 1.5U CubeSat radiation detection system designed for space-based neutron and gamma detection applications. This project integrates scintillator-based sensing, custom power regulation, signal amplification, and thermal analysis within strict CubeSat power and size constraints.

---

## Project Overview

This CubeSat system was designed to operate within standard U-class spacecraft constraints (10×10×10 cm units). The 1.5U configuration integrates:

- Encapsulated 6LiInSe2 scintillator for neutron detection
- SiAPD / SiPM photodetection
- Custom power supply architecture (5V primary input)
- Preamplifier and shaper circuitry
- Micro-computer data acquisition system
- USB digital output interface

The CubeSat structure includes solar cells capable of delivering 5V × 1A per unit.

---

## System Architecture

### Sensor Module
- 6LiInSe2 scintillator crystal
- SiAPD / SiPM light detection
- Optical coupling and encapsulation
- Radiation-hardened considerations

### Signal Processing
- Preamplifier
- Shaper
- Multi-Channel Analyzer (MCA)
- External data acquisition and transmission

### Power Architecture
- 5V primary input
- Custom voltage regulation for:
  - -440V bias
  - +12V output
- Power budget limited to:
  - 5V × 1.5A (7.5W max for 1.5U configuration)

---

## Electrical Requirements

- All electronics operate on 5V input or regulated derivatives
- Total consumption < 5V × 1A per unit
- Radiation-hardened component considerations
- Controlled inrush current during power-up

---

## Power Testing Results

Extensive testing was performed under multiple operational states:

### Peak Current During Boot
- Inrush current up to 1.61A (brief spike)
- Mitigated via system optimization and startup reduction

### Operational Current
- Idle range: 0.55A – 0.7A
- Active data acquisition: 0.7A – 1.33A
- Peak operational: ~1.52A

System optimization included:
- OS cleanup
- Startup reduction
- Power profile tuning

---

## Thermal Analysis

Heat generation modeled using:

Q = m · c · ΔT

For a 1U equivalent mass:
- Max mass: 2 kg
- Specific heat capacity: 0.89 J/g°C
- Estimated temperature rise: ~10°C under sustained 5W load

Thermal analysis was critical due to the absence of convective cooling in space.

---

## Experimental Battery Test

System powered via 8000mAh battery:
- Runtime ≈ 6 hours
- Average current ≈ 1.33A

---

## Applications

- Space-based radiation monitoring
- Neutron detection research
- Compact satellite sensor systems
- Radiation-hardened embedded platforms

---

## Acknowledgment

Supported by the National Science Foundation under Grant #HRD-2112556
