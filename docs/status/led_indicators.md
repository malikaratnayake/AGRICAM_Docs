# AGRICAM LED Status Indicators

The AGRICAM robot uses two panels of three RGB LEDs each to provide a simple, visual summary of its operational state. These LEDs are grouped as follows:

- [AGRICAM LED Status Indicators](#agricam-led-status-indicators)
  - [Panel 1: System and Movement Status](#panel-1-system-and-movement-status)
  - [Panel 2: Recording and Scheduling](#panel-2-recording-and-scheduling)
  - [Notes](#notes)

Each LED uses distinct colours to convey information clearly and intuitively.

---

## Panel 1: System and Movement Status
This panel indicates standby status, robot movement, and overall system health.

| LED Index | Function | LED Colours |
|-----------|----------|--------------|
| 0 | Standby / Auto Scheduling | Green: Standby with schedule<br>Amber: Standby without schedule |
| 1 | Movement Status | Blue: Moving left<br>Magenta: Moving right<br>White: Stopped at station<br>Red: Stopped at home |
| 2 | System Health | Green: Normal<br>Amber: Warning<br>Red: Critical |

---

## Panel 2: Recording and Scheduling
This panel communicates the recording status, environmental data logging, and whether the robot is returning home.

| LED Index | Function | LED Colours |
|-----------|----------|--------------|
| 0 | Recording Mode | Red: Video recording<br>Amber: Timelapse<br>Magenta: Motion-based timelapse |
| 1 | Sensor Activity | White: Logging active<br>Amber: Shake detected |
| 2 | Travelling Home | Red: Returning to base |

---

## Notes
- Each panel corresponds to a dedicated RGB LED module on the robot.
- Colours are chosen for quick field-level interpretation.
- LEDs update automatically to reflect the robot’s real-time status.

This indicator system helps users understand AGRICAM's operation at a glance without needing additional displays or interfaces.