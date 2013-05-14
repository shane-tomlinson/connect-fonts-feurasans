# connect-fonts-feurasans

Feura Sans fontpack for [connect-fonts](https://github.com/shane-tomlinson/connect-fonts).

## Usage

1. Include [connect-fonts](https://github.com/shane-tomlinson/connect-fonts) in a node module.
```js
const font_middleware = require("connect-fonts");
```

2. Include the font packs that you want to serve.
```js
const font_pack  = require("connect-fonts-feurasans");
```

3. Add a middleware by calling the `setup` function.
```js
    app.use(font_middleware.setup({
      fonts: [ font_pack ],
      allow_origin: "https://exampledomain.com"
    }));
```

4. Add a link tag to include the font CSS.
```html
<link href="/feurasans-bold/fonts.css" type="text/css" rel="stylesheet"/ >
```

Multiple fonts from the family can be included by using a comma separated list of fonts:
```html
<link href="/feurasans-bold,feurasans-light,feurasans-medium,feurasans-regular/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available fonts:
* feurasans-bold
* feurasans-light
* feurasans-medium
* feurasans-regular

Locale-optimised font sets can be served by specifying the locale in the fonts.css URL.
```html
<link href="/latin/feurasans-bold/fonts.css" type="text/css" rel="stylesheet"/ >
```

Available subsets:
* latin
* en

5. Set your CSS up to use the new font by using the "Feura Sans" font-family.
```
    body {
      font-family: 'Feura Sans', 'sans-serif', 'serif';
    }
```

## Font Info
Feura Sans

* Copyright: Digitized data copyright Â© 2012-2013, The Mozilla Corporation and Telefonica S.A.
* Trademark: Feura Sans is a trademark of The Mozilla Corporation.
* Designer: Carrois Corporate & Edenspiekermann
* Designer URL: http://www.carrois.com 
* Vendor: Carrois Corporate GbR & Edenspiekermann AG
* Vendor URL: http://www.edenspiekermann.com

## Development Info
* Homepage: https://github.com/shane-tomlinson/connect-fonts-feurasans
* Repo: https://github.com/shane-tomlinson/connect-fonts-feurasans

## Author
* Shane Tomlinson
* shane@shanetomlinson.com
* stomlinson@mozilla.com
* set117@yahoo.com
* https://shanetomlinson.com
* https://github.com/shane-tomlinson
* https://github.com/stomlinson
* @shane_tomlinson


## License

Software: Licenced under version 2.0 of the MPL

  https://www.mozilla.org/MPL/

Fonts: Licensed under version 2.0 of the Apache

  http://www.apache.org/licenses/LICENSE-2.0

