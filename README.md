# MPPD

Project MPPD: Modular Parallel-Pulse Disc Propulsion
1. Abstract & Disclosure
Date of Disclosure: February 1, 2026

Purpose: This document serves as a formal public disclosure of a novel propulsion system to establish Prior Art. This system utilizes a non-chassis, modular approach to electromagnetic transport, specifically bypassing the "internal force" paradox through a cascading parallel-control architecture.

2. System Architecture
The MPPD system is defined by three primary layers that decouple the load from the propulsion medium:

A. The Propulsion Module (The "Magnetic Gear")
Structure: A circular rotating housing containing a radial array of high-discharge electromagnets.

Mechanism: Instead of a central axle, the unit uses Leap-Frog Momentum. An internal controller fires magnetic pulses at the 6 o'clock position (contact point) to create a vector of repulsion against the surface or an internal traction rim.

Stabilization: The circular rotation provides gyroscopic stability for the platform above.

B. The Control Plane (Cascading Parallel Logic)
To eliminate switching latency and handle the high-frequency demands of magnetic pulsing, the system utilizes Distributed Parallel Processing:

Master Controller (L3): Manages high-level kinematics, rider balance (via IMU/PID loops), and directional vectoring.

Slave Controllers (L1/L2): Dedicated microcontrollers for each drive disc. Their sole function is the micro-timing of the magnetic pulses based on the angular velocity of the disc.

Communication: Real-time synchronization via I2C or CAN bus protocols.

C. The Shielded Platform
Interference Mitigation: A Mu-metal or carbon-composite shield is integrated between the drive units and the rider standing surface to contain magnetic flux and protect sensitive electronics.

3. Claimed Novelty
Software-Defined Propulsion: The elimination of mechanical gears in favor of code-timed magnetic pulses.

Decoupled Load: Moving away from a "vehicle body" to a "modular platform" where the rider is part of the stabilization loop.

Parallel Redundancy: Using cascading micro-brains to handle the "Back-EMF" and heat issues associated with high-speed magnetic switching.

4. Technical Implementation (Draft)
The system is designed to be built using off-the-shelf components to ensure democratic access to the technology:

Logic: Arduino/ESP32 Environment.

Switching: High-current MOSFET arrays with flyback diode protection.

Energy: High-C rating Lithium Polymer (LiPo) cells.
