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
|Immutable| Mutable|
|Generally hetrogeneous| Generally homogeneous|
|Generally accessed by unpacking or indexing | Generally iterated over|
|=====

### Tuple unpacking 
we can unpack a tuple to get individual elements
{% highlight python %}
>>> m=(3,7,9)
>>> x,y,z = m 
>>> x
3
>>> y
7
>>> z
9
{% endhighlight %}
Note that the number of variables on right hand side should match the length of tuple.

A tuple can be converted to list by using list() 
{% highlight python %}
>>> ll = list(m)
>>> ll
[3, 7, 9]
{% endhighlight %}