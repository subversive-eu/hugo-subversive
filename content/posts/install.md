---
title: "Installation"
author: subversive.eu
ShowToc: true
tocopen: true
draft: false
categories:
 - Install
date: 2020-10-08T17:44:04+02:00
---

A sample guide tools about installing hugo theme and Configuration.
<!--more-->

# Prerequisite

- [Install hugo](https://gohugo.io/getting-started/installing/)
- [Make your site](https://gohugo.io/getting-started/quick-start/)

Minimum version of hugo 0.74.0 .

# Install theme

When your website is on. You will install the theme.

Go in the folder /themes/ and run the command :

## by clone

```html

git clone https://github.com/subversive-eu/hugo-subversive.git

```

To update the theme use this :

```html

cd themes/hugo-PaperMod
git pull

```

## by submodule

```html

git submodule add https://github.com/subversive-eu/hugo-subversive.git hugo-subversive

```

To update the theme use this :

```html

git submodule update --remote --merge

```

## by download

> On github repository, clic on -code (green button) then download zip.

> Copy and paste the folder in your sitefolder/themes/ rename it by hugo-subversive.


To understand the file configuration checkout, and take attention of [exampleSite](https://github.com/subversive-eu/hugo-subversive/tree/exampleSite)

# config.yml

## theme

In your config file write the name of your folder like this :

config.yml :

`theme: hugo-subversive`

config.toml :

`theme = "hugo-subversive"`

## all params

I show you an example config.yml :


```yml

baseURL: 'https://mywebsite.com/'
title: mywebsite
paginate: 5
theme: hugo-subversive
author: John Mac Artur

languageCode: en
DefaultContentLanguage: en
enableInlineShortcodes: true

enableRobotsTXT: true
buildDrafts: false
buildFuture: false
buildExpored: false

googleAnalytics: UA-423-45

# rise perfomance
minify:
  disableXML: true
  minifyOutput: true

params:
  env: production # enable google analytics, opengraph, twitter-cards and schema.
  title: mywebsite
  description: 'mywebsite's description'
  author: John Mac Artur
  images: "<link or path of image for opengraph, twitter-cards>"
  ShowReadingTime: true
  ShowShareButtons: true
  comments: false
  disableSpecial1stPost : false
  contentTypeName: posts
  disableShare: false
  keyword: 'hugo, hugo-theme, subversive'

  homeInfoParams:
    Title: "Hey \U0001F44B"
    Content: Welcome to my super website !! 

  socialIcons:
    - name: twitter
      url: 'https://twitter.com/'
    - name: stackoverflow
      url: 'https://stackoverflow.com'
    - name: github
      url: 'https://github.com/'

  menu:
    - name: home
      url: '/'
      weight: 5
    - name: info
      url: /about/
      weight: 10
#    - name: tag
#      url: /tags/
#      weight: 15
    - name: categorie
      url: /categories/
      weight: 20
#    - name: serie
#      url: /series/
#      weight: 25
    - name: archive   
      url: /archives/
      weight: 30

sitemap:
  changefreq: dayly
  filename: sitemap.xml
  priority: 0.5

markup:
  tableOfContents:
    endLevel: 3
    ordered: false
    startLevel: 1

taxonomies:
  category: categories
  tag: tags
  series: series

privacy:
  vimeo:
    disabled: false
    simple: true

  twitter:
    disabled: false
    enableDNT: true
    simple: true

  instagram:
    disabled: false
    simple: true

  youtube:
    disabled: false
    privacyEnhanced: true

# RSS feed
rsslimit: 10

```

# Page Variables

In the root directory of your site, go to /archetypes/default.md

This is the schema when you use the command `hugo new posts/mypost.md` or `hugo new photos.md`.  
The default.md is add to your new page.

This is an example :

```yml
---
title: "{{ replace .Name "-" " " | title }}"
author: "{{ .Site.Params.author }}"
ShowToc: true
draft: false
hidemeta: false
disableShare: false
categories:
 - 
date: {{ .Date }}
---

<!--more-->
```

## more options

If you want to personnalize a page you can add this at the top of the page:  

```yml
cover:
 image: '<image path/url>'
 alt: '<alt text>'
 caption: '<text>'
comments: false
description: 'description of your page or article'
tags:
 -
series:
 - 
```

You can use `true or false`.
