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

## configuration

In your config file write the name of your folder like this :

`theme: hugo-subversive`

