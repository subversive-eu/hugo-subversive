---
title: "Installation tricks"
author: subversive.eu
ShowToc: true
draft: false
categories:
 - install
date: 2020-10-06T17:44:04+02:00
---

Hey, I will give you some tricks to make your website. 
<!--more-->

## Favicons 

I used this <https://favicon.io/favicon-generator/>

### Deploy

First, download files listed below :

Paste the files in themes/your-theme/static/  

{{< highlight html >}}

    android-chrome-192x192.png
    android-chrome-512x512.png
    apple-touch-icon.png
    favicon-16x16.png
    favicon-32x32.png
    favicon.ico
    site.webmanifest

{{< / highlight >}}

That's all !

---

## i18 Language

To use it, just add and use in [config.yml](https://github.com/subversive-eu/hugo-subversive/blob/exampleSite/config.yml) :

languageCode: fr  
DefaultContentLanguage: fr

There is three languages : French(fr), English(en), Spanish(es). 

I don't know if there is default language. Be carefull.

Check in themes/your-theme/i18n/ - [here](https://github.com/subversive-eu/hugo-subversive/tree/main/i18n)

____

## Home Page

If you want to introduce your website : 

* Do not touch in params :

>{{< highlight yml >}}
  homeInfoParams:  
      Title: Hi there wave  
      Content: Can be Info, links, about...  
{{< / highlight >}}


* If you just want a list of post + Title, delete it in config.yml  

***

## Markdown

### Youtube

Youtube video without cookie, and privacy (Only European).

> [hugo-privacy-settings](https://gohugo.io/about/hugo-and-gdpr/#all-privacy-settings).

### Image 

> /your-theme/layouts/_default/_markup/render-image.html

### links

> /your-theme/layouts/_default/_markup/render-link.html

### other shortcodes

- rawhtml.html
- collapse.html 
- blockquote.html
- iframepdf.html

> {< iframepdf doc_name >}

---

## Menu with svg icons

You can add, what you want.

Check the [list of icons](https://subversive-eu.github.io/hugo-subversive/posts/utilisation/) or add some in /your-theme/layouts/partials/svg.html

### Right-menu | Social-icons

This params will appear in the right of the menu.

> In config -> name: nameofsvg.  

{{< highlight yml >}}
* params:  
 * socialIcons:  
    - name: rss  
      url: 'posts/index.xml'  
    - name: github  
      url: 'https://github.com/subversive-eu/hugo-theme-subversive'  
{{< / highlight >}}

### Left-menu | Page-icons

Main menu, in the left.  

{{< highlight yml >}}
* params:
 * menu:
    - name: home
      url: '/'
      weight: 5
    - name: info
      url: /about/
      weight: 10
    - name: tag
      url: /tags/
     weight: 15
    - name: categorie
      url: /categories/
      weight: 20
    - name: serie
      url: /series/
      weight: 25
    - name: archive   
      url: /archives/
      weight: 30
{{< / highlight >}}

---
