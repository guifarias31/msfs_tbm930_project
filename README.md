# MSFS TBM 930 Project 0.6.0 (Continue project)

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
## Known Issues:

- (SU5 Issue) Taxi/Landing Light switch wrong definition. Use cockpit interaction.
- (SU5 Issue) Throttle lever left<->right position. Hold left mouse button, then click right mouse button.
- (Vanilla issue) Fuel consumption is increasing during climb, which is the opposite that should happen. It's lower than it should be at lower altitudes and higher than it should be at higher altitudes. That's not happening only on the TBM, and it's a vanilla MSFS issue. The fuel flow will match closely on cruise altitudes, and will be way lower on lower altitudes.

For any other suggestions or bug reports, feel free to contact us:
- [Discord](https://discord.gg/jzcaAv3dP6)
- [FlightSim.to](https://flightsim.to/profile/Mugz)
- [Forum](https://forums.flightsimulator.com/u/mixmugz)
## How to Install:

1: Click on the green button in the top right corner that says 'Code' and click "Download as ZIP" or download from Release page.

2: Unzip and put the folder "aircraft-tbm930-improvement" inside your MSFS Community folder

## How to Uninstall:

To uninstall just delete the folder "aircraft-tbm930-improvement" from your MSFS Community folder.

## Donation

If you want to support me, here's my donation link:

[![Donation](https://i.imgur.com/vQyI7N5.png)](https://www.buymeacoffee.com/mugz)

or [Buy Me a Beer](https://paypal.me/mixmugz) :)
