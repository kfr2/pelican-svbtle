# Pelican-Svbtle

Svbtle theme is a close copy of the design of [Svbtle.com](http://www.svbtle.com) with a few minor changes for use with [Pelican](http://getpelican.com) and to suit [Kevin Richardson](https://github.com/kfr2)'s personal tastes.

## DEMO

You can see the [theme in action](http://magically.us/), or the site code [here](https://github.com/kfr2/magically.us).

![theme screenshot](https://raw.github.com/kfr2/pelican-svbtle/master/screenshot.png)

## FEATURES

- syntax highlighting for code blocks
- Google Analytics
- Disqus commenting
- custom list of links

## INSTALLATION

Download or clone the [repository](https://github.com/kfr2/pelican-svbtle). Edit `pelicanconf.py` and modify the `THEME` variable to point to the downloaded theme location.

## PELICANCONF.PY

The following are the Pelican global variables currently supported by the theme.  You may wish to view [Kevin Richardson's pelicanconf.py](https://github.com/kfr2/magically.us/blob/master/pelicanconf.py) for more information.

### sidebar settings
- *note: listed in the order shown in the template*
- `LOGO_URL` -- the URL of the logo for the site.
- `TAGLINE` -- the text to display underneath AUTHOR in the left-hand menu.
- `DISPLAY_PAGES_ON_MENU` = True/False.    If True, display a list of pages defined within `content/pages`
- `MENUITEMS` -- (('name1', 'url1'), ('name2', 'url2'))
- `LINKS` -- (('name1', 'url1'), ('name2', 'url2'))`

### other
- `DEFAULT_DATE_FORMAT = ('%b %d, %Y')` -- date format for post publication dates
- `FEED_DOMAIN = SITEURL`.  The prefix URL for the Atom/RSS feeds.
- `FEED_ATOM` -- ATOM feed name.  ex: 'feeds/all.atom.xml'
- `FEED_RSS` -- RSS feed name.  ex: 'feeds/all.rss'
- `HEADER_MESSAGE` -- the text to display in the header of the homepage.  Defaults to "Have a great day."
- `GOOGLE_ANALYTICS` -- the site's Google Analytics key string.

When developing locally, set the following variable:

`SITEURL = http://localhost:8000`

## MODIFICATION

- Accent color can be changed by editing `@accent` in `./static/css/style.less`.  You will need to install lessc via node package manager (`npm install -g lessc`) or a similar tool to compile the LESS stylesheet into a CSS stylesheet via `make less`.

- A different Pygmentize theme can be used by editing `./Makefile` and running `make pygments`.

## AUTHORS

- [William Ting](https://github.com/wting)
- [Kevin Richardson](https://github.com/kfr2)

## LICENSE

Released under MIT License.  See full details in `LICENSE` file.

## KNOWN ISSUES

- no IE testing
- no custom menu