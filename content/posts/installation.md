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

To use it add this :

```yml

languageCode: fr  
DefaultContentLanguage: fr

```
to your [config.yml](https://github.com/subversive-eu/hugo-subversive/blob/exampleSite/config.yml) :

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


If you just want a list of post + Title, delete it in config.yml  
Or do not copy it.

---

## Markdown

The full markdownsyntax.md [here](https://raw.githubusercontent.com/subversive-eu/hugo-subversive/exampleSite/content/posts/markdownsyntax.md). Use it to fund how to deploy your content.

### Blockquote

* [Example hard level](https://subversive-eu.github.io/hugo-subversive/posts/markdownsyntax/#blockquote-hard)
* [Sample example](https://subversive-eu.github.io/hugo-subversive/posts/markdownsyntax/#blockquote-sample)


> [blockquote.html](https://github.com/subversive-eu/hugo-subversive/blob/main/layouts/shortcodes/blockquote.html)

### Image and Figure

#### Image

css : image-css

> [render-image.html](https://github.com/subversive-eu/hugo-subversive/blob/main/layouts/_default/_markup/render-image.html)

#### Figure

**I recommand you to use this because it's responsive and beautifull !!**

* [Example](https://subversive-eu.github.io/hugo-subversive/posts/markdownsyntax/#figure)

### Render-Link

css : sources-link

> [render-link.html](https://github.com/subversive-eu/hugo-subversive/blob/main/layouts/_default/_markup/render-link.html)

### Pdf Reader

Use shortcode ```{{< iframepdf nameofyourpdf >}}```

> ```\static\media\nameofyourpdf.pdf```

> [iframepdf](https://github.com/subversive-eu/hugo-subversive/blob/main/layouts/shortcodes/iframepdf.html)

### Button

Use shortcode :

```go

{{< button href="Link.com" class="" >}}Display Content{{< /button >}}

```

* [Example](https://subversive-eu.github.io/hugo-subversive/posts/markdownsyntax/#buttons)

> [button](https://github.com/subversive-eu/hugo-subversive/blob/main/layouts/shortcodes/button.html)

### Tab/Tabs

Use shortcode. Check markdownsyntax.md

* [Example](https://subversive-eu.github.io/hugo-subversive/posts/markdownsyntax/#tabs)

> [Tab](https://github.com/subversive-eu/hugo-subversive/blob/main/layouts/shortcodes/tab.html)
> [Tabs](https://github.com/subversive-eu/hugo-subversive/blob/main/layouts/shortcodes/tabs.html)

### Details

Use shortcode. Check markdownsyntax.md

* [Example](https://subversive-eu.github.io/hugo-subversive/posts/markdownsyntax/#details)

> [Details](https://github.com/subversive-eu/hugo-subversive/blob/main/layouts/shortcodes/details.html)

### Columns

Use shortcode. Check markdownsyntax.md

* [Example](https://subversive-eu.github.io/hugo-subversive/posts/markdownsyntax/#colunms)

> [Columns](https://github.com/subversive-eu/hugo-subversive/blob/main/layouts/shortcodes/columns.html)

### Copy button

There is a copy button for code text ```class="highlight"```.

> [Check script.js](https://github.com/subversive-eu/hugo-subversive/blob/main/assets/js/script.js)


### other shortcodes

- rawhtml.html
- collapse.html 

---

## Cover Image

Used to add a post header image.

```cover: "https://i.ibb.co/K0HVPBd/paper-mod-profilemode.png"```

With a direct link like this |^ .
Or a file from your ```\static\media\nameofyourfile.pdf```

## SVG icons tricks

You can add, what you want.

Check the [list of icons](https://subversive-eu.github.io/hugo-subversive/posts/utilisation/) or add some in ```/your-theme/layouts/partials/svg.html```

### Social-icons

This params will appear in the middle of the sidebar.

> In config -> name: nameofsvg.  

{{< highlight yml >}}
 params:  
  socialIcons:  
   - name: rss  
    url: 'posts/index.xml'  
   - name: github  
     url: 'https://github.com/subversive-eu/hugo-theme-subversive'  
{{< / highlight >}}

### Page-icons

Main menu : 

{{< highlight yml >}}
  params:
   menu:
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
