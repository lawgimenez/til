## Install Android Studio on Fedora

```
sudo dnf upgrade
sudo dnf update
sudo dnf install bzip2-libs.i686 zlib.i686 ncurses-libs.i686 -y 
```

Download Android Studio from developer.android.com and it comes in tar.gz file. Cd to download folder and then run on terminal

```
sudo tar -zxvf android-studio-*-linux.tar.gz
sudo mv android-studio /opt/
sudo ln -sf /opt/android-studio/bin/studio.sh /bin/android-studio
```

Install vim and then run the command below

```
sudo vim /usr/share/applications/android-studio.desktop
``` 

Type in the following below

```
[Desktop Entry]
Version=1.0
Type=Application
Name=Android Studio
Comment=Android Studio
Exec=bash -i "/opt/android-studio/bin/studio.sh" %f
Icon=/opt/android-studio/bin/studio.png
Categories=Development;IDE;
Terminal=false
StartupNotify=true
StartupWMClass=jetbrains-android-studio
Name[en_GB]=android-studio.desktop
```

Exit vim by typing in : then wq