---
layout: post
title: Installing Jekyllgems Themes On Your Site
author: leatheresque
categories: themes
---

# {{ page.title }}
On: {{ page.date | date: "%B %d, %Y" }}
 
{:. .col-lg-8}
* * *

If you already have a site installed on your server and you want to use one of my themes, you should save your posts first. Save your data files, and then in your Gemfile edit the line where you find this comment:

```yaml
# This is the default theme for new Jekyll base site 
# You may change this to anything you like.

gem "jekyll-base"
```

It may be some other gem being used if you have already been running a site. Just change it to `jekyll-base` and when you run `bundle install` it will pull the gem you need along with the files you need and install everything. Then you run `bundle exec jekyll serve` and it will serve up your site.