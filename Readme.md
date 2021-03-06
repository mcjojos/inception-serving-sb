# Zero to image recognition in 60 seconds with Tensorflow and Spring Boot 

[![Build Status](https://travis-ci.org/florind/inception-serving-sb.svg?branch=master)](https://travis-ci.org/florind/inception-serving-sb)
[![Coverage Status](https://coveralls.io/repos/github/florind/inception-serving-sb/badge.svg?branch=master)](https://coveralls.io/github/florind/inception-serving-sb?branch=master)

TL;DR: for the impatient ones wanting to have a web service for image recognition without any Tensorflow prerequisites: run ```./gradlew fetchInceptionFrozenModel bootrun```, navigate to http://localhost:8080 and upload an image. The backend will categorize the image and output the result along with the probability.

Screenshot (non clickable)<br/>
<div align="center" style="text-align:center"><img src="cat_classified.jpg" width="560"/></div>

## Why
Tensorflow is hard enough to wrap one's head around. It has several parts that deal with preparing data, defining and training a model and finally, outputting a model that can then be used to categorize (infer) other data. There's math involved, new vocabulary to learn and on top, a toolchain which revolves around Python.
This project only addresses serving a Tensorflow pre-trained image categorization model, otherwise called the Inception model.  

## Prerequisites
- JDK 8

## Run
```./gradlew fetchInceptionFrozenModel bootrun```

Navigate to http://localhost:8080 and upload an image. The backend will categorize the image and output the result along with the probability.

## How
Head to [the blog post](https://blog.newsplore.com/2017/07/31/zero-to-image-recognition-in-60-seconds-with-tensorflow-and-spring-boot) for the ful monty.
