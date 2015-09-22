---
layout: post
title: "Recursion In Ruby"
description: "DBC week 8 tech blog"
modified: 2014-08-24 14:28:16 -0700
tags: [dev bootcamp, web development, DBC, blog, jekyll, shane biggs]
image:
  feature: abstract-5.jpg
  credit: dargadgetz
  creditlink: http://www.dargadgetz.com/ios-7-abstract-wallpaper-pack-for-iphone-5-and-ipod-touch-retina/ 
comments: true
share: true
---
### What is recursion? 

Today we are going to discuss recursion in regards to Ruby code. So what is recursion? Recursion in its most simplified state is a function that calls itself from within the same function. In Ruby the method would call itself from within the same method. Below is a simple example of a Ruby method "countdown" which shows us how recursion works.

{% highlight ruby %}
def countdown(n)
  return if n.zero?   # base case
  puts n
  countdown(n-1)      # getting closer to base case    
end               

countdown(5)
5
4
3
2
1
{% endhighlight %}
<a href="http://stackoverflow.com/questions/6418017/what-is-ruby-recursion-and-how-does-it-work" target="_blank" title="Source">Source</a>

In the example above the Ruby method countdown calls itself from inside the same method. For the recursive algorithm to terminate you need a base case so the method will stop calling itself. The base case above is zero. So when the algorithm reaches 0 it will terminate and stop running the code. 

You can see how this could be problematic. Recursion if not used properly can cause major issues in your code. For example if the recursion is too large you could end up with stack overflows (using up allowed memory). Recursion can be completed using normal Ruby loops that are not as dangerous. But to an experienced coder recursion can be a very powerful tool. Ruby coders often use recursion to elegantly express mathematical methods. So be careful when using recursion in your Ruby code.