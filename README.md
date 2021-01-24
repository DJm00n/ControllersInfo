### HID Gamepad Descriptors

This repo contains info on various game controlles.
USB dumps were made via [Wireshark](https://www.wireshark.org/).

HID descriptors were decoded via [RDD! HID Report Descriptor Decoder](https://sourceforge.net/projects/hidrdd/) tool:
```
rexx rd.rex -d -b -x -f "hid_report_descriptor.bin" -o "hid_report_descriptor.txt"
```

This info may be userfull for writing gamepad mappings for these controllers or making your own HID game controller.

![](photo.jpg)

### Userfull links

- [Human Interface Devices (HID) Information at usb.org](https://www.usb.org/hid)
- [Device Class Definition for HID 1.11](https://www.usb.org/document-library/device-class-definition-hid-111)
- [HID Usage Tables 1.21](https://usb.org/document-library/hid-usage-tables-121)
- [Device Class Definition for PID 1.0](https://www.usb.org/document-library/device-class-definition-pid-10-0) (force feedback for joysticks, steering wheels, etc)
