# TAMAN

Taman is a responsive theme for [Pelican](http://getpelican.com), it is hackish port of Jekyll's [Logom](https://github.com/swanson/lagom) theme. 

The name is synonym of word [Lagom](https://en.wikipedia.org/wiki/Lagom) in Slavic languages.

## DEMO

You can see the [theme in action](http://carambir.in/).

![theme screenshot](https://raw.github.com/karambir/taman/master/screenshot.png)

## FEATURES

- responsive
- syntax highlighting for pre blocks
- supports google analytics
- custom list of links
- social links with FontAwesome4
- custom favicon and logo urls
- no custom menu

## INSTALL

Clone the [repository](https://github.com/karambir/taman), edit your `pelicanconf.py` and modify the `THEME` variable to make it point to the downloaded theme location.

## PELICANCONF.PY

Supports a number of common global variables but patches are welcomed if you need better support.

- `GOOGLE_ANALYTICS` to use Google Analytics, set this var to your UA-XYZ code

- `DISQUS_SITENAME` set this to your Disqus sitename to enable disqus comments in articles

- `TAGLINE` some text rendered right below the logo

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

Lagom theme is originally authored by [Matt Swanson](https://mdswanson.com/). Theme color is copied from [Daniel Berkompas](http://blog.danielberkompas.com/). I started with [pelican-svbhack](https://github.com/gfidente/pelican-svbhack) as base.

## LICENSE

Released under MIT License, full details in `LICENSE` file.
