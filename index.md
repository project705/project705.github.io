---
layout: default
title: "Engineering Blog"
---

# GitHub Blog Entries

{% for post in site.posts %}

{{ post.date | date: "%-d %B %Y" }} - [{{ post.title }}]({{ post.url }})

{% endfor %}

# How To Preview and Submit a Blog Entry

This site is hosted on [GitHub Pages](https://pages.github.com/) and uses [Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll) to generate the site HTML from markdown.

## Ubuntu/Linux

First, clone the github pages repo.  Then, to make and preview edits locally, install, and start [Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll):

```
cd $GITPAGES_DIR
sudo apt-get install bundler jekyll rails
sudo bundle install
bundle exec jekyll serve
```

You should now be able to preview your site locally at `http://127.0.0.1:4000`.  Note that the Jekyll server should automatically pick up edits upon save via inode notify.
