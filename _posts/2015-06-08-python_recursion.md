---
layout: post
title: Recursion and variable number of arguments
description: "An example showing recursion along with a function which take variable number of arguments."
modified: 2015-06-08
tags: [recursion, code, python,list unpacking]
---

List unpacking feature can be used to write functions which can ingest variable number of arguments. 
Here is a quick example.

{% highlight python %}
def add(*nums):
    """Add any number of integers together"""
    #print " Num args ", len(nums)
    if len(nums)>1:
        return nums[0] + add(*nums[1:])
    else:
        return nums[0]
    return 0

{% endhighlight %}

Here is the above function in action.
{% highlight python console session %}
In [2]: vals=(3,3,5,6,8,9)

In [3]: add(*vals)
Out[3]: 34

{% endhighlight %}
