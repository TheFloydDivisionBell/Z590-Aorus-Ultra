OpenCore-0.8.2

SSDTS

[SSDT-AWAC.aml](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-AWAC.aml)
[SSDT-EC-USBX-DESKTOP.aml](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-EC-USBX-DESKTOP.aml)
[SSDT-PLUG-DRTNIA.aml](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-PLUG-DRTNIA.aml)
[SSDT-RHUB.aml](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-RHUB.aml)
SSDT-SBUS-MCHC.aml (Needs compiling manually but I took it from a similar Aorus build)

Drivers
HfsPlus.efi (Commit 16/01/2022)
OpenRuntime.efi (0.8.2)
OpenCanopy.efi

Kexts
Airportltlwm (v2.1.0_stable_Monterey)
[BlueToolFixup](https://github.com/acidanthera/BrcmPatchRAM) (2.6.3)
IntelBluetoothFirmware (v2.1.0)
IntelBluetoothInjector (v2.1.0) - DISABLED
Lilu (v.1.6.1)
USBInjectAll
USBMap (Needs building manually and bluetooth wont be enabled until this is mapped)
USBWakeFixup
VirtualSMC (v.1.3.0)
WhateverGreen (v.1.6.0)

Tools

[USB Map Tool](https://github.com/corpnewt/USBMap)