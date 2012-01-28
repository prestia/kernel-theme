---
layout: post
category : projects
tags : [toto, dodo, github, html5]
title: dodo&#58; A Template for toto
project: dodo
---
{% include JB/setup %}

## What is dodo?

Dodo is a personal blogging template for the compact, hacker-friendly blog engine [toto](http://github.com/cloudhead/toto). Dodo looks beautiful and degrades gracefully thanks to [HTML5 Boilerplate](http://html5boilerplate.com/), [jQuery](http://jquery.com/), [modernizr](http://www.modernizr.com/), [hyphenator.js](https://code.google.com/p/hyphenator/), and [highlighter.js](http://softwaremaniacs.org/soft/highlight/en/). All posts are written in [John Gruber](http://daringfireball.net/)'s excellent [markdown](http://daringfireball.net/projects/markdown/) syntax and published to [Heroku](http://heroku.com/) using [git](http://git-scm.com/).

Dodo was written by [Anthony Prestia](http://anthonyprestia.com) and you can see it in action on his (now retired) [personal blog](http://blog.anthonyprestia.com).

## Want to try dodo?

Assuming you are already a [GitHub](http://github.com) and [Heroku](http://heroku.com) user, setup takes less than 10 seconds:

    $ git clone git://github.com/prestia/dodo.git <blog_name>
    $ cd <blog_name>
    $ heroku create <blog_name>
    $ git push heroku master

## Configuration

Once installed, you can configure dodo by modifying the `config.ru` file. The default options are as follows:

    set :blog_title,   ''  # main blog title
    set :author,       ''  # blog author
    set :root,         "index"  # page to load on /
    set :markdown,     :smart  # use markdown + smart-mode
    set :disqus,       ''  # disqus id, or false
    set :fulltext,     ''  # for index, true or false
    set :summary,      :max => 150, :delim => /~/
    set :ext,          'txt'  # file extension for articles
    set :cache,        28800  # cache duration, in seconds

    set :git,          false  # github username
    set :twitter,      false  # twitter username
    set :description,  ''  # default blog description
    set :main_url,     ''  # main, non-blog url
    set :analytics,    ''  # your site's Google Analytics ID

    set :date,         lambda {|now| now.strftime("%B #{now.day.ordinal} %Y") } # date format for articles


## Problems?

Dodo is a work in progress. While it is perfectly stable, some code is still a bit messy and there may be some layout hiccups. If you have any problems using [dodo](http://github.com/prestia/dodo), please submit them [here](https://github.com/prestia/dodo/issues).