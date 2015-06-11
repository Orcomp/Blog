---
layout : post
title : Image Annotations
category : Useful
tags :
  - Documentation
  - Annotations
---

## Problem statement

Add annotations to an image. The annotations should be in a separate file to the image.

Images will be viewed in HTML pages as part of documentation.

The problem comes from taking lots of pictures of GUIs, which tend to change a lot. I want a solution that would allow me to update images without having to annotate them manually all over again. That is why I would like to keep the annotations in a separate file and have the whole process automated.

## Solutions

- Annotate in svg and save the svg image
- Use Javascript ([Raphaeljs](http://raphaeljs.com/))

## Links

- [Annotorious](http://annotorious.github.io/)
- Reduce the size of png images: http://antix.co.uk/Projects/Nibbler
- Screen capture that can call an external program to post process. Ideal for slicing up images. [Screenshot Captor](https://www.donationcoder.com/Software/Mouser/screenshotcaptor/)


## Image slicer

Looked everywhere on the internet and could not find a simple image slicer.
Turns creating one from scratch is not too hard.

In this case I am using imageMagick to crop the same image multiple times.