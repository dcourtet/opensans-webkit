# Google Open Sans - Web Font Kit

This project contains tools for integrating [Google Open Sans](https://github.com/google/fonts/tree/master/apache/opensans) fonts in a web environment.

## Installation (npm)

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
$opensans-path '/your/custom/path/';
```

To include [Google Open Sans](https://github.com/google/fonts/tree/master/apache/opensans) fonts in your project, just add:

```
# set your custom path for fonts
$opensans-path '/your/custom/path/';

# include fonts from
@import 'open-sans.scss';
```

# Compile SASS to CSS

CSS files in the `src/css/` directory are generated from SASS files using:

```
# compile for development and production environment
$ npm run compile

# compile for development
$ npm run compile:development

# compile for production (minify)
$ npm run compile:production
```

## License

The source code is released under the Apache 2.0 license.