---
title: "Example"
author: subversive.eu
ShowToc: true
draft: true
categories:
 - Example
date: 2020-09-27T17:44:04+02:00
---

I will show you some extras about Markdown, css, and shortcodes.
There is savegame of simple tricks too.

<!--more-->

# Image

![Drag Racing](/media/logo.png "coucou")

![](/media/roman300AD.png "roman empire")

## PostMeta

I added this to my personnal website

```html
      <!--- This is the end of meta. not for me. I add some download options + printer option -->
      &nbsp;·&nbsp;
      <button class="sample-btn">
      <a name="Télécharger" href="/pdf/{{ .Title }}.pdf" target="_blank" rel="noopener noreferrer" download>{{ i18n "pdf" }}</a>
      </button>&nbsp;·&nbsp;<button class="sample-btn">
      <a name ="Imprimer" href="javascript:if(window.print)window.print()">{{ i18n "print" }}</a>
      </button>&nbsp;·&nbsp;<button class="sample-btn">
        <a name="Télécharger" href="/epub/{{ .Title }}.epub" target="_blank" rel="noopener noreferrer" download>{{ i18n "ebook" }}</a>
      </button>&nbsp;·&nbsp;
```

* Do not forget to add i18n translation for all languages

## youtube

/ cf layouts/shortcodes/youtube.html

{{< youtube "8IZ9Cqi2rGM" >}}

## tweeter

{{< twitter 877500564405444608 >}}


## vimeo

{{< vimeo 146022717 >}}

## Instagram

/ Hidingcaption

{{< instagram BWNjjyYFxVx hidecaption >}}

{{< instagram BWNjjyYFxVx >}}

---

# Conclusion

Do not use Instagram ? or Vimeo ? I hope will work on soon.
