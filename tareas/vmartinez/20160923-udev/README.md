# Udev rules

I create an udev rule to execute a script when my personal USB is connected
or disconnected, I also modify an exercice done in class to get device
information from `/sys` directory.

The get the device information I use the following:
	udevadm info -a path -n /dev/sdb1 (actually /dev/sdb1 was the id assigned it can change)
	udevadm monitor --property

NOTE: the path of mDevice.sh, is in hardcode, I tested it on the course computer, so it must be change to another directory.
Soon I would like to add a makefile to fix some issues.
