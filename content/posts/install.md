---
title: "Installation"
author: subversive.eu
ShowToc: true
tocopen: true
draft: false
categories:
 - Install
date: 2020-10-07T17:44:04+02:00
---

# Prerequisite

- [Install hugo](https://gohugo.io/getting-started/installing/)
- [Make you site](https://gohugo.io/getting-started/quick-start/)

Minimum version of hugo 0.74.0 .

# Install theme

When your website is on. you will install the theme.

Go in the folder /themes/ and run the command :

## by clone


> {{< highlight git >}}
  git clone https://github.com/subversive-eu/hugo-subversive.git
{{< / highlight>}}

To update the theme use this :

> {{< highlight git >}}
cd themes/hugo-PaperMod
git pull
 {{< / highlight>}}

## by submodule

> {{< highlight git >}}
  git submodule add https://github.com/subversive-eu/hugo-subversive.git hugo-subversive
 {{< / highlight>}}

To update the theme use this :

> {{< highlight git >}}
git submodule update --remote --merge
 {{< / highlight>}}

To understand the file configuration checkout, and take attention of [exampleSite](https://github.com/subversive-eu/hugo-subversive/tree/exampleSite)

## configuration 

### theme

In your config file write the name of your folder like this :

config.yml :  
`theme: hugo-subversive`

config.toml :
`theme = "hugo-subversive`

### rest of params

I show you a config.yml.

{{< highlight yml >}}

baseURL: 'https://subversive-eu.github.io/hugo-subversive/'
title: Subversive
author: subversive.eu
paginate: 5
languageCode: en
DefaultContentLanguage: en
enableInlineShortcodes: true
theme: hugo-subversive

# I use this because problems with my github pages.
#uglyurls: true
canonifyURLs: true
#relativeURLs: true

params:
  description: 'Theme Subversive- https://github.com/subversive-eu/hugo-subversive'
  author: subversive.eu
  keyword: 'hugo, hugo-theme, subversive'
  ShowReadingTime: true
  contentTypeName: posts
  ShowShareButtons: true
  comments: false

  homeInfoParams:
    Title: "Rhello \U0001F44B"
    Content: Welcome to the Subversive Theme Demo

  socialIcons:
    - name: rss
      url: 'posts/index.xml'
    - name: github
      url: 'https://github.com/subversive-eu/hugo-subversive'

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

services:
  instagram:
    disableInlineCSS: true
  twitter:
    disableInlineCSS: true

{{< / highlight >}}