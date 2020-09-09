# MSFS TBM 930 Project version 0.2 Beta
This is the improvement project for the MSFS default TBM 930.

Current features of this modification are:

**Removed the 30% gap between 0 and 30% throttle:**

tp_high_idle_throttle_pos = 0; *(default = 30)*

**Ajusted ITT slightly:**

itt_peak_temperature = 1150 *(default = 2100)*

itt_tuning_constant = 2 *(default = 1)*

**Ajusted autopilot maximum pitch:**

max_pitch = 15 *(default = 10)*

**Corrected some numbers:**

pitch_takeoff_ga = 10 *(default = 8)*

min_n1_for_starter_cutoff = 52 *(default = 50)*

min_n2_for_starter_cutoff = 80 *(default = 200)*

rated_shaft_hp = 850 (default = 0)

n1_to_shaft_torque_table = ... 68:0.12 ...

CG_aft_limit = 0.355 *(default = 0.36)*

rotation_speed_min = 80 *(default = 90)*

cruise_alt = 31000 *(default = 30000)*

best_glide = 120 *(default = 0)*

**Corrected torque vs air density (by [PositiveZero](https://forums.flightsimulator.com/u/positivezero/summary), modified by me):**

density_on_torque_table=0.000737:0.441, 0.000889:0.488, 0.001065:0.541, 0.001267:0.616, 0.001496:0.72, 0.001755:0.85, 0.002048:0.92, 0.002377:0.965

**Landing gear creates more drag (by [PositiveZero](https://forums.flightsimulator.com/u/positivezero/summary)):**

drag_coef_gear = 0.04700 *(default = 0.01000)*

## Known Issues:

- Inertial Separator is decreasing too much the torque (around 30%);

- Still testing fuel consumption.

## How to Install:

1: Click on the green button in the top right corner that says 'Code' and click "Download as ZIP"

2: Unzip and put the folder "aircraft-tbm930-performance" in your MSFS Community folder

For more liveries see this thread: https://forums.flightsimulator.com/t/turboprop-master-livery-list/168196/16
