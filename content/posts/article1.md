---
title: "Article1"
author: subversive.eu
ShowToc: true
draft: true
hidemeta: false
tocopen: false
disableShare: false
categories:
 - Démocratie
date: 2020-09-30T17:44:04+02:00
cover: "https://i.ibb.co/K0HVPBd/paper-mod-profilemode.png"
---

This is an example and a work base for trying new feature
Cet article permet de tester des markups, des shortcodes, des variables et environnements

<!--more-->
## Image

### Classic markdown

![Drag Racing](/media/logo.png "coucou")

![](/media/roman300AD.png "roman empire")

### figure shortcode with css

{{< figure src="/media/logo.png" alt="image" caption="coucou" class="no-class" >}}

{{< figure src="/media/roman300AD.png" alt="image" caption="roman empire" class="no-class" >}}

It's better no ??  
Let's check more !


Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.


{{< figure src="https://via.placeholder.com/400x280" alt="image" caption="figure-right" class="right" >}}
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

{{< figure src="https://via.placeholder.com/400x280" alt="image" caption="figure-left" class="left" >}}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
{{< figure src="https://via.placeholder.com/1600x800" alt="image" caption="figure-normal (without any classes)" >}}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

{{< figure src="https://via.placeholder.com/1600x800" alt="image" caption="figure-big" class="big" >}}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## PostMeta

links :  
<a name="Télécharger" href="/pdf/{{ .Title }}.pdf" target="_blank" rel="noopener noreferrer" download>télécharger le pdf</a>
&nbsp;·&nbsp;
<a name ="Imprimer" href="javascript:if(window.print)window.print()">imprimer</a>
&nbsp;·&nbsp;
<a name="Télécharger" href="/epub/{{ .Title }}.epub" target="_blank" rel="noopener noreferrer" download>télécharger format epub</a>

## Cover for a post

cover = "<absolute image url>"
  can also paste direct link from external site
  ex. https://i.ibb.co/K0HVPBd/paper-mod-profilemode.png

/ Permet d'ajouter une image au post.

## youtube

{{< youtube DWcJFNfaw9c >}}

## tweeter

{{< tweet 877500564405444608 >}}

## vimeo

{{< vimeo 146022717 >}}

## Footer hugo theme

<span>Powered by <a href="https://gohugo.io/" rel="noopener noreferrer" target="_blank">Hugo️️</a>️</span>
<span>&middot;</span>
<span>Theme️ <a href="https://git.io/hugopapermod" rel="noopener" target="_blank">PaperMod</a></span>
