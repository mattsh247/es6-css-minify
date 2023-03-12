# Archived - Feel free to fork and upload to VSC Marketplace.

# JS & CSS Minifier

[![Visual Studio Marketplace](https://vsmarketplacebadge.apphb.com/installs-short/olback.es6-css-minify.svg)](https://marketplace.visualstudio.com/items?itemName=olback.es6-css-minify)
[![rating](https://vsmarketplacebadge.apphb.com/rating-star/olback.es6-css-minify.svg)](https://marketplace.visualstudio.com/items?itemName=olback.es6-css-minify)
[![Visual Studio Marketplace](https://vsmarketplacebadge.apphb.com/version/olback.es6-css-minify.svg)](https://marketplace.visualstudio.com/items?itemName=olback.es6-css-minify)
[![GitHub package version](https://img.shields.io/github/package-json/v/olback/es6-css-minify/3.0.svg?style=flat&logo=github&label=Github%20(This%20branch))](https://github.com/olback/es6-css-minify/tree/3.0)

If you found this extension useful and want to support further development, please consider [donating](https://www.paypal.me/olback).

# [Help wanted - New maintainer(s)!](https://github.com/olback/es6-css-minify/issues/140)

| OS | Status |
|----| ------ |
| Linux & MacOS | [![Build Status](https://travis-ci.com/olback/es6-css-minify.svg?branch=3.0)](https://travis-ci.com/olback/es6-css-minify) |
| Windows | [![Build status](https://ci.appveyor.com/api/projects/status/9xa8j6tq3vstixj2/branch/3.0?svg=true)](https://ci.appveyor.com/project/olback/es6-css-minify/branch/3.0) |

A simple Javascript & CSS minifier.  
A `Minify` button should appear in the status bar when opening a `.js` or a `.css` file. You can also run `Minify: Document` by clicking `F1` or `CTRL+SHIFT+P`.

### Loading custom configs
By default the extension will look for `.uglifyrc`, `.cleancssrc` and `.autoprefixerrc`.  
You can change the paths in settings. After changing settings in any of the config files, make sure to reload with `Minify: Reload config`. If the reload fails, make sure you don't have syntax errors in your config. If you want to go back to the default config, rename/delete your config file(s).

The config parsed by the extension is just passed to terser, clean-css or autoprefixer. If the output is diffrent from what you expected, please confirm that the issue is with the extension and not terser, clean-css or autoprefixer before opening an issue.

### Minify on save, `disabled` by default!
Minify on save can be enabled in settings.  

### Generate source maps
Source maps can be generated by changing `es6-css-minify.genCSSmap` and `es6-css-minify.genJSmap` respectively.

#### Dependencies:
* [terser](https://www.npmjs.com/package/terser)
* [clean-css](https://www.npmjs.com/package/clean-css)
* [autoprefixer](https://github.com/postcss/autoprefixer)
