---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: false
toc: true
author: "{{ .Site.Params.author.writterName }}"
authorlink: "{{ .Site.Params.author.writterLink }}"
tags: [""]
---
