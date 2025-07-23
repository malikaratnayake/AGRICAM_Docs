# AGRICAM Control

The **Operator** tab in the AGRICAM GUI provides a comprehensive interface for managing robot operations in the field. It allows operators to control the robot, preview camera feeds, download system logs, and override autonomous schedules as needed.

---

## Overview

The Operator tab is divided into three main sections:

- [📸 Camera Previews](#camera-previews)
- [📝 Robot Logs](#robot-logs)
- [⚙️ Robot Control Panel](#robot-control-panel)

---

## 📸 Camera Previews

This section enables manual preview of the robot's onboard cameras.

- **Primary Camera**: Captures a preview image from the main (front-facing) camera.
- **Secondary Camera**: Captures a preview image from the secondary camera.

> Note: Camera previews are disabled during active recording sessions to avoid conflicts.

---

## 📝 Robot Logs

These buttons allow the operator to download system logs for diagnostics or performance review:

- **Download Debug Log**: Downloads the main unit log (via 4G or local network).
- **Download Sensor Data Log**: Downloads environmental and positional sensor logs.

> For video and image data, physical SSD/Thumb Drive removal is required after shutting down the device.

---

## ⚙️ Robot Control Panel

This panel provides buttons to manage the robot’s current state. Below is a description of each action:

### PROGRAM
- Wakes up the device.
- Does **not** initiate any scheduled movement or monitoring.
- Useful for diagnostics or status checks.

### START (UN-PAUSE)
- Wakes up the robot if paused.
- Moves the robot to the **Home Station**.
- Waits for the next scheduled monitoring run to begin.

### PAUSE
- Immediately stops the robot in its current location.
- Puts the system to sleep.
- Active monitoring runs are aborted.
- Monitoring resumes upon next **START** command.

### ABORT
- Immediately ends the current monitoring run.
- Returns the robot to the **Home Station**.
- Automatically resumes scheduled monitoring from the next cycle.

### RETURN HOME
- Interrupts all activity and immediately commands the robot to return to **Home Station**.
- The unit remains idle upon arrival.

### REMOVE
- Commands the robot to return **Home**.
- Enters an auto-shutdown state for safe physical removal.

### SHUTDOWN
- Immediately stops all activity and shuts down the robot at its current location.
- Used when quick termination is needed.

### REBOOT
- Issues a shutdown followed by an automatic reboot of the device.

---

## Confirm Dialogs

For safety and redundancy, confirmation dialogs are shown before executing critical commands such as **Shutdown** and **Return Home**. This prevents accidental disruption of operations.

---

## Notes

- Camera previews are implemented using `libcamera-still`.
- Log files are downloaded from predefined storage paths.
- All control actions use event-driven signals handled by backend scripts.
- The Operator tab is especially useful in manual intervention scenarios or system recovery workflows.

This interface ensures that field operators can reliably control, diagnose, and interact with the AGRICAM system as needed.
