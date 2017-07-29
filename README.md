## TWRP device tree for Micromax Canvas Selfie Lens Q345 (Q345)

Add to `.repo/local_manifests/Q345.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/micromax/Q345" name="android_device_micromax_Q345" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_Q345-eng
make -j5 recoveryimage
```
