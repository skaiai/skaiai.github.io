---
layout: post
title: "[Paper] State-of-the-art speech recognition with sequence-to-sequence models"
tags: paper seq2seq end2end 
categories: speech-recognition
comments: true
---
last update: 2018-09-20    
paper: [State-of-the-art speech recognition with sequence-to-sequence models (Feb 2018)](https://static.googleusercontent.com/media/research.google.com/ko//pubs/archive/46687.pdf)
<!--[example pic]({{ site.baseurl }}/assets/images/post_180920/header.png= 250x)-->
<img name="header" img src="{{ site.baseurl }}/assets/images/post_180920/header.png" width="600">

# Intro
improved version of LAS model
* structural side
	* words instead of graphemes
	* multi-head attention instead of a single-head one 
* optimization side
	* synchronous training
	* scheduled sampling
	* label smoothing
	* minimum word error rate optimization
