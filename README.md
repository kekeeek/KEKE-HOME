<p align="center">
  <img src="icon.png" alt="KEKE HOME icon" width="110">
</p>

<h1 align="center">KEKE HOME</h1>

**KEKE HOME** is a modern PS4 homebrew dashboard designed to provide a clean, simple and useful interface for monitoring and managing a PS4.

It combines system monitoring, application management, controller testing, network information, settings and an automatic diagnostic tool in one place.

## Features

### 🏠 Dashboard
A modern dashboard with quick access to the main sections:

- **System**
- **Applications**
- **Tools**
- **Settings**

The interface is designed to stay clean and responsive while remaining easy to navigate with a PS4 controller.

### 🌡️ System Monitoring

The **System** section provides live hardware information, including:

- CPU / APU temperature
- SoC sensor temperatures when available
- Maximum detected temperature
- Fan duty percentage
- Internal storage capacity
- Free storage space
- Storage usage percentage
- Basic system information

Temperature states are shown directly next to the readings:

- **OK** — normal operating range
- **WARNING** — temperature is getting high and should be monitored
- **ALERT** — temperature is very high and should be checked

The exact sensor information available can depend on the PS4 model and firmware.

### 💾 Storage

KEKE HOME displays the internal storage information available to the application:

- Total capacity
- Free space
- Used space
- Percentage used

The application avoids guessing whether the physical drive is an HDD or SSD when the firmware does not expose enough information to make that determination reliably.

### 📱 Applications

The **Applications** section scans installed PS4 applications and displays:

- Application name
- Title ID / CUSA
- Application version
- Application icon

You can select an application and use the clearly indicated **OPTIONS — DELETE** action to remove it, with confirmation before deletion.

KEKE HOME protects itself from accidental self-deletion.

### 🎮 Joystick Test

The **Joystick** tool provides real-time visualization of both analog sticks.

The two stick indicators react to movement even before a test is started.

The automatic test is designed to make controller testing simple:

1. Keep the sticks untouched during the resting phase.
2. Move the left stick in circles when instructed.
3. Move the right stick in circles when instructed.
4. KEKE HOME evaluates the collected readings and reports whether drift was detected.

The test uses the controller's analog values rather than relying only on button states.

### 🌐 Network Information

The Network section displays information exposed by the PS4 network APIs, such as:

- Connection state
- Local IP address
- Netmask
- Gateway
- DNS information when available
- Interface information when available

Availability of individual fields may depend on the current network configuration and firmware.

### ⚙️ Settings

The Settings section contains interface preferences such as:

- Interface animations
- Temperature gauges
- Live data refresh
- High contrast mode
- About / application information

Settings are designed to persist between launches when supported by the current configuration.

### 🩺 Automatic Diagnostic

The **Diagnostic** tool performs an automatic health check without requiring an input between every step.

It checks:

- CPU / APU temperature
- SoC temperature information when available
- Fan information
- Internal storage
- Free storage space
- Storage usage

The test starts with **WAITING** states and only shows **OK** or **ERROR** after each check has actually completed.

At the end, KEKE HOME reports either:

- **DIAGNOSTIC PASSED**
- **DIAGNOSTIC COMPLETED WITH ERRORS**

The joystick test is intentionally kept separate from the automatic diagnostic.

## Compatibility

### Tested and working

- ✅ **PS4 firmware 9.00**
- ✅ **PS4 firmware 11.00**

### Expected to work

KEKE HOME is expected to work on other PS4 firmware versions supported by the OpenOrbis/homebrew environment, but those versions have **not been fully tested** by the KEKE HOME project.

> ⚠️ **Important:** Individual features, especially hardware monitoring and system information, may behave differently depending on the PS4 model and firmware. Compatibility with an untested firmware should not be considered guaranteed.

## Installation

1. Download the latest `KEKE HOME` `.pkg` from the GitHub Releases page.
2. Install the PKG using your normal PS4 homebrew workflow.
3. Launch **KEKE HOME** from the PS4 home screen.

No official Sony SDK is required to build the project; development uses the OpenOrbis homebrew toolchain.

## Controls

| Button | Action |
|---|---|
| D-Pad | Navigate |
| X | Select / Confirm |
| O | Back |
| OPTIONS | Application delete action when available |
| Touchpad / other inputs | Reserved for future features |

## Project Status

KEKE HOME is currently at the **4.x final release line**.

The current feature set is considered stable on the tested firmware versions.

Future improvements may include additional diagnostics, more system telemetry and further UI refinements.

## Screenshots

Screenshots and media will be added to this section as the project page is published.

## Credits

- **KEKE HOME** — application development
- **OpenOrbis** — PS4 homebrew toolchain
- PS4 homebrew community and open-source projects that made the development and testing possible

## Disclaimer

KEKE HOME is an independent homebrew project.

It is not affiliated with, endorsed by, or sponsored by Sony Interactive Entertainment.

Hardware information is presented only when it can be obtained reliably from the PS4 environment. The application intentionally avoids inventing sensor values when a firmware or hardware configuration does not expose them.

## License

License information will be added with the first public source release.
