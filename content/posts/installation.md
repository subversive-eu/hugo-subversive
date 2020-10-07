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

## Favicons 

I used https://favicon.io/favicon-generator/

### Installation

First, use the download button to download the files listed below. Paste the file in themes/your-theme/static/

    android-chrome-192x192.png
    android-chrome-512x512.png
    apple-touch-icon.png
    favicon-16x16.png
    favicon-32x32.png
    favicon.ico
    site.webmanifest

That's all !

---
## i18 Language

To use it, just add and use in config.yml :

languageCode: fr
DefaultContentLanguage: fr

There is three languages : French, English (default), Spanish. 

Check in themes/your-theme/i18n/

---

## Home Page

* If you want to introduce your website :
    Do not touch.
    homeInfoParams:
        Title: Hi there wave
        Content: Can be Info, links, about...

* If you just want a list of post, delete it in config.yml

---

## Markdown

### Youtube

There is a shortcode for youtube video without cookie, and privacy (Only European) cf [all privacy settings -hugo](https://gohugo.io/about/hugo-and-gdpr/#all-privacy-settings)

For css /your-theme/layouts/shortcodes/youtube.html

### Image 

For css /your-theme/layouts/_default/_markup/render-image.html

### links

For css /your-theme/layouts/_default/_markup/render-link.html

### others shortcodes

rawhtml + collapse + blockquote
