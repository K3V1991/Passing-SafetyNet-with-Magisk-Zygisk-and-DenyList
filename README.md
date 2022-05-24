<p align="center"><img src="https://i.ibb.co/Jzbngh8/Google-Play-Services.png" width="200"></a>
<h1 align="center"><b>Passing SafetyNet with Magisk's Zygisk and DenyList</b></h1>
<h4 align="center">Magisk 24 will no longer have Magisk Hide natively bundled with Magisk. 
Unless of course you use a Fork of Magisk from another Developer.
How do you pass SafetyNet without it?</h4>
<br />

<p align="center">
<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=HW8B98TVDLKWA" alt="Donate-PayPal"><img src="https://img.shields.io/badge/Donate-PayPal-blue"></a>
<a href="https://github.com/K3V1991/Donate-Crypto" alt="Donate-Crypto"><img src="https://img.shields.io/badge/Donate-Crypto-yellow"></a>
<hr>
<br />

## Prequisites:
* Magisk - [Github](https://github.com/topjohnwu/Magisk "Magisk")
* MagiskHide Props Module - [Magisk Modules Repo](https://github.com/Magisk-Modules-Repo/MagiskHidePropsConf "MagiskHidePropsConf")
* Terminal Emulator - [Google Play Store](https://play.google.com/store/apps/details?id=com.termux "Termux") or Terminal Emulator for Android - [Google Play Store](https://play.google.com/store/apps/details?id=jackpal.androidterm "Terminal Emulator") 
* SafetyNet Checker - [Google Play Store](https://play.google.com/store/apps/details?id=rikka.safetynetchecker "YASNAC") or SafetyNet Test - [Google Play Store](https://play.google.com/store/apps/details?id=org.freeandroidtools.safetynettest "SafetyNet Test")
<br />

## How-To:
1. Update to the latest Magisk.
2. Open Magisk > Settings > Enable Zygisk & Enable Enforce DenyList.
3. Now tap on Configure DenyList (Tap on the 3 Button Menu and enable "Show System Apps")
4. Now turn off your Internet Connections and enable Airplane Mode. Double check and ensure that Wifi is turned off after enabling Airplane Mode.
5. Configure DenyList for Google Play Store and Google Play Services and all the other Apps you need Root hidden from.
6. Go into the Phone's Settings > Apps > Clear Data of all the Apps you configured in the DenyList.
7. Install the MagiskHide Props Module and reboot.
8. Open Termux or Terminal Emulator and grant Root Permissions by typing in:
```
su
```
Now type in:
```
props
```
9. Enter the 4th Submenu and configure so that the:
```
ro.boot.verifiedbootstate & ro.boot.flashlocked
```
Says active like in the Screenshots.

10. Now Reboot.
11. After Boot, connect to the Internet, let the Phone sit idle for 5-10 Minutes and check SafetyNet Status. 
You should be passing both Basic Integrity and CtsProfile and Google Play Certification.
<br />

## Screenshots
<img src="https://i.ibb.co/7bKvCLV/Temux-su.jpg" width="250"></a>
<img src="https://i.ibb.co/Kq2m4GL/Termux-props.jpg" width="250"></a>
<img src="https://i.ibb.co/S6M7sq2/Magisk-Hide-Props-Config-Menu.jpg" width="250"></a>
<img src="https://i.ibb.co/Q91dcFh/Edit-Magisk-Hide-props.jpg" width="250"></a>
