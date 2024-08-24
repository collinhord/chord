# Nintendo Switch (Unpatched) Jailbreak Guide

Welcome to the guide for operating a Nintendo Switch that has been jailbroken and modded with custom firmware. Please follow the steps carefully to ensure proper functionality and minimize the risk of damaging your device.

## Overview
This guide covers:
- Entering Recovery Mode using an RCM Jig.
- Injecting the Hekate bootloader payload.
- Booting custom firmware Atmosphere on the emuMMC partition.
- Accessing and operating homebrew applications.

### Prerequisites
Before proceeding, ensure you have:
- An unpatched Nintendo Switch.
- A computer with internet access.
- An RCM Jig.
- A USB-C cable.

## Note on Device Reboot
When the Nintendo Switch powers off, it will automatically boot into the sysNAND partition running the official Nintendo firmware, which has no applications installed. To access the Atmosphere custom firmware:
1. **Re-enter Recovery Mode** using the RCM Jig.
2. **Inject the Hekate payload** as previously described to launch into Atmosphere.

## Entering Recovery Mode (RCM)
1. **Power off your Switch.**
2. **Remove the Joy-Cons.**
3. **Slide the RCM Jig into the right Joy-Con rail.**
4. Continue to hold the **Volume Up** button and press the **Power** button. Release both buttons once the screen remains black, indicating that the Switch is in Recovery Mode.

## Injecting the Hekate Payload
1. Download the latest release of the Fusee Payload Injector Interface from [GitHub here](https://github.com/nh-server/fusee-interfacee-tk/releases).
2. Download the latest release of the Hekate payload from [GitHub here](https://github.com/CTCaer/hekate/releases/tag/v6.2.0).
   - The file is 'hekate_ctcaer_6.2.0_Nyx_1.6.2_v4.zip'.
3. Launch the interface on your computer. It should display "Looking for Device..."
4. With the Switch in RCM Mode, connect it to your computer via a USB-C cable. The interface should update to "Device Found."
5. Browse and select the `hekate payload.bin` file within the interface.
6. Click **“Send Payload”** to initiate the bootloader on the Nintendo Switch.

## Booting Atmosphere from emuMMC
1. Once Hekate boots, navigate to **Launch**.
2. Select **emuMMC** as your desired partition.
3. **Enjoy** playing from a custom firmware environment!

## Running Homebrew Applications
The Nintendo Switch with Atmosphere supports running homebrew applications:
- While opening any album or game application, hold the **right trigger** button to access the Homebrew Menu.
- Homebrew apps can greatly extend the functionality of your Switch but should be used with caution to prevent instability or unintended behavior.

## Game Management
Games are primarily managed through **Tinfoil**, an application for browsing, installing, and uninstalling game backups. The program accesses servers that host game backups.
- With the shutdown of popular services like LiberaShop, the current alternative for accessing game backups is **Ghost**.
- **Attention:** Installing official software updates from unofficial sources can potentially brick your device due to compatibility issues. If you notice a software update not installing, it's likely because the Updates and DLCs are .XCI files and not .NSP. Either that, or the Code is "Unsigned" and doesn't match Nintendo's servers.

## Tinfoil Install Settings
You can control the software installation settings and permissions in Tinfoil's settings under the Options panel by navigating to the Install section. Here you have the option to:
- Install Unsigned Code
- Install Updates from XCI
- Install DLCs from XCI
The default settings are NO/FALSE, and I have no experience changing them, but if I were to experiment with them I would allow "Install Updates/DLCs from XCI" before Installing Unsigned Code.

## Safety and Online Play
- This environment configures settings to block communication with Nintendo servers, which means **online play is disabled**.
- This measure also reduces the risk of your device being permanently damaged or “bricked” when operating within the jailbroken environment.

**Disclaimer:** Modifying your device can void warranties and violate terms of service. Additionally, downloading games you do not own is illegal in many jurisdictions. This guide is for informational purposes only.

## Conclusion
Enjoy enhanced features on your Nintendo Switch with the flexibility of a custom firmware environment. Always use caution when downloading new software and keep your system's safety settings current to avoid conflicts or potential damages.
