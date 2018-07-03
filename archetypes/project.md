---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: true
description: "Project Description. Tagline in /projects page"
author: ~
weight: 10 # higher = lower on list
draft: false
toc: false
callout: |
  **ProjectName** is a thing that does things well.
  
github_url: "#"
app_url: "#"
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

<!-- Project Description or README Goes Here -->