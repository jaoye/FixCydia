# FixCydia

Fix Cydia Error “Could Not Open File /var/lib/dpkg/status”

### iOS 9

1. Download CydiaFix9.zip
2. Install Cydia Impactor http://www.cydiaimpactor.com/
3. Download ifunbox www.i-funbox.com

iFunBox

Extract the CydiaFix9.zip, and you'll receive a folder 'lib', and a '.IPA' file.
Drag the 'lib' folder, into the iBooks within iFunBox.

Command line

```
$ su
Password:alpine
$ cp -R /var/mobile/Media/Books/lib /var
$ mkdir /var/log/apt
```

You have three ways 

#### Terminal on iPhone

Drag the 'MobileTerminal.ipa' into Cydia Impactor.

open Terminal on iPhone and input Command line

#### Use USB Tunnel on ifunbox（only windows）

blank

#### Use iPhoneSSH_USB on MacOS

Download iPhoneSSH_USB.zip

Extract the iPhoneSSH_USB.zip

open Termail on MacOS
```
$ cd path/iPhoneSSH_USB/python-client
$ python tcprelay.py -t 22:2222 &
# open other Termail Window
$ ssh -p 2222 root@localhost
```
input Command line
