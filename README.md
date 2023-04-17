# flutter_flavors_demo
An demo to show how to create Flutter white label apps by flavors

## Flavors
* Check ***base_app** and **ext_app*** folders
* Check **dependencies** in ext_app/pubspec.yaml
``` yaml
dependencies:
  flutter_flavors_demo_base_app:
    path: ../base_app
```
* Check **dependency_overrides** in ext_app/pubspec.yaml
``` yaml
dependency_overrides:
  flavor:
    path: flavor
```
* Check ***base_app/flavor/lib/flavor_strings.dart*** and ***ext_app/flavor/lib/flavor_strings.dart***


## Android Localized App Name on Desktop (安卓名稱及圖標本地化)
* Noted: **android:label="@string/app_name** in ***base_app/android/app/src/main/AndoridManifest.xml*** and in ***ext_app/android/app/src/main/AndoridManifest.xml***
* Specify **app_name** in ***base_app/android/app/src/main/res/values/strings.xml***, ***base_app/android/app/src/main/res/values-zh-rCN/strings.xml***, ***base_app/android/app/src/main/res/values-zh-rTW/strings.xml***
* Specify **app_name** in ***ext_app/android/app/src/main/res/values/strings.xml***, ***ext_app/android/app/src/main/res/values-zh-rCN/strings.xml***, ***ext_app/android/app/src/main/res/values-zh-rTW/strings.xml***


## Icons
* To change app icons, replace icons in ***base_app/assets/icon-base.png*** and ***ext_app/assets/icon-base.png***. And then run "flutter pub run flutter_launcher_icons" in both "base" and "ext_app" folders to generate app icons （執行指令，產生app icons）