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

[Human Interface Devices (HID) Information from usb.org](https://www.usb.org/hid):

- [Device Class Definition for HID 1.11](https://www.usb.org/document-library/device-class-definition-hid-111)
> The Device Class Definition for HID 1.11 is intended to supplement the USB Specification and provide HID manufacturers with the information necessary to build USB-compatible devices. It also specifies how the HID class driver should extract data from USB devices. The primary and underlying goals of the HID class definition are to:
> - be as compact as possible to save device data space
> - allow the software application to skip unknown information
> - be extensible and robust
> - support nesting and collections
> - be self-describing to allow generic software applications

- [HID Usage Tables 1.21](https://usb.org/document-library/hid-usage-tables-121)
> The HID Usage Tables 1.21 document defines constants that can be interpreted by an application to identify the purpose and meaning of a data field in a HID report.
> Usages are also used to define the meaning of groups of related data items. This is accomplished by the hierarchical assignment of usage information to collections.
> Usages identify the purpose of a collection and the items it contains. Each Input, Output, Feature, and/or Collection data item within a Collection item can be assigned a purpose with its own usage item. Usages assigned to a collection apply to the items within the collection.
- [Device Class Definition for PID 1.0](https://www.usb.org/document-library/device-class-definition-pid-10-0)
> The Device Class Definition For Pid 1.0 Provides Information For The Development Of Physical Interface Devices. These Devices Include Force Feedback Joysticks, Steering Wheels, Etc. It Allows Peripheral And Driver Developers To Use A Common Set Of Hid Report Descriptors, Device Usages And Reports To Describe The Characteristics Of A Pid Class Device.

[Bluetooth Profiles Specifications from bluetooth.com](https://www.bluetooth.com/specifications/profiles-overview/):

- [Bluetooth Human Interface Device (HID) Profile 1.1.1](https://www.bluetooth.org/docman/handlers/downloaddoc.ashx?doc_id=309012)
> This profile defines how devices with Bluetooth wireless communications can use the HID Specification initially to discover the feature set of a Bluetooth HID device, and then communicate with the Bluetooth HID device. This profile further defines how a device with Bluetooth wireless communications can support HID services over the Bluetooth protocol stack using the Logical Link Control and Adaptation Protocol (L2CAP) layer.
- [HID Service (HIDS) 1.0](https://www.bluetooth.org/docman/handlers/downloaddoc.ashx?doc_id=245140) 
> This service exposes HID reports and other HID data intended for HID Hosts and HID Devices.
- [HID over GATT Profile (HOGP) 1.0](https://www.bluetooth.org/docman/handlers/downloaddoc.ashx?doc_id=245141)
> This profile defines how a device with Bluetooth low energy wireless communications can support HID services over the Bluetooth low energy protocol stack using the Generic Attribute Profile.
