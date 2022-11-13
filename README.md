# CIRCE_fault_database

Database of a real low voltage installation obtained using the PSCAD simulation program.

# Data structure:

- **CSV_CT802**: Raw data of a 2 millisecond test simulations (200 files) with the next collected data.
  - time [seg]
  - Prefault R [V]
  - Prefault S [V]
  - Prefault T [V]
  - Fault R [V]
  - Fault S [V]
  - Fault T [V]

Being **Prefault** the state of the electrical network before the fault at the injector location in volts, and **Fault** its state after the fault.

- **SimulationBriefing-200_CT802_24V**: 200 registers corresponding to each one of above simulations with the next data structured:
  - File number
  - Period [s]
  - AmpR [V]
  - AmpS [V]
  - AmpT [V]
  - Fault_type
  - R_fault [ohm]
  - Fault_dist [m]
  - Fault_time [us]

Being **AmpR**, **AmpS** and **AmpT** the corresponding amplitude of the injected pulse.
**R_fault** the fault impedance used.
And **Fault_dist** and **Fault_time**, the distance or time where the fault is happening.

[![DOI](https://zenodo.org/badge/565257241.svg)](https://zenodo.org/badge/latestdoi/565257241)
