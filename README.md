# Add in local manifest

```
 <remote  name="tavukkdoner"
           fetch="https://github.com/tavukkdoner"
           revision="lineage-21" />

<project path="packages/apps/CameraGo" name="android_packages_apps_CameraGo" remote="tavukkdoner" revision="inherit" />
```

# Add following in device.mk

```
# Google Camera Lite
$(call inherit-product, packages/apps/CameraGo/config.mk)
```

# Crash that occurs when trying to view a photo taken

### error.log
```
ErrorHandlingIntentFact: Neither Gallery Go nr Photos app installed on device.
AndroidRuntime: Shutting down VM
AndroidRuntime: FATAL EXCEPTION: main
AndroidRuntime: Process: com.google.android.apps.cameralite, PID: 26334
AndroidRuntime: java.lang.IllegalArgumentException: Error type OPEN_SETTINGS_GALLERY should have an intent.
```

### Solution: 

> install Gallery ( https://play.google.com/store/apps/details?id=com.google.android.apps.photosgo )
> or 
> install Photos ( https://play.google.com/store/apps/details?id=com.google.android.apps.photos )



https://www.virustotal.com/gui/file/f226b2531076fe08cc943232d18bcc820aee0f6825fdaba31df43e46a3429f6d
