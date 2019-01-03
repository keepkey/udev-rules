# UDEV Rules

On linux platforms, you'll need to install UDEV rules in order to allow
non-root users to communicate with the device.

```
$ curl -OL https://raw.githubusercontent.com/keepkey/udev-rules/master/51-usb-keepkey.rules
$ sudo mv 51-usb-keepkey.rules /usr/lib/udev/rules.d
$ sudo udevadm control --reload-rules
```

Then unplug & replug your device. You do not need to restart your mmachine.
