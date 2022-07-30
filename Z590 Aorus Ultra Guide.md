# Z590 Aorus Ultra + i5-11600K + AMD 6600 XT OpenCore

## Hardware

| Component     | Details                                                                             |
| ------------- | ----------------------------------------------------------------------------------- |
| CPU           | Intel i5-11600K (Rocket Lake)                                                       |
| Motherboard   | Gigabyte Z590 Aorus Ultra ATX for LGA 1200                                          |
| GFX           | AMD 6600 XT Sapphire Pulse                                                          |
| RAM           | Corsair CMK16GX4M2B3000C15 Vengeance LPX 16 GB (2 x 8 GB) DDR4 3000 MHz C15 XMP 2.0 |
| PSU           | Corsair RM650x 80 Plus Gold 650 W                                                   |
| Case          | Corsair 4000D Airflow Mid-Tower ATX                                                 |
| LAN           | i225-V (onboard Intel 2.5GbE LAN)                                                   |
| WiFi          | Intel Wi-Fi 6 AX200 (onboard)                                                       |
| Audio         | Realtek® ALC4080 codec                                                              |
| Storage       | Sabrent 512GB Rocket NVMe PCIe M.2 2280                                             |


## Introduction

I was previously running a Z390i Aorus Pro WiFi with the i5-9600K which worked extremely well. I wanted to upgrade to a newer gen board and try to make use of my old Apple Thunderbolt display so I'm currently waiting for an Alpine Ridge Thunderbolt expansion card to arrive so that I can flash it and attempt to get it working. If it turns out to not be possible I will just sell the display and continue to use my MSI MAG274QRF-QD which works perfectly and I would personally recommend.

This is only my second hackintosh and is at the time of writing this guide only 2 days old so there's a lot to improve but I thought I would write it up so far as there are no guides for this specific motherboard from what I can find.

## OpenCore-0.8.2 - Monterey

## SSDTS

<a href="https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-AWAC.aml" target="_blank">SSDT-AWAC.aml</a>

<a href="https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-EC-USBX-DESKTOP.aml" target="_blank">SSDT-EC-USBX-DESKTOP.aml</a>

<a href="https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-PLUG-DRTNIA.aml" target="_blank">SSDT-PLUG-DRTNIA.aml</a>

<a href="https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-RHUB.aml" target="_blank">SSDT-RHUB.aml</a>

SSDT-SBUS-MCHC.aml (Needs compiling manually but I took it from a similar Aorus build)

## Drivers
HfsPlus.efi (Commit 16/01/2022)
OpenRuntime.efi (0.8.2)
OpenCanopy.efi

## Kexts
Airportltlwm (v2.1.0_stable_Monterey)

<a href="https://github.com/acidanthera/BrcmPatchRAM" target="_blank">BlueToolFixup (2.6.3)</a>

IntelBluetoothFirmware (v2.1.0)

IntelBluetoothInjector (v2.1.0) - DISABLED

Lilu (v.1.6.1)

USBInjectAll

USBMap (Needs building manually and bluetooth wont be enabled until this is mapped)

<a href="https://github.com/osy/USBWakeFixup" target="_blank">USBWakeFixup</a>

VirtualSMC (v.1.3.0)

WhateverGreen (v.1.6.0)

## Tools

<a href="https://github.com/corpnewt/USBMap" target="_blank">USB Map Tool</a>

## Sources

I realise this link may not work forever but at the moment its the only decent source.

<a href="https://github.com/dortania/OpenCore-Install-Guide/pull/343">Add Rocket Lake Support PR - OpenCore-Install-Guide</a>

DISCLAIMER: This EFI does not work for my specific build!!! It crashes at the recovery Apple logo but can be used to borrow files from if necessary.

<a href="https://github.com/nickw444/opencore-efi-z590">nickw444's Gigabyte Z590 Aorus Elite Monterey Hackintosh</a>