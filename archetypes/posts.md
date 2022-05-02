---
title: {{ replace .Name "-" " " | title }}
date: {{ .Date | time.Format ":date_long" }}
draft: true
toc: true
tags: [{{ replace (replace .Dir "posts" "") "/" "" }}]
---

