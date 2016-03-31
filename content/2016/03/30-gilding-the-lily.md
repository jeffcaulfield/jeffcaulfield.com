date: 2016-03-30
#forum: True
title: Gilding the Lily
template: post.haml
---
I'm writing my own static site generator. What could possibly go wrong?
---

I tried a variety of static site generators on my way to rebuilding my personal website: [hexo](https://hexo.io/), [hugo](https://gohugo.io/) and [sculpin](https://sculpin.io/), just to name a few. These all seem very complicated for what they purport to be, and definitely overkill for my needs.

Eventually, I stumbled across [embellish](http://boscoh.github.io/embellish/). It's very lightweight. It doesn't require a ton of files to get started. It's written in [Python](https://www.python.org/). I was able to get something off the ground quickly without getting bogged down in excessive detail.

There's still some "fat" that could yet be trimmed, I feel. I  don't understand the need to use [Haml](http://haml.info/) for templates when [Jinja](http://jinja.pocoo.org/) is fine on its own. I'm not using compiled assets ([CoffeeScript](http://coffeescript.org/), [Sass](http://sass-lang.com/) and so forth), although that's not to say that I might not want to later on. I'd like the command-line to auto-detect "site.yaml" when it is present. I'd also like to remove or at least rename the "site.cache" file.

At the same time, there are a few small but important features that are missing. A [sitemap](http://www.sitemaps.org/) and a syndication feed ([Atom](http://atomenabled.org/) and/or [RSS](http://www.whatisrss.com/) format) should be automatic. Pagination might be useful for large archive indexes. I'd also like a simple way to add site-specific extensions (Python scripts) to customise the render process.

This all seems acheivable. I think I'll call it [gild](https://github.com/jeffcaulfield/gild) as in "gilding the lily" in keeping with the theme of embellishment.

What could *possibly* go wrong?
