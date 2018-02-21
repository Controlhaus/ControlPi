# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).

## [Unreleased]  -
### Added

### Changed

## [1.1.0]  - 2018-02-21
### Added
- Enabled Video Output
- Added ControlPi Config running at startup on port 12345

### Changed
- Changed OS to Raspbian Stretch Lite

## [0.3.0]  - 2017-12-06
### Added
- Set up LIRC to use GPIO-06 31 as an IR output and GPIO-05 29 as an IR input (IR input not tested).
- node-red-contrib-lirc. To use LIRC with Node-RED.
- Sample Apple TV IR driver.
- Sample NodeRED flow. Shows how to use GPIO-06 31 as an infrared output.

## [0.2.0]  - 2017-12-04
### Added
- Default to DHCP for ethernet adapter eth1.
- RPi.GPIO 0.6.3. To control the GPIO ports.
- Sample NodeRED flow. Shows how to toggle a GPIO pin as a digital output.
- Sample NodeRED flow. Shows how to read a GPIO pin as a digital input.

### Changed
- Set Node-Red to run as root (so it can use the GPIO ports).
- Edited /home/avprogrammer/.node-red/settings.js to include the following (So user avprogrammer still has access to flows and directories while Node-Red is run as root. Otherwise these items would become inaccessible in the root directory.):
flowFile: '/home/avprogrammer/.node-red/flows.json',
userDir: '/home/avprogrammer/.node-red/',
nodesDir: '/home/avprogrammer/.node-red/nodes',

## [0.1.0] - 2017-11-29
### Added
- Minibian 2015-11-12 with Raspbian GNU/Linux 8 (jessie). A Raspbian operating system image without the overhead.
- raspi-config. Needed to expand the size of the files system on the SD card. Could be useful for other tasks as well.
- GNU nano. To edit text files.
- sudo 1.8.10p3. To access the root user.
- NPM 3.10.10. To install packages.
- curl 7.38.0. Used to install Node.js and NodeRED. Could be useful for other tasks as well.
- Node.js v6.12.0. To run Node-RED.
- Node-RED v0.17.5. To program automation and control projects.
- Set Node-RED to automatically start when Raspbian boots.
- Node-RED Dashboard 2.6.2. To create simple user interface web pages.
- Sample NodeRED flow. Shows how to send an iOS push notification with Open App (http://getopenapp.com). Browse to controlpi:1880 to give it a try.
- LIRC 0.9.0-pre1. To control devices with infrared using the built-in GPIO. Package is installed but not set up yet.
- Added default user: avprogrammer with password: takebackcontrol
- Enabled SSH.
- Enabled DHCP.

[0.3.0]: https://drive.google.com/file/d/1pvJX5tlXPAyqEBm5hWdl4LEmcw49MMo4/view?usp=sharing
[0.1.0]: https://drive.google.com/open?id=1iw3-s6GG7UDD8edw0WkQrZthd2odlugE

