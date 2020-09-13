# MSFS TBM 930 Project version 0.4.1
This is the improvement project for the MSFS default TBM 930.

And I suggest using the [msfs-navsystems-performance](https://github.com/Smirow/msfs-navsystems-performance) for G3000 extra funcionalities and performance.

Current features of this modification are:

**Removed the 30% gap between 0 and 30% throttle:**

tp_high_idle_throttle_pos = 0; *(default = 30)*

...so then I needed to ajust:

n1_to_shaft_torque_table = ... 68:0.12, 87:0.88 ...

**Ajusted autopilot maximum pitch:**

max_pitch = 15 *(default = 10)*

**Corrected some numbers:**

pitch_takeoff_ga = 10 *(default = 8)*

min_n1_for_starter_cutoff = 52 *(default = 50)*

min_n2_for_starter_cutoff = 80 *(default = 200)*

rated_shaft_hp = 850 (default = 0)

CG_aft_limit = 0.355 *(default = 0.36)*

rotation_speed_min = 80 *(default = 90)*

cruise_alt = 31000 *(default = 30000)*

best_glide = 120 *(default = 0)*

**Ajusted torque vs air density:**

density_on_torque_table = 0.0005:0.01, 0.0006:0.4, 0.0007:0.727, 0.000895:0.771, 0.001144:0.817, 0.001459:0.866, 0.001862:0.911, 0.002378:0.965

(Calculated using 5,6% decrease on torque every 21.63% decrease on density.)

*(default = 0.0005:0.01, 0.0006:0.4, 0.0007:0.6, 0.0008:0.75,  0.0009:0.9,0.000975:1.0, 0.002378:1.000000)*

**Landing gear creates more drag (by [PositiveZero](https://forums.flightsimulator.com/u/positivezero/summary)):**

drag_coef_gear = 0.04700 *(default = 0.01000)*

**Ajusted inertial separator decrease in torque to 3/4 (now 19%, instead of 25%):**

(L:XMLVAR_InertSep#ID#_Deployment) 12288 * (&gt;K:ANTI_ICE_GRADUAL_SET_ENG#ID#) (default = 16384)

**Added [Uwa’s lighting fix](https://github.com/Uwajimaya/FS2020) v1.1**

**Transponder now starts on Stand by when cold and dark**

**COM1, COM2 and ADF frequency changed when started cold and dark**

## Known Issues:

- ITT is a big problem. If I increase too much, it overheats on the ground, and if a decrease too much it stays too low on cruise level.

- Still testing fuel consumption. If you enconter any problems, let me know.

My Discord: Guilherme Farias#9971

My forum profile: [GuiFarias31](https://forums.flightsimulator.com/u/guifarias31/summary)

## How to Install:

1: Click on the green button in the top right corner that says 'Code' and click "Download as ZIP"

2: Unzip and put the folder "aircraft-tbm930-performance" in your MSFS Community folder

For more liveries see this thread: https://forums.flightsimulator.com/t/turboprop-master-livery-list/168196/16
