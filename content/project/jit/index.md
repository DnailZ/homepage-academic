---
title: Leverage JIT Code and Profile Sharing for serverless application 
summary: Modern serverless platform profiles and compiles JIT code in multiple nodes. In this work, we are trying to share runtime profiles and JIT-compiled code in different nodes to accelerate serverless function execution. (click for more details)
tags:
- PL
date: "2016-04-27T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

# image:
  # caption: Photo by rawpixel on Unsplash
  # focal_point: Smart

# links:
# - icon: twitter
#   icon_pack: fab
#   name: Follow
#   url: https://twitter.com/georgecushen
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example
---

The serverless computing model leverages high-level languages, such as JavaScript and Java, to raise the level of abstraction for cloud programming. However, today’s design of serverless computing platforms based on stateless short-lived functions leads to missed opportunities for modern runtimes to optimize serverless functions through techniques such as JIT compilation and code profiling.

We found that modern serverless platforms can not fully leverage language runtime optimizations: Modern serverless platforms can not share JIT-compiled code between different instances. From the picture, we noticed original serverless function can be accelerated by JIT code and profile sharing. 

Working in progress: I'm trying to implement this on HotspotVM. [Draft Paper](/homepage-academic/uploads/draft.pdf) [Implementation Report](/homepage-academic/uploads/JITRelocation.pdf)
