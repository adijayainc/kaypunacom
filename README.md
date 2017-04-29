## Spresso theme

Spresso is a simple theme for **[Spress](http://spress.yosymfony.com)**
based on Bootstrap 3. The content is organized in one central column.

See a [demo](http://yosymfony.github.io/Spress-example/).

![Spresso theme preview](/screenshot.png)

## Installation
You can create a [site based on Spresso](#creating-a-new-site-based-on-this-theme-creating-site)
or install this one as a theme of a [pre-existing site](#install-as-a-theme-of-pre-existing-site-pre-existing).

**Requirements:**
* Spress >= 2.2.0

### Creating a new site based on this theme {#creating-site}

Performs the following command and Spresso theme will be
installed in `mysite` folder:

```bash
$ spress new:site mysite spress/spress-theme-spresso
```

### Install as a theme of pre-existing site {#pre-existing}

Go to your site folder and performs the following command:

```bash
$ spress add:plugin spress/spress-theme-spresso
```
And add this line to the `config.yml` file of your site:

```yaml
themes:
    name: spress/spress-theme-spresso
```

### Features:

* Responsive design: Support to mobile and tablets.
* Disqus comments on your posts.
* Support to [Twitter Cards](https://dev.twitter.com/docs/cards) and [Facebook Open Graph](https://developers.facebook.com/docs/opengraph/).
* Top and bottom menu.
* Social networks link at the footer.
* Support to Google and Bing site validation.
* Code snippets highlight.
* Iconic font by [Fort Awesome](http://fortawesome.github.io/Font-Awesome).
* Sitemap and RSS feed.

### How to install?

This theme is included with Spress.

### How to use?

**Create a new site**:

`$ spress new:site /your-site-dir spresso`

#### Menus

Spresso support top and bottom menus. To configure, you can edit
`top_menu` and `bottom_menu` options from the `config.yml`:

```yaml
top_menu:
    - { name: Home, url: / }
    - { name: About, url: /about }

    # To generate a absolute URL using site.url value:
    - { name: Docs, url: /docs, site_url: true}

bottom_menu:
    - { name: Your link, url: https://your-url }
```

#### Comments

Comments are powered by [Disqus](disqus.com) and it need your
**disqus shortname**. To get it, you need create a account at this service.
It's free.

##### Disable comments

By default, Disqus comments are enabled. If you want a post without comments, set
the `comments` variable to `false` at the Front-matter of the post:

```yaml
---
comments: false
---
```
