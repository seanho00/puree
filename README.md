# Pelican Puree

Based on 
[Pure-Simple](http://purepelican.com) theme, using the
[Purecss](http:purecss.io) responsive framework, for
[Pelican](http://docs.getpelican.com/) blogs.

## Settings in pelicanconf.py

All of these are optional.

* `BANNER` - Top banner image.
* `AVATAR` - Image for the circle cutout.
* `TAGLINE` - Used for the page titles and some meta tags.
* `FAVICON` - Image icon in the browser's address bar.
* `DISQUS_SITENAME` - Enable Disqus comments in articles.
* `DISQUS_ON_PAGES` - Enable Disqus comments in pages.
* `GOOGLE_ANALYTICS` - Enable Google Analytics tracking (eg. "UA-000000-00").
* `PIWIK_URL` and `PIWIK_SITE_ID` - Set the URL and site-id for Piwik tracking.
* `SOCIAL` - List of social links in the following format:

    ```python
    SOCIAL = (
        ('github', 'https://github.com/example/'),
        ('twitter-square', 'https://twitter.com/example'),
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

You may want to use `INDEX_SAVE_AS` in your `pelicanconf.py` to move
your article list to another URL.

## Custom article metadata:
* `banner` - will replace the banner image on a per-article basis

## Additional features
* [FitVids](https://github.com/davatron5000/FitVids.js) jQuery plugin for fluid width video embeds.


