# Fabric Title Changer

A simple Fabric mod that allows you to customize the text that appears in the title window of Minecraft.

## Configuration
There are 5 options which can be modified by editing the configuration .json file found in `<minecraft directory>/config/fabric-title-changer/settings.json`.

- `includeVersionNumber`: Will hide or remove the version number from the title (1.15.2, etc).
- `includeAsterisk`: Modded versions now show an asterisk in the title, set this to `false` to remove it.
- `includeNetworkStatus`: Minecraft now shows a "Singleplayer", "Multiplayer", "LAN" text in the titlebar. Set this to `false` to disable this behavior.
- `overrideMinecraftTitle`: Set a `value` property on this field to change the "Minecraft" text shown in the titlebar to anything else.
- `overrideFullTitle`: This will ignore all other settings and force the window to always have the specified title.

## Default Configuration
```json
{
  "windowTitle": {
    "includeVersionNumber": {
      "comment": "Include the version number (1.15.2, etc)",
      "value": true
    },
    "includeAsterisk": {
      "comment": "Include the asterisk for modded versions",
      "value": true
    },
    "overrideFullTitle": {
      "comment": "Set to ignore other settings and define a full pre-defined name."
    },
    "includeNetworkStatus": {
      "comment": "Include the network status (Singleplayer, Multiplayer, LAN, etc.)",
      "value": true
    },
    "overrideMinecraftTitle": {
      "comment": "Set to change the phrase \"Minecraft\" in the title."
    }
  }
}
```