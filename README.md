# TAMAN

Taman is a responsive theme for [Pelican](http://getpelican.com), it is hackish port of Jekyll's [Logom](https://github.com/swanson/lagom) theme.

The name is synonym of word [Lagom](https://en.wikipedia.org/wiki/Lagom) in Slavic languages.

## Screenshot

![theme screenshot](https://raw.github.com/karambir/taman/master/screenshot.png)

## FEATURES

- responsive
- syntax highlighting for pre blocks
- minify css files
- supports Google Analytics or custom analytics script
- custom list of links
- social links with FontAwesome 6
- a custom favicon and logo urls
- no custom menu
- support canonical urls
- built with Bootstrap 5

## INSTALL

Clone the [repository](https://github.com/karambir/taman), edit your `pelicanconf.py` and modify the `THEME` variable to make it point to the downloaded theme location.

The theme use *assets* plugin to handle minification of css files from [here](https://github.com/getpelican/pelican-plugins/tree/maser/assets)

- Install required package for *assets* plugin by `pip install webassets`
- Refer this [documentation](https://github.com/getpelican/pelican-plugins#how-to-use-plugins) to install plugin.

## PELICANCONF.PY

Supports a number of common global variables but patches are welcomed if you need better support.

- `GOOGLE_ANALYTICS` to use Google Analytics, set this var to your UA-XYZ code

- `CUSTOM_ANALYTICS` set this to your custom js script(including script tag). This is added at the end of body.

- `TAGLINE` some text rendered right below the logo

- Use `canonical_url` var in article markdown file to specify original url of article.

- To set custom logo and favicon set following in config:

    STATIC_PATHS = ['images', 'extra/favicon.png', 'extra/logo.png']
    EXTRA_PATH_METADATA = {
        'extra/favicon.png': {'path': 'favicon.png'},
        'extra/logo.png': {'path': 'logo.png'},
    }

    USER_LOGO_URL = '/logo.png'
    USER_FAVICON_URL = '/favicon.png'

When developing locally, you may want to set the following variable: `SITEURL = http://localhost:8000`

## AUTHOR

Lagom theme is originally authored by [Matt Swanson](https://mdswanson.com/). I started with [pelican-svbhack](https://github.com/gfidente/pelican-svbhack) as base.

## LICENSE

Released under MIT License, full details in `LICENSE` file.
