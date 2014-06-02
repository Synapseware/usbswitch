This file documents changes in the software, firmware and hardware of the
PowerSwitch device. New entries are always appended to the end of the file.
Scroll down to the bottom to see the most recent changes.


* Release 2005-02-07

- check error returns of libusb functions in commandline/powerSwitch.c
- clarification of section II of the liense
- WinAVR compatibility: do checksize in Makefile as last action because the
  Unix commands fail on Windows.
- WinAVR compatibility: add explicit file type for .S.o rule in Makefile.
- usbdrvasm.S: use a .+0 distance for nop2 macro

* Release 2005-02-20

- Added Pitfalls.txt file documenting common pitfalls.
- Updated usb-driver to new version (in separate directory).
- Use avrlibc init function for watchdog.

* Release 2005-04-18

- Updated usb-driver to new version

* Release 2005-06-14

- Use free shared USB IDs.
- Cleanup in commandline tool Makefile.
- Various improvements in the driver.

* Release 2006-01-31

- Fixed shared product ID in commandline tool.

* Release 2006-02-02

- Fixed usbGetStringAscii() in command line tool (returned random character
  at end of string).
- In usbdrv: New configuration variable to set the segment for USB rx buffer.
- In usbdrv: New configuration options for HIDs.

* Release 2006-02-07

- No changes, we just want to ship the newest driver version with PowerSwitch.

* Release 2006-02-20

- Added IAR compiler compatibility to USB driver (not the PowerSwitch project).
  Thanks to Oleg Semyonov for contributing this port!
- Major Bugfixes in the low level parts of the USB driver. See the driver's
  Changelog for details.

* Release 2006-03-14

- No changes, we just want to ship the newest driver version with PowerSwitch.

* Release 2006-03-26

- Use usb_get_busses() instead of the global usb_busses variable because
  Windows DLLs don't allow global variables from libraries across different
  compilers.

* Release 2006-06-26

- Switched to more general usbOpenDevice() function in commandline tool.

* Release 2006-07-18

- Distribute with GNU GPL2 license.
- Use avrdude instead of uisp as the default downloader.
- New AVR-USB version, see Changelog.txt in firmware/usbdrv/
- Ship with Windows executable and driver by default

* Release 2007-03-29

- Update to new driver.

* Release 2007-06-25

- Updated to new USB driver from 2007-07-07

* Release 2007-07-19

- Update to new driver.
- Use usbRequest_t structure in usbFunctionSetup().
- Fake USB disconnect during reset for at least 500 ms.

* Release 2007-08-07

- Update to newest driver 2007-09-19

* Release 2007-10-23

- Update to newest driver 2007-12-01

* Release 2007-12-01

- Use new usbDeviceDisconnect() and usbDeviceConnect() macros.
- Update to newest driver 2008-01-21.

* Release 2008-01-21

- Updated to newest driver.

* Release 2008-02-05

- Use functions from avr/eeprom.h instead of our own functions. This makes
  the code more portable.
- Updated to newest driver 2008-02-16

* Release 2008-02-16

- Updated to newest driver.

* Release 2008-02-28
