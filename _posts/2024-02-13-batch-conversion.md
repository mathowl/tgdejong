---
layout: post
title: Batch image conversion
date: 2024-02-12 08:51:00-0400
description: cmd conversion of files with specific extensions
tags: imagemagick
categories: code
related_posts: false
---

Conversion of images can be a drag. Luckily [Imagemagick](https://imagemagick.org/index.php) supports batch conversion. ``cd`` to the designated folder and type ``magick mogrify -format jpg -quality 100 *.png`` to convert all .png files to .jpg files. 
