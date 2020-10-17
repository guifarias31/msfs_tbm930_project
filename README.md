# MSFS TBM 930 Project 0.5.2
This is the improvement project for the MSFS default TBM 930.

I highly recommend using [Working-Title G3000](https://github.com/Working-Title-MSFS-Mods/fspackages) **OR** [GTC 580 Touchscreens-Restyled](https://github.com/StuTozer/G3000-Touchscreens-Restyled/) by [StuTozer](https://forums.flightsimulator.com/u/electrikkar/summary). They are not compatible with each other at the moment, but should be in the future.

For a guide on how to change your ATC callsign from "Daher" to "TBM", check [this topic](https://forums.flightsimulator.com/t/want-your-pilot-and-atc-to-call-you-tbm-instead-of-daher-heres-how/299603) from Uwajimaya.

And for liveries, see [this post](https://www.nexusmods.com/microsoftflightsimulator/mods/44) on NexusMods.

Current features of this modification are:

* **Removed the 30% gap between 0 and 30% throttle:**

tp_high_idle_throttle_pos = 0; *(default = 30)*

...so then I needed to ajust:

n1_to_shaft_torque_table = ... 68:0.12, 87:0.88 ... *(default = ... 68:0.09, 87:1.0)*

* **Ajusted autopilot maximum pitch:**

max_pitch = 15 *(default = 10)*

* **Corrected some numbers:**

pitch_takeoff_ga = 10 *(default = 8)*

min_n1_for_starter_cutoff = 52 *(default = 50)*

min_n2_for_starter_cutoff = 80 *(default = 200)*

rated_shaft_hp = 850 (default = 0)

CG_aft_limit = 0.355 *(default = 0.36)*

rotation_speed_min = 80 *(default = 90)*

cruise_alt = 31000 *(default = 30000)*

best_glide = 120 *(default = 0)*

* **Ajusted torque vs air density table:**

density_on_torque_table = 0.0005:0.01, 0.0006:0.4, 0.0007:0.5, 0.000850:0.7, 0.000950:0.745, 0.002378:1.000

(Calculated using POH Maximum Cruise Chart)

*(default = 0.0005:0.01, 0.0006:0.4, 0.0007:0.6, 0.0008:0.75,  0.0009:0.9,0.000975:1.0, 0.002378:1.000000)*

* **Landing gear creates more drag (by [PositiveZero](https://forums.flightsimulator.com/u/positivezero/summary)):**

drag_coef_gear = 0.04700 *(default = 0.01000)*

* **Fuel flow ajusted:**

fuel_flow_scalar = 0.72 *(default = 1.0)*

* **Added [Uwa’s light mod](https://github.com/Uwajimaya/FS2020) v1.06**

* **Added [dimmable G3000 panels](https://github.com/kaosfere/msfs-fixes/tree/master/fixes/tbm930_lighting_fix) by [kaosfere](https://github.com/kaosfere/)**

* **Added [Audible Alert Fixes](https://forums.flightsimulator.com/t/tbm-930-audible-alert-fixes-updated/278815) by [PositeZero](https://forums.flightsimulator.com/u/positivezero/summary)**

## Known Issues:

- (Vanilla issue) ITT is a big problem. Increasing it makes the engine overheat on the ground, and decreasing it makes it stays too low on cruise level. Asobo's cfg is very limited, so I decided not to make any chances on that for now;

- (Vanilla issue) Fuel consumption is increasing during climb, which is the opposite that should happen. It's lower than it should be at lower altitudes and higher than it should be at higher altuitudes. That's not happening only on the TBM, and it's a vanilla MSFS issue. The fuel flow will match closely on cruise altitudes, and will be way lower on lower altitudes.

For any other suggestions or bug reports, feel free to contact us:

Discord: [Guilherme Farias#9971](https://discordapp.com/channels/@me/207215431654572032) and [withinboredom#9657](https://discordapp.com/channels/@me/762021447962066944)

Forum: [GuiFarias31](https://forums.flightsimulator.com/u/guifarias31/summary) and [CastTrout888930](https://forums.flightsimulator.com/u/casttrout888930/summary)

## How to Install:

1: Click on the green button in the top right corner that says 'Code' and click "Download as ZIP"

2: Unzip and put the folder "aircraft-tbm930-improvement" inside your MSFS Community folder

## How to Uninstall:

To uninstall just delete the folder "aircraft-tbm930-improvement" from your MSFS Community folder.

## Donation

If you want to support me, here's my donation link:

[![Donation](https://i.imgur.com/vQyI7N5.png)](https://www.buymeacoffee.com/guifarias31)
