# Pelican Puree

Lightweight, mobile-first, responsive theme for 
[Pelican](http://docs.getpelican.com/) blogs.

## Features
* Top header panel on small screens becomes a sidebar on larger screens.
* Special template for optional landing page.
* Minimal dependencies:
  + [Pure.css](http://purecss.io)
  + [Font Awesome](https://fortawesome.github.io/Font-Awesome/)
  + No Bootstrap!  No jQuery!
* Optional dependencies, disabled by default:
  + [Disqus](http://disqus.com)
  + [Google Analytics](http://google.com/analytics)
  + [Piwik](http://piwik.org)

## Many thanks
* [Pure-Simple](http://purepelican.com) Pure.css-based theme for Pelican
* [pelican-bootstrap3](https://github.com/DandyDev/pelican-bootstrap3) theme
* [Pure.CSS Layout](http://purecss.io/layouts/blog/) sample blog layout

## Settings in pelicanconf.py

All of these are optional.

* `TAGLINE` (or `SITESUBTITLE` for compatibility) - Short text for header
* `BANNER` - Background image for header.
* `AVATAR` - Image for the circle cutout.
* `FAVICON` - Image icon in the browser's address bar.
* `DISQUS_SITENAME` - Enable Disqus comments in articles.
* `DISQUS_ON_PAGES` - Enable Disqus comments in pages, not just articles.
* `GOOGLE_ANALYTICS` - Enable Google Analytics tracking (eg. "UA-000000-00").
* `PIWIK_URL` and `PIWIK_SITE_ID` - URL (without "http://") and site-id for Piwik tracking.
* `MENUITEMS` - List of (Title, URL) tuples to add to nav menu.
* `LINKS` - List of (Title, URL) tuples to add to header.
* `SOCIAL` - List of social links in the following format:

    ```python
    SOCIAL = (
        ('github', 'https://github.com/example/'),
        ('twitter', 'https://twitter.com/example'),
    )
    ```
    where the first value of the tuple is the icon name from http://fontawesome.io/icons/ after stripping `fa-` (eg. `fa-github` will be `github`)

This theme respects `DISPLAY_PAGES_ON_MENU` and `DISPLAY_CATEGORIES_ON_MENU`.

## Custom landing page
You may specify a page/article to be your home page, rather than the
default listing of recent articles.  In the metadata of your chosen
landing page, specify the following (assuming you're using Markdown):

	Title: My wonderful site
	Template: landing
	URL:
	Save_As: index.html
	Status: hidden

You may want to use `INDEX_SAVE_AS` in your `pelicanconf.py` to move
your article list to another URL.

## Custom article metadata:
* `banner` - will replace the `BANNER` image on a per-article basis

