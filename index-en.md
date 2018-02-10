---
#
# Here you can change the text shown in the Home page before the Latest Posts section.
#
# Edit jekyll-theme-simple-blog's home layout in _layouts instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: home
permalink: /index.html
header:
  image: /assets/img/home-header.jpg
tagline: > # this means to ignore newlines until "repository:"
  Human being writing code for living. In love with Ruby and Ruby on Rails
excerpt: >
  Write an awesome description for your new site here. You can edit this
  line in index.md. It will appear in your document head meta (for
  Google search results) and in your feed.xml site description.
repository:
  is_project_page: false
  show_downloads: false
ref: home
lang: en
---

Experienced Software Engineer with a demonstrated history of working in the information technology and services industry. Writes code in Ruby and builds promising web applications and services in Ruby on Rails. Strong engineering professional with a Bachelor's Degree focused in Computer Science and Engineering from College of Engineering Thalassery.

<h2>Latest Articles</h2>
<div>&nbsp;</div>
{% include list-category-posts.html lang=page.lang category="articles" %}

---

<h2>Latest Projects</h2>
<div>&nbsp;</div>
{% include list-category-posts.html lang=page.lang category="projects" max=1 %}
