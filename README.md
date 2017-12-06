# A Simple Cellular Modem Test Project

This is a simple example of how to use resin.io base image when your device is connected via cellular modem. It includes some specific udev rules to ensure that the modem is not disconnected on container restart, update or reboot. Without these rules it is possible for the modem to get into an unrecoverable state.

This project also packages in the `mmcli` tool to check the modem and set AT commands to it. It currently just queries the modems signal strength every 1 minute and logs it to the dashboard.

This project will only work on resinOS 2.0 and greater.