# Google Open Sans - Web Font Kit

This project contains tools for integrating [Google Open Sans](https://github.com/google/fonts/tree/master/apache/opensans) fonts in a web environment.

## Installation

This [package](https://www.npmjs.com/package/opensans-webkit) can be deployed automatically using [npm](https://www.npmjs.com):

```
$ npm i opensans-webkit
```

## Usage (CSS)

CSS files are located in the `src/css/` directory:

* `src/css/open-sans.css` - file with no optimization for production environments;
* `src/css/open-sans.min.css` - file optimized for production environments.

Font files are located in the `fonts/` directory.

## Usage (SASS)

SASS files are located in the `src/sass/` directory:

* `src/sass/_mixins.scss` - mixins;
* `src/sass/_variables.scss` - variables;
* `src/sass/open-sans.scss` - main file.

Font files are located in the `fonts/` directory.

You can change the default fonts path by overriding `$opensans-path`:

```
$opensans-path: '/your/custom/path/';
```

To include [Google Open Sans](https://github.com/google/fonts/tree/master/apache/opensans) fonts in your SASS project, just add:

```
# set your custom path for fonts
$opensans-path '/your/custom/path/';

# include fonts from
@import 'open-sans.scss';
```

Optionally, the default font weights can be customized by overriding the following variables:

```
# with default values
$opensans-weight-extrabold: 800;
$opensans-weight-bold: 700;
$opensans-weight-semibold: 600;
$opensans-weight-normal: 400;
$opensans-weight-light: 300;
```

## Compile SASS to CSS

CSS files in the `src/css/` directory are generated from SASS files using:

```
# compile for development and production environment
$ npm run compile

# compile for development environment
$ npm run compile:development

# compile for production environment (minify)
$ npm run compile:production
```

## Font Formats

In addition to the `local` directive, the fonts are available in WOFF and WOFF2 formats.

Since the version 1.1.0 of this package, TTF fonts are no longer available. All recent browsers now support the WOFF format ([Browser Support for Font Formats](https://www.w3schools.com/css/css3_fonts.asp)).

## License

The source code is released under the Apache 2.0 license. For more information, see the [LICENSE](https://github.com/dcourtet/opensans-webkit/blob/master/LICENSE) file.