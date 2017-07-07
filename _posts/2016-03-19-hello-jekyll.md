---
layout: post
title: Hello Jekyll
author: Deon
disqus_disabled: true
#categories: thoughts
#tags: thoughts
#cover: /assets/instacode.png
---

This is my first official post and I'll keep it short (and sweet), so I thought I'd share my experience on how I got up and running with GitHub Pages and Jekyll.

I have been looking to create a personal site for myself for a while now. I have finally decided to stop looking and just dive into it. I settled upon [GitHub Pages](https://pages.github.com/) and [Jekyll](https://jekyllrb.com/). 

### Why GitHub Pages and Jekyll?

First of all, I like to keep things simple. GitHub Pages is hosted directly from your GitHub repo and you can get blogging with [Jekyll](http://jekyllrb.com/) in no time at all.

### This theme

This theme was created by [Ben Centra](https://github.com/bencentra) - thanks Ben! You can check it out on the [Github repository](https://github.com/bencentra/centrarium).

### Getting started

First off, getting your GitHub repo for your GitHub Pages site was straightforward - the GitHub Pages home page shows you how to get started. Lastly, I had to get my local machine ready for creating and testing my Jekyll site. I run Ubuntu 14.04 LTS, so getting set up wasn't as simple as double clicking on an installer. Fortunately, I found this helpful [guide](http://michaelchelen.net/81fa/install-jekyll-2-ubuntu-14-04/). This guide is very well assembled and the only constraint on how quickly Jekyll will be serving sites on your local machine is your Internet connection. 

Jekyll 3.x requires Ruby version >= 2.0.0, which slightly changes the prerequisites as described in the above mentioned guide.

The two steps to take instead are as follows and were taken from [this](http://stackoverflow.com/questions/33503796/error-installing-jekyll-requires-ruby-2-0-0) SO post.

<h4>1. Install Ruby 2.0</h4>
{% highlight shell %}
sudo apt-get install ruby2.0 ruby2.0-dev
{% endhighlight %}
 
<h4>2. Remove and add symlinks to the new Ruby and Gem binaries</h4>
{% highlight shell %}
sudo rm /usr/bin/ruby
sudo rm /usr/bin/gem
sudo ln -s /usr/bin/ruby2.0 /usr/bin/ruby
sudo ln -s /usr/bin/gem2.0 /usr/bin/gemv
{% endhighlight %}

The step below is only applicable for if you're using the Centrarium theme. 

After cloning the Centrarium template (there is an installation guide) and serving it on Jekyll, the only 'error' message I saw was the following:

<p class="message">
Deprecation: You appear to have pagination turned on, but you haven't included the `jekyll-paginate` gem. Ensure you have `gems: [jekyll-paginate]` in your configuration file.
</p>

The message describes how to resolve it, so it was easy to fix.

Getting started with Jekyll was remarkably simple. 

In closing, using GitHub Pages and Jekyll has been a pleasant experience. I look forward to learn more about Jekyll. Watch this space!

### References

* http://michaelchelen.net/81fa/install-jekyll-2-ubuntu-14-04/
* http://stackoverflow.com/questions/33503796/error-installing-jekyll-requires-ruby-2-0-0


