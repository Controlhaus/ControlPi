# ControlPi

ControlPi is a Raspberry Pi 3 image for automation and control of AV/IT and Smart Home Systems.
It is based on the Minibian image with tools like NodeRED pre-installed.

## Getting Started

1. Download (and unzip if needed) the latest image here:
  http://learnavprogramming.com/controlpi
2. Burn controlpi.img to an SD card (with a tool like https://etcher.io ).
3. Insert the SD card into a Raspberry Pi 3.
4. Connect power to the Raspberry Pi.
5. Connect the Raspberry Pi to a network with a DHCP server.
6. Connect via SSH
    ssh avprogrammer@controlpi
    password takebackcontrol
7. Enter read write mode by entering:
    rw↵
8. Change your password by entering:
    passwd↵
9. Browse to controlpi:1880 and create your automation and control project with NodeRED.
10. When done editing your project, go back to the SSH window and enter read only mode by entering:
    ro↵
11. Check out some of the tutorials and take control!
  https://learn.controlhaus.de/avit/controlpi-initial-release/

## Contributing
Please post any issues or feature requests to this repository.
Your feedback is the best way to improve this project.

## Built With
* [Raspbian](https://www.raspbian.org) - The operating system.
* [Minibian](https://minibianpi.wordpress.com) - The starting Raspbian image.
* [Raspi-config](https://www.raspberrypi.org/documentation/configuration/raspi-config.md) - Raspberry Pi configuration tool.
* [GNU nano](https://en.wikipedia.org/wiki/GNU_nano) - Text editor.
* [Sudo](https://en.wikipedia.org/wiki/Sudo) - Allows users to run programs as root.
* [Npm](https://github.com/npm/npm) - Node Package Manager.
* [curl](https://curl.haxx.se) - Library and command-line tool for transferring data using various protocols.
* [Node-RED](https://github.com/node-red/node-red) - A visual tool for wiring the Internet of Things.
* [Node-RED Dashboard](https://github.com/node-red/node-red-dashboard) - A dashboard UI for Node-RED.
* [RPi.GPIO](https://pypi.python.org/pypi/RPi.GPIO) - A module to control Raspberry Pi GPIO channels.
* [LIRC](http://www.lirc.org) - A package that allows you to decode and send infra-red signals of many (but not all) commonly used remote controls.
* [node-red-contrib-lirc](https://github.com/estbeetoo/node-red-contrib-lirc) - LIRC nodes for node-red.

## Authors

* **Patrick Murray** - [Controlhaus](https://github.com/Controlhaus)

## License

This project is licensed under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Acknowledgments

* Thanks to the Raspberry Pi Foundation for the excellent hardware and software.
* Thanks to Charles-Henri Hallard for this article: http://hallard.me/raspberry-pi-read-only/
* Thanks to the Node-RED team and all the node-red-contributors.
* Extra special thank you for all the feedback and encouragement of my fellow AV programmers.
