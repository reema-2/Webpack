# WebPack Environment

This environment it is helpful for any one need to:

- Compile all SCSS files and transformed to two CSS files for LTR and RTL.
- Compile all JS files on single file.
- Compile all Images on single file.
- Compile all Font on single file.

### Loader used:

- css-loader
- file-loader
- html-loader
- sass-loader
- image-webpack-loader
- babel-loader

### plugins used:

webpack has a rich plugin interface. Most of the features within webpack itself use this plugin interface. This makes webpack flexible.
<br>

- html-webpack-plugin # Webpack plugin that simplifies creation of HTML files to serve your webpack bundles
- mini-css-extract-plugin # Webpack plugin extracts CSS into separate files. It creates a CSS file per JS file which contains CSS. It supports On-Demand-Loading of CSS and SourceMaps.
- optimize-css-assets-webpack-plugin # Webpack plugin to optimize \ minimize CSS assets.
- rtl-css-transform-webpack-plugin # Webpack plugin that implements RTLCSS framework for transforming Left-To-Right (LTR) Cascading Style Sheets (CSS) to Right-To-Left (RTL).
- clean-webpack-plugin # his plugin will remove all files inside webpack's `output.path` directory, as well as all unused webpack assets after every successful rebuild.
- babel-minify-webpack-plugin # Webpack Plugin for babel-minify - A babel based minifier

### `npm install`

Runs this to install all the project dependencies

### `npm run start:dev`

Runs this to start to webpack dev server with HMR ready

### For production

Run `npm run build` to build project's all assets in `dist` folder.

### WebPack Environment Architecture

```bash
├── dist/
    ├── fonts/
    ├── images/
    ├── index.html
    ├── script.js
    ├── style-ar.css
    ├── style.css
├── src/
    ├── fonts/
    ├── img/
    ├── js/
    │   └── App.js
    ├── sass/
    │   ├── base/
    │   ├── components/
    │   ├── layout/
    │   ├── pages/
    │   ├── themes/
    │   ├── utils/
    │   ├── vendors/
    │   └── main.scss
    ├── index.html

```
