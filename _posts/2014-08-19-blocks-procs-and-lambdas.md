---
layout: post
title: "Blocks, Procs, and Lambdas"
description: "DBC week 6 tech blog"
modified: 2014-08-19 11:05:22 -0700
tags: [dev bootcamp, web development, DBC, blog, jekyll, shane biggs, ruby, blocs, procs, lambdas]
image:
  feature: abstract-5.jpg
  credit: dargadgetz
  creditlink: http://www.dargadgetz.com/ios-7-abstract-wallpaper-pack-for-iphone-5-and-ipod-touch-retina/ 
comments: true
share: true
---

### Ruby Blocs, Procs, and Lambdas Oh My!

Today we are going to take a look at one of Ruby's most powerful features. Ruby uses what are called Blocks, Procs, and Lambdas to pass code to a method and then execute that code at a later point and time. Like most things in Ruby, these three functions perform very similar actions and can often be used interchangeably.

Lets begin with discussing the Ruby Block. In the image above we have constructed a very simple .map! solution for iterating through an array and multiplying each number by 5. There are two ways to perform this action. First it can be written using the (do..end) syntax that you see in the first example. This syntax would often be used for a block containing multiple lines of code. In the second example you can see the (do..end) block has been replaced with just the curly brackets {}. This version would most often be used for a simple block of code that fits nicely on one line. The code in between the (do..end)and {} is what's referred to as the block.

<img src="/images/week_6/block.png" alt="block">

Enter the Proc! So we can see here that using the Ruby Proc object of Proc.new, we can perform the same function as our block code. The Proc however is a little different from a block in that you are able to save the code and call it over and over again. You see the block code is simply syntax and as syntax it is disposable. In order to use the block again you must retype it whenever you need it. The Proc remedies this by allowing you to save the code inside of a variable which can then be called later. You must remember to use the & symbol in front of your variable when passing your Proc as an argument like in the example above (&multiply).

<img src="/images/week_6/proc.png" alt="proc">

So what's the deal with Lambda? It may look like it is performing the exact same function as our previous Proc method but behind the scenes it is behaving very differently. First of all lambda will check to see if the correct number of arguments have been passed to it. If the wrong number of arguments are passed, lambda will issue an ArgumentError. Proc does not behave in the same manner. A Proc will ignore any unexpected arguments and assign nil as the value of any missing arguments. Another key difference is when a lambda returns, it will pass control back to the calling method. When a Proc returns, it returns immediately without going back to the calling method. This can cause different outcomes depending on how your code is written.

<img src="/images/week_6/lambda.png" alt="lambda">

So as you can see Blocks, Procs, and Lambdas are all very useful for performing certain functions in Ruby code. Go ahead and try it out on your own! I know I will be using them a lot more in my own coding in the future. 
