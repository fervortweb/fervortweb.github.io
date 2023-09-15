---
title: "How This Website Build"
published: false
---

This page contains all the details of how this website/blog is created using Github pages.
This will not be visible on website because it is set as published: false in front matter. (See above).
But this page can be visible through github repository https://github.com/fervortweb/fervortweb.github.io

# How to build website using Github pages.

Download https://github.com/mmistakes/mm-github-pages-starter repository and upload everything as it is on https://github.com/fervortweb/fervortweb.github.io . It is also possible to use this repo as template. For future reference, it is forked under our name: https://github.com/fervortweb/mm-github-pages-starter

Delete all pages from _pages directory as these are not needed.

Delete all posts from _posts directory except one post. To know how can a post will be developed in future. But it is set as published: false

In future Blog posts shall be written in _posts directory because this theme and jekyll provide some benefits like paginations, feed (update) etc. But old posts are moved into blog directory to keep same URL as original wordpress blog. These old posts are already rank in google search. 

_config.yml file is modified and unnecessary things are commented like user bio links, footer links. 

Added new scope section in defaults. Search with query FervorT . This is added for blogs inside blog folder. 

_data\navigation.yml is commented to hide top menus.

index.md added on root to hide index.html file. This is because index.html shows pagination of _posts folder but as there are no posts in folder. It is hidden usinf index.md


