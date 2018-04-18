# ControlPi

ControlPi is a Raspberry Pi 3 image for automation and control of AV/IT and Smart Home Systems.
It is based on the Raspbian Stretch Lite image with tools like NodeRED pre-installed.

## Getting Started

1. Download (and unzip if needed) the latest image here:
	https://s3.amazonaws.com/controlpi/ControlPi-1.3.0.img.zip
2. Burn controlpi.img to an SD card (with a tool like https://etcher.io ).
3. Insert the SD card into a Raspberry Pi 3.
4. Connect power to the Raspberry Pi.
5. Connect the Raspberry Pi to a network with a DHCP server.
6. Connect via SSH
    ssh pi@raspberrypi
    password raspberry
7. Enter read write mode by entering:
    rw↵
8. Change your password by entering:
    passwd↵
9. Browse to raspberrypi:1880 and create your automation and control project with NodeRED.
10. When done editing your project, go back to the SSH window and enter read only mode by entering:
    ro↵
11. To change the default web page shown on the HDMI output, use SSH to edit /home/pi/start.sh with:
	nano start.sh
12. Check out some of the tutorials and take control!
  https://learn.controlhaus.de/avit/controlpi-initial-release/
13. To use ControlPi Config instead of SSH, browse to raspberrypi:12345

## Contributing
Please post any issues or feature requests to this repository.
Your feedback is the best way to improve this project.

## Built With
* [Raspbian](https://www.raspbian.org) - The operating system.
* [Npm](https://github.com/npm/npm) - Node Package Manager.
* [Node-RED](https://github.com/node-red/node-red) - A visual tool for wiring the Internet of Things.
* [Node-RED Dashboard](https://github.com/node-red/node-red-dashboard) - A dashboard UI for Node-RED.
* [RPi.GPIO](https://pypi.python.org/pypi/RPi.GPIO) - A module to control Raspberry Pi GPIO channels.
* [LIRC](http://www.lirc.org) - A package that allows you to decode and send infra-red signals of many (but not all) commonly used remote controls.
* [node-red-contrib-lirc](https://github.com/estbeetoo/node-red-contrib-lirc) - LIRC nodes for node-red.

## Authors

* **Patrick Murray** - [Controlhaus](https://github.com/Controlhaus)
* **Matteo Mattei** - (http://www.matteomattei.com)

## License

This project is licensed under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Acknowledgments

* Thanks to the Raspberry Pi Foundation for the excellent hardware and software.
* Thanks Matteo Mattei for all your help! http://www.matteomattei.com
* Thanks to Charles-Henri Hallard for this article: http://hallard.me/raspberry-pi-read-only/
* Thanks to the Node-RED team and all the node-red-contributors.
* Extra special thank you for all the feedback and encouragement of my fellow AV programmers.
