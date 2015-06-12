---
layout: post
title: Tuples 
description: "Notes on using tuples in Python"
modified: 2015-06-12
tags: [tuple, code, python]
---

Tuples are number of values seperated by commas. Elements can be of different kinds.

{% highlight python %}
In [1]: m = 12,67,'ping','ding'

In [2]: m
Out[2]: (12, 67, 'ping', 'ding')

In [3]: n=90,100

In [4]: n
Out[4]: (90, 100)

In [5]: new_tuple=m,n

In [6]: new_tuple
Out[6]: ((12, 67, 'ping', 'ding'), (90, 100))
{% endhighlight %}


A tuple can have lists as its elemets
{% highlight python %}
>>> lt= [1,2,3],[4,5,6]
>>> lt
([1, 2, 3], [4, 5, 6])
>>> 
{% endhighlight %}

Now, one may ask, what's the difference between using tuples vs list ??

| Tuples | Lists|
|:--------|:-------:|
|immutable| mutable|
|Generally hetrogeneous| generally homogeneous|
|Generally accessed by unpacking or indexing | Generally iterated over|
|=====
