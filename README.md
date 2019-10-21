## Build Chrome Extension Using Vue.js
Tutorial Link: [Build a Super Fast Google Chrome Extension Using Vue.js](https://www.mynotepaper.com/build-a-google-chrome-extension-using-vuejs.html)

## Output
![build-a-super-fast-google-chrome-extension-using-vue-js-output](https://user-images.githubusercontent.com/13184472/67241777-e3b2af00-f475-11e9-8f63-1be9751d6db6.png)

## Usage

### `npm run build`

Build the extension into `dist` folder for **production**.

### `npm run build:dev`

Build the extension into `dist` folder for **development**.

### `npm run watch`

Watch for modifications then run `npm run build`.

### `npm run watch:dev`

Watch for modifications then run `npm run build:dev`.

It also enable [Hot Module Reloading](https://webpack.js.org/concepts/hot-module-replacement), thanks to [webpack-chrome-extension-reloader](https://github.com/rubenspgcavalcante/webpack-chrome-extension-reloader) plugin.

:warning: Keep in mind that HMR only works for your **background** entry.

### `npm run build-zip`

Build a zip file following this format `<name>-v<version>.zip`, by reading `name` and `version` from `manifest.json` file.
Zip file is located in `dist-zip` folder.
