# 📊 Overview

The **Overview** section displays the robot’s live status across multiple subsystems using icons and labels. It refreshes automatically to reflect the most recent data from the system's `status.json` file.

### Indicators and Labels

- **Standby / Auto Scheduling**: Displays whether the robot is idle or operating on an automated schedule.
- **Recording**: Shows if the robot is recording video or capturing images. The recording type is also labeled.
- **Movement & Direction**: Indicates whether the robot is in motion and its current direction (e.g., forward or backward).
- **Station Info**: Displays the current station ID. If the robot is at its home base, it’s labeled `(Home)`.
- **Travelling Home**: Indicates if the robot is returning to its base station.

### System Health

- **System Space (GB)**: Available storage on the Raspberry Pi.
- **USB Space (GB)**: Available storage on the connected USB device.
- **Battery Charge (%)**: Current battery level.
- **Battery Voltage (V)**: Voltage reading from the battery.
- **Battery Current (A)**: Current draw.
- **System Temperature (C)**: CPU temperature of the Raspberry Pi.

Each metric is visually represented with a colour-coded circle (e.g., green for active, red for alerts).