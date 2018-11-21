NorthWalesTech SDR Workshop - Software Installation
===================================================

As part of the [INSPACE THREE event](https://www.meetup.com/NorthWalesTech/events/255567846/), there will be
a short workshop to help get people up and running with the RTL-SDR.

It would be helpful if software could be downloaded before hand to save faffing with the Pontio WiFi.

Any useful links / further info to come out of the workshop will be put here after the event.

Linux
-----

The following has been tested on Ubuntu 18.04:

```bash
sudo apt-get update
sudo apt-get install rtl-sdr gqrx-sdr gpredict cubicsdr librtlsdr-dev
sudo rmmod dvb_usb_rtl28xxu
git clone https://github.com/antirez/dump1090
echo 'blacklist dvb_usb_rtl28xxu' | sudo tee /etc/modprobe.d/blacklist-dvb_usb_rtl28xxu.conf
```

Windows / OS X
--------------

Please download [CubicSDR](https://github.com/cjcliffe/CubicSDR/releases/tag/0.2.4)

