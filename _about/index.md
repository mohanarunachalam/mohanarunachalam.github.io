---
layout: default
title: "About me"
description: "My job and project experiences"
category: introduction
---
<br/>
<img class="profile-picture" src="mohan.jpg">

I am a Deep Learning consultant at a EduTech startup, based out of Hyderabad,India.

Previously, I worked as a Applied Research Fellow with [Prof. C.V.Jawahar](https://faculty.iiit.ac.in/~jawahar/) at [CVIT,IIIT-Hyderabad](https://cvit.iiit.ac.in/). I worked on projects involving automating the evaluation of handwritten student assignments. I worked on the webapp development part of the project using Django and Python.

Prior to that, I worked at [Cognitivescale](https://www.cognitivescale.com/) on data ingestion pipeline, recommendation apis and test automation. I have also worked on continuous integration pipeline.

I graduated from [BITS PILANI, Hyderabad Campus](http://www.bits-pilani.ac.in/hyderabad/) in 2016 with a Master's Degree (M.E) in Computer Science with specialization in Information Security.

## Research Interest

My interest lies in the fields of Computer Vision and Machine learning. Recent interest is in applying reinforcement learning techniques in games like Rubik's cube.

<br/>

## News

<table>
{% for article in site.data.news %}
<tr>
{% include news.html %}
</tr>
{% endfor %}
</table>
