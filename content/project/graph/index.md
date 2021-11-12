---
title: Order Scheduling in Disk-based Graph Processing
summary: This is a traditional work in graph processing systems. We are trying to reorder tasks to reduce IO overhead in a disk-based graph processing system.
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

Graph processing is a common task that has been researched for many years. You can model many real-world structures in graphs: social networks, web documents … In most of the time, graphs are stored as sparse matrices. But in many real-world problems, sparse matrices are sometimes too large to fit into memory. We may use distributed strategy to resolve this problem. However, recent research has shown that the single machine disk-based method outperforms many distributed ones in many cases. But these disk-based graph processing systems still have a lot of IO overhead. To address this problem, we proposed a new graph task ordering algorithm that can reduce almost 50% of data loading from the disk.


The process of this algorithm is shown in this [slides](/homepage-academic/uploads/Ordering.pdf).


