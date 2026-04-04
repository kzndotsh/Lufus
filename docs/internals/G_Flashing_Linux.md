# Flashing Linux

When the specified ISO is found to be a non-Windows/Linux ISO, `dd` is used for flashing under the hood.
The exact command used here is:
```
dd if={iso_path} of={raw_device} bs=4M status=progress conv=fsync oflag=direct
```
