### HID Gamepad Descriptors

This repo contains info on various game controlles.
USB dumps were made via [Wireshark](https://www.wireshark.org/).

HID descriptors were decoded via [RDD! HID Report Descriptor Decoder](https://sourceforge.net/projects/hidrdd/) tool:
```
"rexx" rd.rex -d -b -x -f "hid_report_descriptor.bin" -o "hid_report_descriptor.txt"
```

This info may be userfull for writing gamepad mappings for these controllers or making your own HID game controller.

![](photo.jpg)