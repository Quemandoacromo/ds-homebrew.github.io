# 卸载 Unlaunch

::: danger

**Installing or uninstalling Unlaunch may randomly brick your console! You have been warned!**

:::

**WARNING:** An uninstall of Unlaunch may brick your Nintendo DSi. 这里有一些关于您可能想要卸载Unlaunch，但并不需要卸载Unlaunch就可解决问题的例子。

- **The Unlaunch Background is scary:** [Reinstall Unlaunch](installing-unlaunch.html) using the new instructions. 它们现在包含关于如何改变背景的说明
- **I'm having an issue with Unlaunch or my console after installing it:** The [Troubleshooting](troubleshooting.html#unlaunch) page will explain how to fix many issues you may have

::: warning

减少变砖的几率， 请确保您的系统NAND中的没有安装任何非合法的 DSiWare(不包括HiyaCFW 提供的 SDNAND 重定向)， 或以其他方式篡改系统文件。

:::

::: warning

When uninstalling Unlaunch, you should **NOT** use its built-in uninstaller directly on your console as there is a chance that it will brick the console. Please see below for information on uninstalling it properly.

:::

Once you have reviewed the above information, follow the [Dumping NAND](dumping-nand.html) instructions to make a new NAND backup, then proceed to [Restoring a NAND Backup](restoring-nand.html). This will guide you through uninstalling Unlaunch from the NAND backup and flashing that to your console.

If you are not able to use no$gba or get an error after uninstalling Unlaunch in no$gba it is also possible to flash a NAND backup made prior to installing Unlaunch if you still have one, however it is recommended to try using a NAND backup that previously had Unlaunch first. This will make recovery significantly easier in the case of a brick requiring a hardmod as Unlaunch leaves the no$gba footer embedded in the NAND even when uninstalled.
