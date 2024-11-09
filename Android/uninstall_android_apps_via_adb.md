# Uninstall Android apps via ADB

Enable Developer Options in the device, and accept any prompt options displayed from the device.

```bash
adb shell
```

```bash
pm list packages
pm uninstall -k --user 0 com.huawei.browser
```
