# K8DDV's HF Station Manager — installers

Windows installers for **K8DDV's HF Station Manager**, a program for running a QRP-Labs QMX and/or a Yaesu FT-891 transceiver from the PC over CAT.  It covers radio control and setup, propagation forecasts for your own antennas, Winlink gateway ranking, US and Canadian callsign lookup, an off-grid map, and tools for optimizing your SSB signal.

**Radios:** QRP Labs QMX / QMX+ and Yaesu FT-891.
**Needs:** Windows 10 or 11, 64-bit.

This is a **beta** for a few testers.  The installers are on the [Releases](../../releases) page.

## How it was built

K8DDV's HF Station Manager was not "vibe coded": it was built over four months through an iterative process between a professional programmer and analyst (K8DDV) and Anthropic's Claude AI, with over 2,000 builds, each checked against an automated test suite, and extensive design and on-air testing sessions with real radios.

It works the way that a person would want it to work, not the way an AI thinks a person would want it to work.

## Which installer?

Click a name to download it (version 9.0.180 beta 8).  All three install the same program.  They differ only in which data comes with it:

| Installer | Size | Pick it if… |
|---|---|---|
| [`…_fcc-yes_tiles-yes_ants-all.exe`](https://github.com/jimdolson/hf-station-manager-releases/releases/download/v9.0.178-beta-7/K8DDVs_Station_Manager_Setup_9.0.180_fcc-yes_tiles-yes_ants-all.exe) | 1.16 GB | You want everything ready at first start, with no further downloads.  It includes the FCC and Canadian callsign database, the finished map, and the whole antenna library (6,050 patterns) for propagation forecasts. |
| [`…_fcc-no_tiles-no_ants-all.exe`](https://github.com/jimdolson/hf-station-manager-releases/releases/download/v9.0.178-beta-7/K8DDVs_Station_Manager_Setup_9.0.180_fcc-no_tiles-no_ants-all.exe) | 549 MB | You want the whole antenna library but a smaller download.  The program offers to download the FCC/Canadian database the first time it runs, then builds the map tiles itself, which takes a while. |
| [`…_fcc-no_tiles-no_ants-min.exe`](https://github.com/jimdolson/hf-station-manager-releases/releases/download/v9.0.178-beta-7/K8DDVs_Station_Manager_Setup_9.0.180_fcc-no_tiles-no_ants-min.exe) | 155 MB | You want the smallest download.  It offers the FCC/Canadian database on first run, then builds the map tiles itself, which takes a while.  It contains only dipoles and EFHW antennas at 20 ft in the antenna library. |

`ants-min` means the antenna library holds six antennas: 80, 40 and 20 m dipoles and end-fed half-waves, flat at 20 ft.

## Installing

1. Download one installer: click its name in the table above, or pick it from the [Releases](../../releases) page.
2. Run it.  The installer isn't code-signed, so Windows SmartScreen may say *"Windows protected your PC."*  Click **More info**, then **Run anyway**.
3. Start the program and follow the setup questions.

## Feedback

Please report problems and suggestions as an [Issue](../../issues) on this repository, or contact K8DDV directly.  With a problem report, please include the Debug Log from `%LOCALAPPDATA%\K8DDVs_HF_Station_Manager\logs`.
