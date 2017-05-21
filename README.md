[![Codacy Badge](https://api.codacy.com/project/badge/Grade/a40541d66db746bcb6669b7f30fd498d)](https://www.codacy.com/app/bazzite/nativescript-vibrate?utm_source=github.com&utm_medium=referral&utm_content=bazzite/nativescript-vibrate&utm_campaign=badger)
[![Bazzite Project](https://img.shields.io/badge/Bazzite-project-blue.svg?logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4NCjwhLS0gR2VuZXJhdG9yOiBBZG9iZSBJbGx1c3RyYXRvciAxNi4wLjAsIFNWRyBFeHBvcnQgUGx1Zy1JbiAuIFNWRyBWZXJzaW9uOiA2LjAwIEJ1aWxkIDApICAtLT4NCjwhRE9DVFlQRSBzdmcgUFVCTElDICItLy9XM0MvL0RURCBTVkcgMS4xLy9FTiIgImh0dHA6Ly93d3cudzMub3JnL0dyYXBoaWNzL1NWRy8xLjEvRFREL3N2ZzExLmR0ZCI%2BDQo8c3ZnIHZlcnNpb249IjEuMSIgaWQ9IkxheWVyXzEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHg9IjBweCIgeT0iMHB4Ig0KCSB3aWR0aD0iMzAyLjc4NnB4IiBoZWlnaHQ9IjI5MC4yNjZweCIgdmlld0JveD0iMC45MDUgMC40OTggMzAyLjc4NiAyOTAuMjY2IiBlbmFibGUtYmFja2dyb3VuZD0ibmV3IDAuOTA1IDAuNDk4IDMwMi43ODYgMjkwLjI2NiINCgkgeG1sOnNwYWNlPSJwcmVzZXJ2ZSI%2BDQo8dGl0bGU%2BbG9nb19yZWN0YW5nbGU8L3RpdGxlPg0KPGRlc2M%2BQ3JlYXRlZCB3aXRoIFNrZXRjaC48L2Rlc2M%2BDQo8ZyBpZD0iUGFnZS0xIj4NCgk8ZyBpZD0ibG9nb19yZWN0YW5nbGUiPg0KCQk8ZyBpZD0iR3JvdXAiPg0KCQkJPGcgaWQ9IkNsaXBwZWRfN18iPg0KCQkJCTxwb2x5Z29uIGlkPSJTaGFwZV83XyIgZmlsbD0iI0ZGRkZGRiIgcG9pbnRzPSIxMTAuMTIzLDAuNjAzIDAuOTA1LDIxNC42NjEgNDIuMzMzLDI5MC43NjQgMTkzLjI0NSwwLjQ5OCAJCQkJIi8%2BDQoJCQk8L2c%2BDQoJCQk8ZyBpZD0iQ2xpcHBlZF84XyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMDAwMDAsIDIxNC4wMDAwMDApIj4NCgkJCQk8cG9seWxpbmUgaWQ9IlNoYXBlXzhfIiBmaWxsPSIjRkZGRkZGIiBwb2ludHM9IjQyLjYxLDc2Ljc2NCAxNTIuNTEsNDguMTM1IDE1Mi4zOTgsMC40NjcgMC45MDksMC42NjEgCQkJCSIvPg0KCQkJPC9nPg0KCQkJPGcgaWQ9IkNsaXBwZWRfOV8iIHRyYW5zZm9ybT0idHJhbnNsYXRlKDE1MS4wMDAwMDAsIDIxNC4wMDAwMDApIj4NCgkJCQk8cG9seWxpbmUgaWQ9IlNoYXBlXzlfIiBmaWxsPSIjRkZGRkZGIiBwb2ludHM9IjEwOC45ODYsNzYuMzIzIDAuMTk4LDQ4LjEzNyAwLjA4OCwwLjQ2OSAxNTIuNjkxLDAuMjc1IAkJCQkiLz4NCgkJCTwvZz4NCgkJCTxnIGlkPSJDbGlwcGVkXzEwXyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTEwLjAwMDAwMCwgMC4wMDAwMDApIj4NCgkJCQk8cG9seWdvbiBpZD0iU2hhcGVfMTBfIiBmaWxsPSIjRkZGRkZGIiBwb2ludHM9IjAuMTIzLDAuNjAzIDE1MC4wNzcsMjkwLjMyMyAxOTMuNjkxLDIxNC4yNzUgODMuMjQ1LDAuNDk4IAkJCQkiLz4NCgkJCTwvZz4NCgkJPC9nPg0KCTwvZz4NCjwvZz4NCjwvc3ZnPg0K)](https://github.com/bazzite/nativescript-vibrate)

# NativeScript Vibrate

A vibrate NativeScript plugin for Android and iOS

## Installation

Run the following command from the root of your project:

```
$ tns plugin add nativescript-vibrate
```

This command automatically installs the necessary files, as well as stores nativescript-texttospeech as a dependency in your project's package.json file.

Due to a current open issue with NativeScript, [#669](https://github.com/NativeScript/nativescript-cli/issues/669), the plugin needs to be added before adding any platforms with the `tns add platform` command.

## Permissions

### Android

To use the vibrate functionality on Android your app must request permission access the vibrator. The plugin automatically adds the required permission shown below for you so you don't need to worry about editing the Android Manifest.

```xml
<uses-permission android:name="android.permission.VIBRATE" />
```

## Usage

To use the vibrate module you must first `require()` it:

```js
var vibrator = require("nativescript-vibrate");
```

After you have a reference to the module you can then call its `vibration(milliseconds)` method.

```js
// my-page.js
var vibrator = require("nativescript-vibrate");
vibrator.vibration(2000);
```

### Notes

#### iOS

There is no API to vibrate for a specific amount of time, so it will vibrate for the default no matter what (the duration is ignored).

## TODO

- [ ] Add support for vibration patterns in Android (iOS does not support this feature)
