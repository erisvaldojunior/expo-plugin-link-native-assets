# @erisvaldo.junior/expo-plugin-link-native-assets

Plugin to link assets to a native project so they can be loaded synchronously. 

It supports not only images and fonts but raw files too.

On Android, fonts are added to /res/font folder. Raw files are added to /res/raw.

On iOS, all files are linked as Resources.

## Add the package to your npm dependencies

```
yarn add @erisvaldo.junior/expo-plugin-link-native-assets
```

## Usage

```json
{
  "plugins": [
    [
      "@erisvaldojunior/expo-plugin-link-native-assets",
      [
        "./assets/icon.png",
        "./assets/font.ttf",
        "./assets/sound.wav",
      ],
    ],
  ],
}
```

Then run expo prebuild to link assets.
