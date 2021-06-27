---
title: ML Storytelling in Python (Part 1)
author: Lucas Forrest
date: '2021-06-27'
slug: ml-storytelling-in-python-part-1
categories: [coding, machine learning]
tags: [coding, machine learning, python]
subtitle: ''
summary: ''
authors: []
lastmod: '2021-06-27T10:32:26-07:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---

## Introduction

Recently I’ve found myself having all sorts of fun as I work with the “big-sleep” python package. Big-sleep combines OpenAI’s CLIP (Contrastive Language-Image Pre-Training) and a GAN (Generative Adversarial Network) to allow a user to enter a text prompt. After the computer has “dreamed” what the picture looks like, it saves the image. 

Some of my favorite images so far are shown below:

### A Sad Man Looking at the River, Oil Painting

Telling the computer specifics about the image seems to lead to better results. For many of the images, I told the computer how to create the image. In this case, I chose to use "Oil Painting."

![A Sad Man Looking at the River, oil painting](images/an_oil_painting_of_a_sad_man_looking_at_the_river.png)

### Alone, Ink on Linen

Single-word statements can be all that is necessary to get a good image. Ink on Linen is one of my favorite styles to use in big-sleep.

![Alone, ink on linen](images/alone_ink_on_linen.png)

### Death and Taxes

After all, only two things in life are truly inevitable. 

![Death and Taxes](images/death_and_taxes.png)

### Mountain, Woodblock Print

Big-sleep also does a great job with woodblock prints. Considering that woodblock prints were incredibly popular during the Edo period in Japan, this isn't that surprising. Narrowing the focus of big-sleep always seems to improve results.

![Mountain, woodblock print](images/mountain_woodblock_print.png)

### Life, Ink on Linen

![Life, ink on linen](images/life_ink_on_linen.png)

### Planes of Edo

![Planes of Edo](images/planes_of_edo.png)
### Solitude 

![Solitude](images/solitude.png)

## Moving One Step Further

Only after I started making these images did I start to question the thought process for the computer. What was the starting picture? How did that image change? Luckily, big-sleep lets you save every part of the process, and stitching the images together allows us to see the dreams taking shape!

### The Persistence of Memory

![The Persistence of Memory](images/the_persistence_of_memory.gif)

## Automation and Moving Forward

One hurdle I faced was the training time. It takes about one and a half hours to dream, so one simple for loop later, and we could now iterate through a list of dreams and keep training the computer, which let me create dreams while I was sleeping (somewhat like the real thing). 

Why stop at just automating the dreams? The next reasonable thing to automate is the list. While creating a tool that could develop prompts was interesting in its own right, it seemed much more interesting to summarize text documents and use those summarizations to prompt the dreams. Then we could give the computer a story and have it draw us the pictures (and give us an abridged version of the story to go along!). 

That's all I have for part one. Once I have a few more pieces of the puzzle put together, we'll see what we can make! If you want to look at the code used for this project, you can [check out the repo on GitHub.](https://github.com/lfrrst/mlstoryteller)
