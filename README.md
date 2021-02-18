# MSFS TBM 930 Project 0.5.7 (Continue project)

This is the continue improvement project for the MSFS default TBM 930.

I highly recommend using [Working-Title G3000](https://github.com/Working-Title-MSFS-Mods/fspackages).

### Change ATC call sign to "TBM"
In the real world the TBM 930's ATC call sign is not "Daher" but "TBM". To change this:
1. Open in `<MSFS2020 Install Dir>\Official\OneStore\fs-base\en-US.locPak` in a text editor
2. Search for `"ATCCOM.ATC_NAME_DAHER.0.tts":`
3. Change `Daher` to `TBM`

```json
      "ATCCOM.ATC_NAME_DAHER.0.text": "TBM",
      "ATCCOM.ATC_NAME_DAHER.0.tts": "TBM",
```
**Note:** This will reset after every update of MSFS.

Current features of this modification are:

* **Removed the 30% gap between 0 and 30% throttle:**

tp_high_idle_throttle_pos = 0; *(default = 30)*

...so then I needed to ajust:

n1_to_shaft_torque_table = ... 68:0.12, 87:0.88 ... *(default = ... 68:0.09, 87:1.0)*

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

* **Added [Uwa’s light mod](https://github.com/Uwajimaya/FS2020) v1.08**

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

[![Donation](https://i.imgur.com/vQyI7N5.png)](https://paypal.me/mixmugz)
