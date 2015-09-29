# BLE Micro Development Environment

This image provides a development environment to build software for the [Seeed Studio's BLE Micro][1].

# How to

	docker run --rm -v <local path>:/home/dev/mbed_ble/app docker.io/skyplabs/ble-micro

The *local path* refers the folder on your host system which holds the source code of your application with a **Makefile**.

If you already are in this folder :

	docker run --rm -v $(pwd):/home/dev/mbed_ble/app docker.io/skyplabs/ble-micro

And if you want to specify a *target name* to **make** :

	docker run --rm -v $(pwd):/home/dev/mbed_ble/app docker.io/skyplabs/ble-micro <target name>

## License

[MIT][2]

 [1]: http://www.seeedstudio.com/depot/Seeed-Micro-BLE-Module-w-CortexM0-Based-nRF51822-SoC-p-1975.html
 [2]: http://opensource.org/licenses/MIT
