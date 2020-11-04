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

## youtube

/ cf layouts/shortcodes/youtube.html

{{< youtube "8IZ9Cqi2rGM" >}}

## tweeter

{{< tweet 877500564405444608 >}}

## vimeo

* Not worked 

{{< vimeo 146022717 >}}

## Instagram

* there is no way with facebook ...

## Blockquote

Normal quote:
{{< blockquote >}}
  This is a simple quote.
{{< /blockquote >}}

Quote with author
{{< blockquote author="Author2" >}}
  This is a quote with only an Author named Author2.
{{< /blockquote >}}

Quote with author and source
{{< blockquote author="Author3" source="Source" >}}
  This is a quote from Author3 and source "source."
{{< /blockquote >}}

Quote with author and link
{{< blockquote author="Author4" link="https://www.google.com" >}}
  This is a quote from Author4 and links to https://www.google.com.
{{< /blockquote >}}

Quote with author, link and title
{{< blockquote author="Author5" link="https://www.google.com" title="Google" >}}
  This is a quote from Author5 and links to https://www.google.com with title "Google."
{{< /blockquote >}}

Quote with author and a link longer than 32 characters, string is first cut at 32 characters then everything after the last forward slash is removed
{{< blockquote author="Author6" link="https://twitter.com/CryptoGangsta/status/716427930126196737" >}}
  This is a quote from Author5 and links to https://twitter.com/CryptoGangsta/status/716427930126196737 which is longer than 32 characters.
  <br>And this is a new line in the quote with the HTML br tag.
{{< /blockquote >}}

Test from the Octopress blockquote page at: http://octopress.org/docs/plugins/blockquote/
{{< blockquote author="@allanbranch" link="https://twitter.com/allanbranch/status/90766146063712256" >}}
  Over the past 24 hours I've been reflecting on my life & I've realized only one thing. I need a medieval battle axe.
{{< /blockquote >}}
---

## iframe for pdf

- just put the name of you pdf file, and paste it in /static/media/

{{< iframepdf gt-metrix-report >}}

# Conclusion

Do not use Instagram ? or Vimeo ? I hope will work on soon.
