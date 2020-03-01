## yet another color converter

Convert HEX/RGB/HSL/HWB color models plus feColorMatrix’s values.

https://noeldelgado.github.io/yacc/

![screenshot](public/images/screenshot.png)

### Development
Start server on port 3000 with livereload watching files on the `src` folder

```sh
npm install
npm start
```

#### SVG sprite
If you need to add a new `.svg` files to the svg sprite located after the `body` tag:

- Place your `.svg`’s files on the `src/assets/svg` folder
- Make sure you have `svg-sprite` installed, e.i.: `npm i -g svg-sprite`
- Run npm script `npm run svg`
  - That should generate a new file at `src/assets/svg-sprite-symbol/svg/sprite.symbol.svg` (ignored by `.gitignore`’s rule)
- Copy the contents of that file and replace the `svg` line after the `body` 🙈

### Build
To minify the `build/{js,css}/main.<ext>` files. Make sure you have `uglify` installed, e.i.: `npm i -g uglify` and then

```sh
npm run build
```
