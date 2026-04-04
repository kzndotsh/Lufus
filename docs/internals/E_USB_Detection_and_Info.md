# USB Detection and Info
Autodetection is done by the `UsbMonitor` class defined in the `src/lufus/drives/autodetect_usb.py` file.

It works by using `pyudev`, a Python binding for `libudev`, to scan block devices for USB devices on start,
as well as watching for hotplug events. The detected devices are then added to the dropdown menu in the GUI.
