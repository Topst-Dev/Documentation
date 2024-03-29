#  Booting Guide

This chapter describes how to boot the TOPST D3 and log in to the for each core.

## 1.1 Booting Sequence

The download sequence of ***FWDN*** is as follows:

1. Connect the DP cable for the DP monitor.
2. Connect the debugging board and the TOPST D3.
3. Connect each TOPST USB cable to the debugging board to log in to the console and perform debugging for each core.
4. Connect the 5V Power.

## 1.2 TOPST Connection with UART

To perform USB debugging and develop Linux environment, you can access the respective core (CA72/CA53/MCU) by using the TOPST debugging board shown below.

<br><div align="center">
    <img src="https://github.com/Topst-Dev/Documentation/assets/16188136/459f6a91-8358-4818-9bab-e8ccf2933521" alt="Figure 1.1 TOPST Debugging Board" width="350" height="250">
    <p><strong>Figure 1.1 TOPST Debugging Board</strong></p>
</div><br>

Install the UART Bridge VCP driver (found on https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers?tab=downloads) on the host PC.

Afterwards, when you , the CP210x USB to UART driver is set up as follows.

<br><div align="center">
    <img src="https://github.com/Topst-Dev/Documentation/assets/16188136/9e5444c8-2990-4d93-99ae-71740d5284e4" alt="Figure 1.1 TOPST Debugging Board">
    <p><strong>Figure 1.2 USB Connection in Windows Environment</strong></p>
</div><br>

Connect each UART port by using the terminal emulator on the host PC. Shown below is the log screen that was booted by connecting to the main core, sub-core, and MCU core. (**Example**: Terminal emulator: PuTTY or mobaXterm, Speed: 115200 bps, Data bits: 8, Parity: None, Stop bits: 1, Flow Control: None)

<br><div align="center">
    <img src="https://github.com/Topst-Dev/Documentation/assets/161264431/eb38e963-ea0c-4453-b59a-d184293d488a" >
    <p><strong>Figure 1.3 Connected Screen for Main Core (ID and Password are root)</strong></p>
</div><br>

<br><div align="center">
    <img src="https://github.com/Topst-Dev/Documentation/assets/16188136/60909aba-3c0f-49d5-b622-9bdfd9073b85" alt="Figure 1.1 TOPST Debugging Board" >
    <p><strong>Figure 1.4 Connected Screen for Sub-core (ID and Password are root)</strong></p>
</div><br>

<br><div align="center">
    <img src="https://github.com/Topst-Dev/Documentation/assets/16188136/24ceb1f4-11bc-4bea-b8fa-2dc135001237" alt="Figure 1.1 TOPST Debugging Board" >
    <p><strong>Figure 1.5 Connected Screen for MCU Core</strong></p>
</div><br>

## 1.3 TOPST Connection with DP Port

When the firmware loads normally, Connect the DisplayPort cable to the monitor and TOPST D3 board. Then Ubuntu loads into the monitor as shown below. Ubuntu operates on the main core as described above.

<br><div align="center">
    <img src="https://github.com/Topst-Dev/Documentation/assets/16188136/0633a9c2-af8f-472e-97c3-26b34a5c5aa4" alt="Figure 1.1 TOPST Debugging Board" width="500" height="300">
    <p><strong>Figure 1.6 Ubuntu Launcher</strong></p>
</div><br>

## 1.4 Run Application on Ubuntu

Figure 1.7 shows a media file being played by using the VLC media player that is included in Ubuntu.

<br><div align="center">
    <img src="https://github.com/Topst-Dev/Documentation/assets/16188136/b145b759-2a52-471e-813a-7aa97fd88fd5" alt="Figure 1.1 TOPST Debugging Board" width="500" height="300">
    <p><strong>Figure 1.7 Running Multimedia Applications</strong></p>
</div><br>

