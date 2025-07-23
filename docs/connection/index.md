# Setup and Connection

!!! success "Already Connected to AGRICAM TailNet?"
    If you have already set up and connected to the AGRICAM TailNet, use the following links to access the robot dashboards. Remember, Tailscale must be active on your device.

    * **AGRICAM 2:** [http://agricam2:5000](http://100.78.160.3:5000)
    * **AGRICAM 4:** [http://agricam-4:1880/ui](http://agricam-4:1880/ui)

## Setup Guide

To ensure a secure and reliable connection to the AGRICAM robots from any location, we use **Tailscale**. Tailscale creates a private network (a "tailnet") that directly connects your devices to our robots, allowing you to access their control dashboards as if you were on the same local network.

This guide provides step-by-step instructions for setting up Tailscale and connecting to the AGRICAM network.

### Step 1: Install Tailscale & Create an Account

First, install the Tailscale application on the device you will use to control the robots (e.g., your smartphone, tablet, or computer).

1. **Download the application** for your specific device:

   * **iOS (iPhone/iPad):** [**Tailscale on the App Store**](https://apps.apple.com/us/app/tailscale/id1470499037)

   * **Android:** [**Tailscale on Google Play**](https://play.google.com/store/apps/details?id=com.tailscale.ipn)

   * **Desktop (Windows, macOS, Linux):** [**Tailscale Downloads Page**](https://tailscale.com/download)

2. **Launch the application** after installation.

3. **Log In to Create an Account.** You will be prompted to log in using an existing identity provider. Select your preferred service (**Google, Microsoft, Apple, or GitHub**) and follow the on-screen instructions to authorize Tailscale. This will create your Tailscale account.

> **\[IMAGE PLACEHOLDER\]**
> *A screenshot showing the Tailscale login screen with the different identity provider options would be beneficial here.*

### Step 2: Request Access to the AGRICAM Network

Once your account is created, you must request access to the secure network where the AGRICAM robots operate.

1. **Compose a new email** with the following details:

   * **To:** `malika.ratnayake@monash.edu`

   * **Subject:** `Tailscale Access Request for AGRICAM`

   * **Body:** Please state your full name, your role or reason for access, and importantly, the email address associated with your new Tailscale account.

You will receive a confirmation email once your account has been granted access to the tailnet.

### Step 3: Connect and Access the Robots

After receiving confirmation, you can connect to the network and access the robots.

1. **Open the Tailscale app** on your device.

2. **Activate the connection.** Ensure the main toggle switch shows the status as **"Active"**.

3. **Verify Access.** Once active, you will see the available devices on the network. Look for `agricam-2` and `agricam-4` in your list of machines.

> **\[IMAGE PLACEHOLDER\]**
> *A screenshot of the Tailscale app's main screen showing the list of connected machines, with `agricam-2` and `agricam-4` highlighted, would be useful here.*

4. **Access the Dashboards.** With Tailscale active, use the following links in your web browser to open the robot control interfaces.

   !!! note "Important"
   These links will only work when Tailscale is running and connected on your device.

   * **To access AGRICAM 2:** [**http://agricam-2:1880/ui**](http://agricam-2:1880/ui)

   * **To access AGRICAM 4:** [**http://agricam-4:1880/ui**](http://agricam-4:1880/ui)

You should now be able to view the Node-RED dashboard for each robot, where you can monitor status and control operations.