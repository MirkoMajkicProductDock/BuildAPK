# Github Action for building Android app of chosen flavour.

Use this action to build APK. Output of action will be path to APK and folder of APK.
It is possible to set a flavour you want to build APK for.

## Usage
```
- name: Build APK
  id: build
  uses: MirkoMajkicProductDock/BuildAPK@v0.0.1
```
To set custom flavour use:
```
with:
  flavour: demo
```
  
**Default flavour is release.**

Flavours that can be used are the one defined in `buildTypes` of `build.gradle` file in `app` module
```
buildTypes {
    dev {
        ...
    }
    qa {
        ...
    }
    demo {
        ...
    }
    release {
        ...
    }
}
```
