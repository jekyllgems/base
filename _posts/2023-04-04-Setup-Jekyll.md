---
layout: post
title: How To Setup Ruby & Jekyll
author: leatheresque
categories: jekyll ruby installation
---

# {{ page.title }}
On: {{ page.date | date: "%B %d, %Y" }}
 
{:. .col-lg-8}
* * *

In this post you will learn how to setup Ruby and Jekyll on your Linux server in order to use this theme. I use Ubuntu Linux so I will walk you through setting up on that system. First you need to run:

```bash
sudo apt-get install ruby-full build-essential zlib1g-dev
```

Avoid installing RubyGems packages (called gems) as the root user. Instead, set up a gem installation directory for your user account. The following commands will add environment variables to your `~/.bashrc` file to configure the gem installation path:

```bash
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

Finally, install Jekyll and Bundler:

```bash
gem install jekyll bundler
```

That’s it! You’re ready to start using Jekyll. Read the next guide to learn "How To Configure Your Site _config.yml"