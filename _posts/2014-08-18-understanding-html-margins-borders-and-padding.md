---
layout: post
title: "Understanding HTML Margin, Border, and Padding"
description: "DBC week 2 tech blog"
modified: 2014-08-18 18:27:15 -0700
tags: [dev bootcamp, web development, DBC, blog, jekyll, shane biggs]
image:
  feature: abstract-5.jpg
  credit: dargadgetz
  creditlink: http://www.dargadgetz.com/ios-7-abstract-wallpaper-pack-for-iphone-5-and-ipod-touch-retina/ 
comments: true
share: true
---
### Make Your HTML Elements Dance

Understanding how to move the elements into the correct position is by far one of the most important concepts of building a web page. Without this understanding it is possible to build a very simple web site but impossible to build a great website.

Let's first take a look at the CSS "Box Model." Each HTML element is essentially a container or "Box". Looking at the representation of the HTML box below you can see that it consists of three parts: margin, border, and padding. The size of each of the three different layers can be changed by specifying the "em, %, or px" for each property. Each property in turn has multiple ways to specify its sizes. Read here for more information on the properties and values:    <a href="http://www.w3schools.com/cssref/pr_margin.asp" target="_blank" title="Margin">Margin</a>  <a href="http://www.w3schools.com/css/css_border.asp" target="_blank" title="border">Border</a>  <a href="http://www.w3schools.com/css/css_padding.asp" target="_blank" title="Padding">Padding</a>
 
![Box](/images/week_2/margin.png)
<figcaption><a href="http://www.washington.edu/accesscomputing/webd2/student/unit3/module4/lesson1.html" target="_blank" title="Source">Source</a></figcaption>

Here is a very basic example of how to create a simple box containing content using the "Box Model" concepts.

{% highlight css %}
#box {
	background-color: red;
	padding: 10px;
	border: 1px solid black;
	margin: 10px;
}

#box p{
	text-align: center;
	background-color: white;
	padding: 1em;
	borer-width: 10px;
	border-style: solid;
	border-color: darkgrey;
	margin: 10px !important;
}
{% endhighlight %}

So as you can see understanding the "box" concepts are instrumental in understanding how to move your elements around the page using CSS. This is fundamental part of HTML/CSS that needs to be mastered in order to create awesome looking, functional website.







