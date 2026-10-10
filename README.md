# StripeLAN for Raspberry Pi

StripeLAN is a browser-based control panel for compatible magnetic-card reader/programmer hardware connected to a Raspberry Pi.

The project provides a ready-to-use Raspberry Pi image with a local web interface. The system uses a read-only root filesystem and a separate writable data partition for settings, language packs, layouts, saved procedures and transmission logs.

## Features

- serial port configuration from the web panel
- manual command sending
- TX/RX/status transmission log with hexadecimal representation
- step-by-step procedure execution
- automatic waiting for controller responses before the next command
- optional guided mode with operator notes
- demo mode for first startup and offline testing
- installable JSON language packs
- configurable panel layout
- saved transmission logs and procedures
- web-based update mechanism
- power-off and reboot controls

## Public Edition

The Public Edition contains restricted functionality and is intended for evaluation, compatibility testing and authorised personal non-commercial use.

The image starts in demo mode by default. After saving serial port settings, the application can reconnect automatically on startup.

A separately issued Full Version upgrade enables the licensed functionality and may include an individual PDF license certificate.

## Downloads

Download the current Raspberry Pi image from the [Releases](../../releases) section:

- `StripeLAN-PUBLIC.7z` — compressed Raspberry Pi image
- `StripeLAN-PUBLIC.7z.sha256` — optional checksum file

Optional language packs are available in the `language-packs/` directory.

## First Startup

1. Download `StripeLAN-PUBLIC.7z`.
2. Extract the `.img` file.
3. Write the image to a microSD card using Raspberry Pi Imager or a comparable tool.
4. Insert the card into the Raspberry Pi.
5. Connect the reader/programmer hardware.
6. Start the Raspberry Pi.
7. Open the web panel in a browser:

   `http://<raspberry-pi-ip>:8080`

8. Configure and save the serial port settings if real hardware is connected.

## Full Version Upgrade

The Full Version upgrade is individually issued to the licensee.

1. Start StripeLAN Public Edition.
2. Open the administration section in the web panel.
3. Select the issued StripeLAN upgrade package.
4. Confirm the update.

The upgrade installs the Full Version and, where applicable, the issued PDF license certificate.

Do not publish or share an individually issued upgrade package: it may contain a recipient-specific license certificate.

## Hardware Notes

StripeLAN is intended for use with supported hardware connected through a serial interface.

The actual configuration depends on the reader model, its firmware, power supply and serial wiring. Compatibility should always be verified with the specific device before operational use.

The interface includes protocol options for MKW1PC, MKW-C11 and MMW. Support for a listed protocol does not guarantee compatibility with every hardware revision.

## Safety and Authorisation

Use this software only with hardware, cards and data that you own or are explicitly authorised to test.

Do not use StripeLAN for unauthorised access, copying, alteration or misuse of third-party magnetic cards or data.

## License

StripeLAN is proprietary software.

The Public Edition is provided under the included [LICENSE](LICENSE). Additional notices are available in [NOTICE](NOTICE).

The Full Version is available only under separately issued license terms.
