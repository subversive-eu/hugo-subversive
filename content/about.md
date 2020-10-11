---
title: "About"
author: subversive.eu
ShowToc: true
draft: false
hidemeta: true
tocopen: true
disableShare: true
date: 2020-10-01T08:37:55+02:00
type: myabouttype
url: "/about/"
---

## /about/

Example of using yousite.com/about/ with :  

ShowToc: true  
hidemeta: true  
tocopen: true  
disableShare: true  

The html of this page.md comes from /layouts/_default/single.html  

For this page, you can use in post data :

```yml
type: myabouttype
url: "/about/"
```

Same than archive.md

Html will come from `/layouts/myabouttype/single.html`  You have to make it and personnalize.

## /archives/

/archives/ come from `/layouts/myarchivetype/single.html`.  
So, it's become easier to css and personnalize.

## command

`hugo new about.md`  
`hugo new photos/africa.md`
