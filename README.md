# PiracyTools

## Description
ADB automation utility to simplify module usage for advancing interactions with an android device.

## Objective
The main objective of this module is to allow advanced use of Android Debug Bridge and certain modules available for android for reverse engineering. The installation and the use of the modules is automated in the script by the appropriate commands generating the read/write permissions necessary for the use of these. Below is a list of commands and descriptions for each module.


## Modules
<details><summary>Frida</summary>

> https://frida.re/  
> Dynamic instrumentation toolkit for developers, reverse-engineers, and security researchers.

| Command                                  | Permission | Description                                              |
|:----------------------------------------:|:----------:|:--------------------------------------------------------:|
| `ptools frida status`                    | shell      | Show frida status                                        |
| `ptools frida install server`            | root       | Install frida server                                     |
| `ptools frida install pip`               | root       | Install frida pip                                        |
| `ptools frida uninstall server`          | root       | Uninstall frida server                                   |
| `ptools frida uninstall pip`             | root       | Uninstall frida pip                                      |
| `ptools frida start`                     | root       | Start frida service                                      |
| `ptools frida stop`                      | root       | Stop frida service                                       |
| `ptools frida pinning $PACKAGE $VERSION` | root       | Bypass SSL pinning for an application                    |
| `ptools frida run $SCRIPT $PACKAGE`      | root       | Run a frida personal script                              |
| `ptools frida create`                    | shell      | Native and classic function interception script creation |
</details>

<details><summary>Advanced</summary>

> https://developer.android.com/studio/command-line/adb  
> Programming tool used for debugging Android-based devices.

| Command                  | Permission | Description                                   |
|:------------------------:|:----------:|:---------------------------------------------:|
| `ptools adv pkg`         | shell      | Application lists                             |
| `ptools adv pkg $NAME`   | shell      | Lists apps by name                            |
| `ptools adv wifi`        | root       | Wifi networks already connected with password |
| `ptools adv db $PACKAGE` | root       | SQLite3 database of an application            |
| `ptools adv switch`      | shell      | Change device without exit                    |
| `ptools adv root`        | shell      | Check root compatibility (CVE-2022-0847)      |
</details>

### Planned
- Any other suggestions

## Disclaimer
The use of these scripts for malicious purposes is under the responsibility of the user.

---
*This scripts are created by __hyugogirubato__.  
Find us on [discord](https://discord.com/invite/g6JzYbh) for more information on projects in development.*