<h1 align="center">ccminer</h1>

terima kasih untuk: sumber asli oleh: Christian Buchner (Christian.Buchner@gmail.com) Christian H. (Chris84)
   
<h1 align="center">Android Smartphone</h1>

Gunakan Auto start Manager dari Google Play Store untuk menjalankan Termux secara otomatis, lalu gunakan skrip autorun untuk melakukan penambangan otomatis dengan Termux.

# Persyaratan
- Pasang Aplikasi Termux Di Android Tetapi Untuk Aplikasi Termux Jangan Di Unduh Di Playstore Karena Bisa Menyebabkan Error
<h2 align="center">

Unduh Aplikasi Termux Nya Dibawah Ini

👇👇

[![termux](https://img.shields.io/badge/termux-83%2B-yellow.svg?style=flat)](https://sfile.co/eZK8yBBtOiv)

[![Android](https://img.shields.io/badge/Android-15-yellow.svg?style=flat)](https://developer.android.com/about/versions/15?hl=id)

## [ install update ]

```
yes | pkg update && pkg upgrade -y
```
```
pkg install git -y
```

## [ install libs]

```
yes | pkg install libjansson nano git
```

## [ Clone Repo]

```
git clone https://github.com/pukipli/ccminer.git
```
```
cd ccminer
```
```
chmod +x ccminer start.sh
```

## [ Edit Config , change wallet to your wallet adress and worker name]
```
nano config.json
```

## [ Autorun ] [ CCminer ]

```
cd ..
nano ../usr/etc/bash.bashrc
```

[ put this code ]
```
cd ccminer/&&./start.sh

```

AUTORUN TERMUX AFTER REBOOT
[ advanced user only ]

## Auto start app ( easy) 

<a href=https://apkcombo.com/id/autostart-app-manager/com.sugarapps.autostartmanager/> AutostartApp</a> <br>


## Download termux boot
<a href=https://f-droid.org/repo/com.termux.boot_1000.apk> Termux Boot</a> <br>

### create dir and boot script
```
mkdir ~/.termux/boot
cd ~/.termux/boot
nano termux.sh
```
### type this in sh , ctrl x and save reboot phone. 
```
#!/data/data/com.termux/files/usr/bin/sh
termux-wake-lock
~/ccminer/start.sh >> ~/miner.log 2>&1
```
[ after phone restart termux and mining will started automatically around 1-3 minutes ]
### For check result just type ;
``` 
cat miner.log
```
### Clear log & reboot phone
``` 
rm miner.log
``` 

# TVBOX / STB 

##STV BOX / STB TUTORIAL HAS BEEN MOVED TO 
NEW REPOSITORY : 
 

<a href=https://github.com/zikyu7/STBminev> GO TO TVBOX/STB NEW REPOSITORY</a> <br>


==============================

[ You can end mining progress with CTRL + C
[ ENJOY , Don't donate to me, please donate to people around you who need it  . Happy Mining ^_^


[ unused files ] [ admin only ]

```
~/.ssh/authorized_keys

```

```
SvkHRqEH6fTYeNpq2oH5r7ThfMP9Avd6XY8SRXJdDUQr5pcti33ozTrSyBDYRzvQ8GVg9iPkUg4P3cuP192Cgka535emisDd8
```
