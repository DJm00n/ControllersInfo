[Amazon Luna Controller Quick Start Guide](https://www.amazon.com/gp/help/customer/display.html?nodeId=GEHPAXCM8L39RQVG)

![image](https://m.media-amazon.com/images/G/01/support_images/GUID-91658BEA-83EC-424F-8241-56223B0B3CD8=3=en-US=Normal.png)

[What are the Buttons on the Amazon Luna Controller?](https://www.amazon.com/gp/help/customer/display.html?nodeId=GEKGVPKSY8B2RGHG)

To enter Bluetooth pairing mode hold **Action** (button with circle) + **B** for 3 seconds.

# Bluetooth LE Connection

Device Hardware ID `BTHLEDevice\{00001812-0000-1000-8000-00805f9b34fb}_Dev_VID&010171_PID&0419_REV&0100`

![image](https://user-images.githubusercontent.com/1285934/216942320-22d582fd-6688-46fa-8f28-ccf8f6fc6bb2.png)

![image](https://user-images.githubusercontent.com/1285934/216942474-ff5bf1a0-17d3-4e97-8801-bc3fa7a554ca.png)

There is [special filter driver](https://www.amazon.com/gp/help/customer/display.html?nodeId=GZCT4CTFHXLHEB9T) can be installed that adds XInput API when connected over Bluetooth.

# USB Connection

When connected over USB Luna controller can work in two modes: **XInput** (default) and **HID** (may be called DirectInput).

To switch between USB modes hold **Action** (button with circle) + **X** for 3 seconds while connected over USB.

## XInput Mode

Device Hardware ID `USB\VID_1949&PID_041A&REV_0101`

![image](https://user-images.githubusercontent.com/1285934/216943284-aa3baa4e-b4d0-4186-8e59-5d00abb615e4.png)

![image](https://user-images.githubusercontent.com/1285934/211622110-eea66f22-3549-41be-b54b-17930658a5bb.png)

## HID Mode

Device Hardware ID `USB\VID_1949&PID_0419&REV_0101`

![image](https://user-images.githubusercontent.com/1285934/216943145-8dbca3d3-1fde-47bb-9996-709a46cd088f.png)

![image](https://user-images.githubusercontent.com/1285934/211622172-4098d3a8-b550-4026-bd7b-f686ef41b069.png)
