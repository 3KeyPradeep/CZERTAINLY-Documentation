# Advanced menu

Advanced menu is used for advanced operations with CZERTAINLY Appliance. You can access it from [**Main menu**](./main-menu) by selecting **Advanced options**.

| Short&nbsp;name | Advanced&nbsp;menu&nbsp;item                         | Description                                                                                  |
|-----------------|------------------------------------------------------|----------------------------------------------------------------------------------------------|
| **u**pdate      | Update Operating System                              | This option updates CZERTAINLY Appliance by `apt update && apt upgrade` command.             |
| **r**emoveC     | [Remove CZERTAINLY](#remove-czertainly)              | This option removes CZERTAINLY Appliance by deleting namespace `czertainly` from Kubernetes. |
| **r**emove      | [Remove RKE2 & CZERTAINLY](#remove-rke2--czertainly) | This option removes RKE2 (Kubernetes) and CZERTAINLY Appliance.                              |
| **s**hell       | [Enter system shell](#enter-system-shell)            | You can enter system shell as `czertainly` user.                                             |
| **r**eboot      | Reboot system                                        | This option reboots CZERTAINLY Appliance by `shutdown -r now` command.                       |
| **s**hutdown    | Shutdown system                                      | This option shutdown CZERTAINLY Appliance by `shutdown -h now` command.                      |
| **e**xit        | [Exit advanced menu](./main-menu)                    | By selecting this option you can return to Main menu.                                        |

## Remove CZERTAINLY

Removing CZERTAINLY from appliance mainly means deleting `czertainly` namespace from Kubernetes. Purpose of this tasks is preparation step for CZERTAINLY re-installation.

This task preserves anything that was configured, including CZERTAINLY data which is stored in Postgres database.

## Remove RKE2 & CZERTAINLY

Removing RKE2 (Kubernetes) and CZERTAINLY might be useful when you change hostname or IP address of virtual appliance. This is preparation step for even deeper CZERTAINLY re-installation.

This task preserves anything that was configured, including CZERTAINLY data which is stored in Postgres database.

## Enter system shell

You can enter system shell as `czertainly` user. The user is in `sudo` group. You can do any administrative task you wish. Please be very careful.

:::warning System shell access
If you are not sure about the result of your operations on the system shell, consult it with the CZERTAINLY support team. It may happen that you will break the system and you will not be able to access it anymore.
:::

