# MSFS TBM 930 Project version 0.2 Beta
This is the improvement project for the MSFS default TBM 930.

Current features of this modification are:

**Removed the 30% gap between 0 and 30% throttle;**

tp_high_idle_throttle_pos = 0; throttle position of high idle (Percent)

**Ajusted ITT slightly;**

itt_peak_temperature = 1150

itt_tuning_constant = 2

**Ajusted autopilot maximum pitch (was 10, now 20).**

max_pitch = 20

**Corrected some numbers**

min_n1_for_starter_cutoff = 52 ; %

min_n2_for_starter_cutoff = 80 ; %

rated_shaft_hp = 850

n1_to_shaft_torque_table = ... 68:0.12 ...

**Corrected torque vs air density (by PositiveZero)**

density_on_torque_table=0.000737:0.141, 0.000889:0.188, 0.001065:.241, 0.001267:.316, 0.001496:.42, 0.001755:.55, 0.002048:.72, 0.002377:.965

**Landing gear creates more drag (by PositiveZero)**

drag_coef_gear = 0.04700

**How to install:**

1: Click on the green button in the top right corner that says 'Code' and click "Download as ZIP"

2: Unzip and put the folder "aircraft-tbm930-performance" in your MSFS Community folder

For more liveries see this thread: https://forums.flightsimulator.com/t/turboprop-master-livery-list/168196/16
