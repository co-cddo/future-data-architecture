Future Data Architecture
==================================

This repository holds documentation on future data architecture.
The documents are written in markdown and published on the web via Github pages:

  https://supreme-adventure-e2erl4p.pages.github.io/

A github action is triggered when code is merged into main, with the result
that any changes are published on the Github pages.

Jekyll
------
The transformation of static markdown pages into a static website is performed
by [Jeykll](https://jekyllrb.com/).

To build the site locally:

- Install Ruby with bundler (see https://www.ruby-lang.org)
- Clone this repo locally
- At the app root use the command `bundle install` to install the dependencies
- The following command can then be used to build the site:

```
jekyll serve
```

This should result in the site being built into `_site` and a local web server being
started that will present the site at: `http://localhost:4000`.

The server will keep track of changes, so if you update the code all you should need
to do is refresh the page to see the effect of the change.

If an error occurs it will be displayed in the console where the jekyll code is running.

Markdown
--------
Jekyll use kramdown markdown. A quick reference can be found here:

  https://kramdown.gettalong.org/quickref.html

Liquid
------
Additional functionality is provided by [Liquid](https://shopify.github.io/liquid/).
The most obvious use of this is the generation of the navigation column which is
defined in `_includes/navigation.html`.

Note that some of the more advanced functions such as `group_by_exp` are provided
by [Liquid Filters](https://jekyllrb.com/docs/liquid/filters/).

The content
-----------

Jeykll searches this repository's files for content that it can convert into web pages.
The main content is provided by markdown files using the extension `.md`. One
such file being `/index.md` which is converted by Jeykll to `index.html` and if running
locally is placed in `_site/index.html`. This becomes the site's default root page.

Other content is presented in the folders `architecture` and `principles`.

For Jeykll to use the markdown files they must start with the following content:

```
---
title: A title
layout: default
position: 5
---
```
Where:

- `title` is the label used to identify the page. It will appear in the `h1` tag at the top
  of the page, and in the navigation bar.
- `layout` defines which layout file will be used to wrap the content. `default` is defined
  at `_layouts/default.html` and provides a GOV.UK styled page structure including a
  navigation element.
- `position` is optional, but when present modfiies where the page is listed within the
  navigation column. A higher number results in the page being positioned further down the
  navigation listing (within the current group - grouping is by directory). If no position
  is provided the page will be placed alphabetically at the top of its group navigation
  listing.

Navigation
----------
The navigation code is currently set so that the only file in the root directory that is
given a navigation link is `/index.md`.

For a page to be listed in the navigation column, it must be placed in a subfolder that does
not start with `_`. For example, `architecture` or `principles`.

The content for each subfolder containing markdown is listed in the navigation column,
below a heading using the folder name.

The navigation code can be found at `/includes/navigation.html` and it is placed in the
page via the default layout (`_layouts/default.html`).

Images
------
Image files should be placed into the folder `assets/images`.

To display an image within the content add a
[link to the image](https://kramdown.gettalong.org/quickref.html#links-and-images)
within the markdown and add an exclamation mark (`!`) at the start of the link markdown.

So if there were an image at `assets/images/my_image.png`, it could be displayed within
the page by adding this markdown:

```
![My image](assets/images/my_image.png)
```
Note that in this example "My image" would appear as the image's alt text.
