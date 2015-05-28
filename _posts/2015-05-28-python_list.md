---
layout: post
title: Python list Comprehension
description: "Some info about Python list Comprehensions feature."
modified: 2015-05-28
tags: [sample post, code, highlighting]
image:
  feature: abstract-10.jpg
  credit: dargadgetz
  creditlink: http://www.dargadgetz.com/ios-7-abstract-wallpaper-pack-for-iphone-5-and-ipod-touch-retina/
---

Python list comprehensions can be used to create lists in a very natural way. 
To create a list, think of the formulae or relationship between each item. 

{% highlight python %}
SQ = [x**2 for x in range(20)]
V = [2**i for i in range(10)]
{% endhighlight %}

This will create the following output 
{% highlight python console session %}
>>> SQ = [x**2 for x in range(20)]
>>> SQ
[0, 1, 4, 9, 16, 25, 36, 49, 64, 81, 100, 121, 144, 169, 196, 225, 256, 289, 324, 361]
>>> V = [2**i for i in range(10)]
>>> V
[1, 2, 4, 8, 16, 32, 64, 128, 256, 512]
{% endhighlight %}