---
layout: page-fullwidth
title: "Documentation"
subheadline: "Documentation for developers"
teaser: "The documentation for developers"
permalink: "/developers/"
header: no
---
<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
**Table of Contents**
{: #toc }
*  TOC
{:toc}
</div>
</div><!-- /.medium-4.columns -->

<div class="medium-8 medium-pull-4 columns" markdown="1">

## Start Here   {#edit-navigation}

To customize the navigation of *Feeling Responsive*, you have to open the [YAML](https://jekyllrb.com/docs/datafiles/)-file `_data/navigation.yml`. Edit the data and adjust it to your own needs.

## About Komodo Platform   {#formats}

*Feeling Responsive* supports you with different templates for your content. These are the actual page/post formats:

## Learning Launchpad   {#formats2}
The [page/post format]({{ site.url }}{{ site.baseurl }}/design/page/) has no sidebar by default, its content is centered and beneath the content the visitor gets some metadata like categories, tags, date and author if provided via data in front matter of the post.

use in front matter via: `layout: page`

## Core Technology Discussions   {#formats2}
If you want to show the sidebar, just enter `sidebar: left` or `sidebar: right` in front matter, and *whoops, there it is*! To customize the content of the sidebar, open `_includes/sidebar`.


# Smart Chain Essentials   {#formats3}
If you want to show metadata like categories, tags and date at the end of the page, just enter `show_meta: true`. It's on by default. You can change it via `_config.yml`. To turn of metadata just enter – *yes, you guessed right* – `show_meta: false`.



## Introduction to Smart Chain Documentation
If you want full control of styling a page, then use the [page fullwidth template]({{ site.url }}{{ site.baseurl }}/design/page-fullwidth/). To set up a grid, just use the [foundation grid system](http://foundation.zurb.com/docs/components/grid.html).

use in front matter via: `layout: page-fullwidth`


## Smart Chain Setup
This template is special. It allows you to define three *widgets* which are displayed with a headline, image, description and a link to the content. It's used for the [homepage]({{ site.url }}{{ site.baseurl }}) of this website.

use in front matter via: `layout: frontpage`


## Smart Chain Tutorials
If you're a video producer or cineast, you'll like the [video template]({{ site.url }}{{ site.baseurl }}/design/video/). It darkens the layout to black and lets the video stand out full-width.

use in front matter via: `layout: video`

<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }

## Smart Chain API   {#styling}

Feeling Responsive offers lots of possibilities to style your articles. You can style your content in different ways. There are elements like subheadlines, feature images, header images, homepage images, meta data like categories and tags and many more.


# Antara Framework

If you need a subheadline for an article, just define a subheadline in front matter like this:

`subheadline:  "Subheadline"`

## Introduction to Antara Documentation

Quotes mix it up a little bit, if you write long articles. So use quotes:


## Antara Customizations

Quotes mix it up a little bit, if you write long articles. So use quotes:


## Antara Tutorials

Quotes mix it up a little bit, if you write long articles. So use quotes:


## Antara Modules

Quotes mix it up a little bit, if you write long articles. So use quotes:

> Age is an issue of mind over matter. If you don't mind, it doesn't matter.
<cite>Mark Twain</cite>

<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }

{% highlight html %}
> Age is an issue of mind over matter. If you don't mind, it doesn't matter.
<cite>Mark Twain</cite>
<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }
{% endhighlight %}

# AtomicDEX

You can use comments with *Feeling Responsive* by the way of Disqus. If you want to use Disqus-Comments just open `config.yml` and add your `disqus_shortname`. [More on how to use Disqus ›](https://disqus.com/websites/)

By default comments are turned off. You can customize the default behaviour in `config.yml`. To **turn on comments** just add `comments: true` to front matter using the page layout `layout: page`. 

<small markdown="1">[Up to table of contents](#toc)</small>
{: .text-right }

## Introduction to AtomicDEX Documentation

With foundation responsive videos are easy. [More ›](http://foundation.zurb.com/docs/components/flex_video.html)

<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/WoHxoz_0ykI" frameborder="0" allowfullscreen></iframe>
</div>

## AtomicDEX Setup

dgfgfhfg

## AtomicDEX Tutorials

dgsfdgdsfgss

## AtomicDEX Beta

dgsfdgdsfgsssfd

## AtomicDEX API

dgsfdgdsfgssfdgf


{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->

 [1]: http://kramdown.gettalong.org/converter/html.html#toc
 [2]: {{ site.url }}/blog/
 [3]: http://srobbin.com/jquery-plugins/backstretch/
 [4]: #
 [5]: #
 [6]: #
 [7]: #
 [8]: #
 [9]: #
 [10]: #
