# MiniCssExtractPluginErrorRepro

This repo is meant to provide a reproduction for an error that Angular CLI and MiniCssExtractPlugin throw when building with postcss-loader and Tailwind CSS.

## Reproduction Error

The error thrown by mini-css-extract-plugin is as follows:
```
ERROR in Module build failed (from ./node_modules/mini-css-extract-plugin/dist/loader.js):
TypeError: Cannot read property 'replace' of undefined
    at normalizeBackSlashDirection (F:\Workspace\mini-css-extract-plugin-error-repro\node_modules\webpack\lib\RequestShortener.js:16:17)
    at new RequestShortener (F:\Workspace\mini-css-extract-plugin-error-repro\node_modules\webpack\lib\RequestShortener.js:26:15)
    at new Compiler (F:\Workspace\mini-css-extract-plugin-error-repro\node_modules\webpack\lib\Compiler.js:195:27)
    at Compiler.createChildCompiler (F:\Workspace\mini-css-extract-plugin-error-repro\node_modules\webpack\lib\Compiler.js:558:25)
    at Compilation.createChildCompiler (F:\Workspace\mini-css-extract-plugin-error-repro\node_modules\webpack\lib\Compilation.js:2243:24)
    at Object.pitch (F:\Workspace\mini-css-extract-plugin-error-repro\node_modules\mini-css-extract-plugin\dist\loader.js:89:43)
```

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.
