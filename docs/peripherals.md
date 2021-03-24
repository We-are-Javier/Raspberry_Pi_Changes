## Correcting Laggy Peripheral Inputs

For the full guide on correcting the mouse: [Fix That Laggy Mouse](https://thepihut.com/blogs/raspberry-pi-tutorials/fix-that-laggy-wifi-mouse). I chose to use a modified command from this guide (see below).

### Correcting Mouse Interactivity Latency

1. Navigate to your boot directory in either the file explorer or by using command prompts.
2. open the `cmdline.txt` file using either `sudo nano /boot/cmdline.txt` or by using a text editor.
3. Add the following text to the end of the single line of text `usbhid.mousepoll=0`, mousepoll=0 uses the devices polling speed instead of manually setting one.
4. Save the file
5. Reboot the system

### Correcting Keyboard Interactivity Latency (for wireless bluetooth keyboard using USB dongle)

As a note this actually changes the USB port speed to 1.1 instead of 2.0. While it may seem counterintuitive it fixed an issue with keys "sticking" when typing because the device is using a bluetooth dongle to connect both mouse and keyboard.

1. Navigate to your boot directory in either the file explorer or by using command prompts.
2. open the `cmdline.txt` file using either `sudo nano /boot/cmdline.txt` or by using a text editor.
3. Add the following text to the end of the single line of text `dwc_otg.speed=1`
4. Save the file
5. Reboot the system
