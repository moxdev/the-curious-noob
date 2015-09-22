---
layout: post
title: "Ruby: {Hash} vs [Array]"
description: "DBC week 4 tech blog"
modified: 2014-08-18 21:33:04 -0700
tags: [dev bootcamp, web development, DBC, blog, jekyll, shane biggs]
image:
  feature: abstract-5.jpg
  credit: dargadgetz
  creditlink: http://www.dargadgetz.com/ios-7-abstract-wallpaper-pack-for-iphone-5-and-ipod-touch-retina/ 
comments: true
share: true
---

### Ruby Array and Hash Structure

I selfishly chose the topic of Hash's and Array's in the hopes that after creating this blog you and I would both be more educated on the subject so lets begin! 

Both arrays and hashes are a rather simple way for Ruby to store a list of items called "elements." The list of elements contained in each format can be comprised of many different types of things, or as we say in Ruby "objects." Each method however handles its elements in a different fashion.

### The Ruby Array

Arrays are structured using the bracket symbol [ ]. Inside the bracket you can have a different mix of of different types of elements. For example:

{% highlight ruby %}
array = [1, 2, 3]
or
array = [1, 2, 3, "hello", x, y, z]
{% endhighlight %}

As you can see an array can hold several different types of elements within the same array. There are several methods built into Ruby that allow you access to the elements of your array. You can count your elements, count the entire length of the array, see which element is at which point in the array and so on. The array holds each element in a certain position starting at 0 and counting up until it reaches the last element. For example the array [1,2,3,4] would count the position of its elements at 0,1,2,3. This position is called the elements "index." Notice how the index starts at 0 instead of 1 so the index list will always be 1 less than the total number of elements. It is important to remember that since an array holds these elements in a certain position, the elements are kept in order and can only be accessed in this particular order.

### The Ruby Hash

A hash stores elements in a slightly different way using what is called key-value pairs inside curly brackets { }. In the image above you can see the variable "inst_section" holds a group of key-value pairs. The left side objects following the colon are the keys and the right side are the values assigned to each key. You can tell the value by looking for the => symbol. The value will alway follow this symbol. The keys do not have to be prefaced with a colon. They could just as easily be strings. For example:

{% highlight ruby %}
grades = { 
	"Bob" => 82, 
	"Jim" => 94, 
	"Shelly" => 89 }
{% endhighlight %}

Now much like the arrays you can access each element either by using the key or the value. It is important to remember however that hashes do not store the elements in any particular order so if you want an ordered list you must use an array. But if you don't care about order and you just want to store a key pair value use a hash.

This is just the tip of the iceberg of what arrays and hashes can be used for. In fact Ruby uses arrays and hashes for just about everything! So if you just need a simple list of ordered objects feel free to use and array but if you need to store your elements in an unordered list, use the a hash.

