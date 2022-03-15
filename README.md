![Logo](https://raw.githubusercontent.com/vicvenpet/schoolweb-proyect/main/img/blue-white-banner.png)

[![license](https://camo.githubusercontent.com/8f54547853cfad57acfc8e06e6008cc296cda34d/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6c6963656e73652d417061636865253230322d626c75652e737667)](https://github.com/costular/android-kotlin-utils/blob/master/LICENSE)

A simple web page for a high school *business* project.

## Download

## How to use

It depends on utilities. Some of them just work as function extensions and you don't have to do anything special, just call a method like another one.

## API 

### Activity

``` kotlin
setFullScreen()
showToolbar() // Support and native
hideToolbar() // Support and native
```

### Context

``` kotlin
getClipboardManager()
copyTextToClipboard(value: String)
copyUriToClipboard(uri: Uri)
getTextFromClipboard(): CharSequence
getUriFromClipboard(): Uri?
getPreferences(): SharedPreferences
getPreferences(name: String, mode: Int): SharedPreferences
```

### SharedPreferences

#### SharedPreferences.use(lambda)
It automatically applies after lambda execution
``` kotlin
val sharedPrefs = context.getPreferences()
sharedPrefs.edit {
    putBoolean("first_use", false) // This refers to sharedPrefs instance
}
```

### Versions

These methods are static.

``` kotlin 
doWithVersion(version: 1.0) // ==
doWithAtLeastVersion(version: 1.1) // >=
doWithHigherVersion(version: 1.2) // >
doWithLowerVersion(version: 1.3) // <
```

Example

``` kotlin
Version 1.3
```
