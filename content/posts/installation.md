---
title: "Installation tricks"
author: subversive.eu
ShowToc: true
draft: false
categories:
 - install
date: 2020-09-30T17:44:04+02:00
---

Hey, I will give you some tricks to make your website. 
<!--more-->

## Favicons 

I used this <https://favicon.io/favicon-generator/>

### Deploy

First, download files listed below :  
Paste the file in themes/your-theme/static/

```html
    android-chrome-192x192.png
    android-chrome-512x512.png
    apple-touch-icon.png
    favicon-16x16.png
    favicon-32x32.png
    favicon.ico
    site.webmanifest
```

That's all !

---

## i18 Language

To use it, just add and use in [config.yml](https://github.com/subversive-eu/hugo-subversive/blob/exampleSite/config.yml) :

languageCode: fr  
DefaultContentLanguage: fr

There is three languages : French(fr), English(en) (default), Spanish(es). 

Check in themes/your-theme/i18n/ [here](https://github.com/subversive-eu/hugo-subversive/tree/main/i18n)

____

## Home Page

If you want to introduce your website :  
 * Do not touch in params:  
    homeInfoParams:  
        Title: Hi there wave  
        Content: Can be Info, links, about...  

* If you just want a list of post + Title, delete it in config.yml  

***

## Markdown

### Youtube

There is a shortcode for youtube video without cookie, and privacy (Only European) cf [hugo-privacy-settings](https://gohugo.io/about/hugo-and-gdpr/#all-privacy-settings).

For css /your-theme/layouts/shortcodes/youtube.html

### Image 

For css /your-theme/layouts/_default/_markup/render-image.html

### links

For css /your-theme/layouts/_default/_markup/render-link.html

### others shortcodes

rawhtml.html + collapse.html + blockquote.html

---

## Menu with svg icons

You can add, what you want.
Follow the [list of icons]() or add some in /your-theme/layouts/partials/svg.html

### Right-menu | SocialIcons

This params will appear in the right of the menu.
name: name of svg.

```
* params:  
 * socialIcons:  
    - name: rss  
      url: 'posts/index.xml'  
    - name: github  
      url: 'https://github.com/subversive-eu/hugo-theme-subversive'  
```

### Left-menu | PageIcons

Main menu, in the left.

```
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
```

<hr>