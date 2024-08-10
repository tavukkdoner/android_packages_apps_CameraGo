### Add in local manifest

```
 <remote  name="tavukkdoner"
           fetch="https://github.com/tavukkdoner"
           revision="lineage-21" />

<project path="packages/apps/CameraGo" name="android_packages_apps_CameraGo" remote="tavukkdoner" revision="inherit" />
```

### Add following in device.mk

```
# Google Camera Lite
$(call inherit-product, packages/apps/CameraGo/config.mk)
```
