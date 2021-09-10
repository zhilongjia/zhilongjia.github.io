---
title: 'search txt in image'
date: 2021-09-10
permalink: /posts/2021/09/search_txt_in_image/
tags:
  - search_txt_in_image
  - slides
---

# A shell tool searching txt in lots of images

Days ago, I saw a tool [rclip, AI-Powered Command-Line Photo Search Tool](https://github.com/yurijmikhalevich/rclip), which is interesting to play.

I would like to **search txt in lot of images**, as I have lots of images captured from various slides in many meetings. It will be great if I can search them directly. I made a investigation and found the [tesserat](https://github.com/tesseract-ocr/tessdoc), suitable to this task. 

Notably, in the tesserat, LSTM, instead of CNN, was used, as explained in this article, "Note for beginners: To recognize an image containing a single character, we typically use a Convolutional Neural Network (CNN). Text of arbitrary length is a sequence of characters, and such problems are solved using RNNs and LSTM is a popular form of RNN. "

Based on Tesseract, I coded a script named [search_txt_in_image.sh](https://gist.github.com/zhilongjia/b7a8aeeedb6fca2821ea5c46e90b162c). There are two stages, **OCR** and **searching**. 

* During the OCR stage, it uses Tesseract to OCR txt in figures, which could be several languages, such as English and Chinese. Then it puts the filename of the figures and their txt in a library file, `~/.search_txt_in_image.db`. 
* In th searching stage, it searches the input of interest in the library file with CASE sensitive or not (tuned by parameter `-c`), prints matched filenames of the matched figures and shows the first 5 (tuned by parameter `-t`) figures using the tool [fim](http://www.nongnu.org/fbi-improved/). The searching term could be a regex, recognized by `awk`.


# Examples:

```
# OCR stage
search_txt_in_image.sh -d "~/Picutres"
# OCR multi dirs with figures 
search_txt_in_image.sh -d "~/Picutres ~/pngs"

# OCR and searching stages
search_txt_in_image.sh -d "~/Picutres" "cohort"
search_txt_in_image.sh -d "~/Picutres ~/pngs" "cohort"

# Searching stages
search_txt_in_image.sh cohort
search_txt_in_image.sh 'cohort|gene'
```

# Script available

[search_txt_in_image.sh](https://gist.github.com/zhilongjia/b7a8aeeedb6fca2821ea5c46e90b162c)

# References:

[Deep Learning based Text Recognition (OCR) using Tesseract and OpenCV](https://learnopencv.com/deep-learning-based-text-recognition-ocr-using-tesseract-and-opencv)