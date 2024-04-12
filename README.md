<p align="center"><img src="https://github.com/K3V1991/Passing-SafetyNet-with-Magisk-Zygisk-and-DenyList/blob/main/Google-Play-Services.png" width="200"></a>
<h1 align="center"><b>Passing SafetyNet with Magisk's Zygisk and DenyList</b></h1>
<h4 align="center">Magisk 24 will no longer have Magisk Hide natively bundled with Magisk. 
Unless of course you use a Fork of Magisk from another Developer.
How do you pass SafetyNet without it?</h4>
<br />

<p align="center">
<a href="https://liberapay.com/K3V1991" alt="LiberaPay"><img src="https://img.shields.io/badge/Liberapay-F6C915?style=for-the-badge&logo=liberapay&logoColor=black" /></a>
<a href="https://www.buymeacoffee.com/k3v1991" alt="BuyMeACoffee"><img src="https://img.shields.io/badge/Buy%20Me%20a%20Coffee-ffdd00?style=for-the-badge&logo=buy-me-a-coffee&logoColor=black" /></a>
<a href="https://ko-fi.com/k3v1991" alt="Ko-fi"><img src="https://img.shields.io/badge/Ko--fi-F16061?style=for-the-badge&logo=ko-fi&logoColor=white" /></a>
<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=HW8B98TVDLKWA" alt="PayPal"><img src="https://img.shields.io/badge/PayPal-00457C?style=for-the-badge&logo=paypal&logoColor=white" /></a>
<a href="https://github.com/K3V1991/Donate-Crypto/blob/main/README.md" alt="Crypto"><img src="https://img.shields.io/badge/Bitcoin-000?style=for-the-badge&logo=bitcoin&logoColor=white" /></a>
</p>
<hr />
<br />

## Prequisites:
* Magisk - [Github](https://github.com/topjohnwu/Magisk "Magisk")
* MagiskHide Props Module - [Magisk Modules Repo](https://github.com/Magisk-Modules-Repo/MagiskHidePropsConf "MagiskHidePropsConf") **(Discuntinued)**, use Universal SafetyNet Fix - [GitHub](https://github.com/kdrag0n/safetynet-fix "Universal SafetyNet Fix")
* Termux - [Google Play Store](https://play.google.com/store/apps/details?id=com.termux "Termux") or Terminal Emulator for Android - [Google Play Store](https://play.google.com/store/apps/details?id=jackpal.androidterm "Terminal Emulator") 
* YASNAC - Yet Another SafetyNet Attestation Checker - [Google Play Store](https://play.google.com/store/apps/details?id=rikka.safetynetchecker "YASNAC") or SafetyNet Test - [Google Play Store](https://play.google.com/store/apps/details?id=org.freeandroidtools.safetynettest "SafetyNet Test")
<br />

## MagiskHide Props Module How-To:
1. Update to the latest Magisk.
2. Open ```Magisk``` > ```Settings``` > enable ```Zygisk``` & ```Enforce DenyList```.
3. Now tap on Configure DenyList (Tap on the 3 Button Menu and enable "Show System Apps")
4. Now turn off your Internet Connections and enable Airplane Mode. Double check and ensure that Wifi is turned off after enabling Airplane Mode.
5. Configure DenyList for Google Play Store and Google Play Services and all the other Apps you need Root hidden from.
6. Go into the Phone's ```Settings``` > ```Apps``` > ```Clear Data``` of all the Apps you configured in the DenyList.
7. Install the MagiskHide Props Module **(Discuntinued)** and reboot.
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
ro.boot.verifiedbootstate & ro.boot.flash:locked
```
Says active like in the Screenshots.

10. Now Reboot.
11. After Boot, connect to the Internet, let the Phone sit idle for 5-10 Minutes and check SafetyNet Status. 
You should be passing both Basic Integrity and CtsProfile and Google Play Certification.
<br />

## Universal SafetyNet Fix Module How-To:
1. Install Universal SafetyNet Fix Module and reboot.
You should be passing both Basic Integrity and CtsProfile and Google Play Certification.
<br />

## Screenshots
<img src="https://github.com/K3V1991/Passing-SafetyNet-with-Magisk-Zygisk-and-DenyList/blob/main/Temux-su.jpg" width="250"></a> &emsp;
<img src="https://github.com/K3V1991/Passing-SafetyNet-with-Magisk-Zygisk-and-DenyList/blob/main/Termux-props.jpg" width="250"></a> &emsp;
<img src="https://github.com/K3V1991/Passing-SafetyNet-with-Magisk-Zygisk-and-DenyList/blob/main/MagiskHide-Props-Config-Menu.jpg" width="250"></a> &emsp;
<img src="https://github.com/K3V1991/Passing-SafetyNet-with-Magisk-Zygisk-and-DenyList/blob/main/Edit-MagiskHide-props.jpg" width="250"></a> &emsp;
<img src="https://github.com/K3V1991/Passing-SafetyNet-with-Magisk-Zygisk-and-DenyList/blob/main/SafetyNet-Checker.jpg" width="250"></a>
