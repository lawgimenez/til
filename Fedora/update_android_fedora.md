## Android

#### Updating Android Studio in Fedora

Download Android Studio from developer.android.com and it comes in tar.gz file. Cd to download folder and then run on terminal

```bash
sudo tar -zxvf android-studio-*-linux.tar.gz
```

If `/opt/android-studio/` is not empty, remove it

```
rm -r /opt/android-studio/
```

Move
```
sudo mv android-studio /opt/
```

```
sudo ln -sf /opt/android-studio/bin/studio.sh /bin/android-studio
```