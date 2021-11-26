---
title: JFass - A New Serverless Platform with Customized JVM Runtime
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

Faas (Function as a service) is one form of serverless computing where users only need to deploy function on the cloud and the cloud service vendor will handle all the hardware resources the function needs. The vendor will provide runtimes for these functions which are driven by events. However, Faas is tailored for short-lived functions which makes traditional runtime optimizations such as JIT compilation fail to enhance performance. We want to design a new framework to bridge the gap between modern language runtime and serverless platforms.

In this work, we aim at building a new serverless platform tailored for JVM runtime with profile information sharing and native code sharing across nodes. We also hope to use hardware tracing technology to help reduce profiling overhead from interpreter stage.

Working in progress: I'm trying to implement this on HotspotVM. [Draft Paper](/homepage-academic/uploads/draft.pdf) [Implementation Report](/homepage-academic/uploads/JITRelocation.pdf)
