# USB Connection

ZEROPLUS Xbox One clone wireless controller

https://www.aliexpress.com/item/1005005272237715.html
https://www.aliexpress.com/item/1005005216325441.html

Presents itself as VID=0x045E PID=0x02EA (Xbox One S Controller).

Then after a moment reconnects as HID device with VID=0x0C12 PID=0x0F11 ("ZEROPLUS Controller").
HID report descriptor is malformed (seems cropped).

Recognized in Windows 10 as:

Hardware ID: USB\VID_0C12&PID_0F11&REV_0100

```
>pnputil /enum-interfaces /class {A5DCBF10-6530-11D2-901F-00C04FB951ED}

Interface Path:         \\?\USB#VID_0C12&PID_0F11#5&2108ad5d&0&8#{a5dcbf10-6530-11d2-901f-00c04fb951ed}
Interface Description:  Unknown
Interface Class GUID:   {a5dcbf10-6530-11d2-901f-00c04fb951ed}
Device Instance ID:     USB\VID_0C12&PID_0F11\5&2108ad5d&0&8
Interface Status:       Disabled

>pnputil /enum-devices /instanceid "USB\VID_0C12&PID_0F11\5&2108ad5d&0&8" /ids
Microsoft PnP Utility

Instance ID:                USB\VID_0C12&PID_0F11\5&2108ad5d&0&8
Device Description:         USB Input Device
Class Name:                 HIDClass
Class GUID:                 {745a17a0-74d3-11d0-b6fe-00a0c90f57da}
Manufacturer Name:          (Standard system devices)
Status:                     Disconnected
Driver Name:                input.inf
Hardware IDs:               USB\VID_0C12&PID_0F11&REV_0100
                            USB\VID_0C12&PID_0F11
Compatible IDs:             USB\Class_03&SubClass_00&Prot_00
                            USB\Class_03&SubClass_00
                            USB\Class_03
```

When connecting to Xbox One you can see error 0x82d60002 (Unauthorized acessory error).