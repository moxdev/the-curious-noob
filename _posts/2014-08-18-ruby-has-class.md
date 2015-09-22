---
layout: post
title: "Ruby Has Class!"
description: "DBC week 5 tech blog"
modified: 2014-08-18 22:05:40 -0700
tags: [dev bootcamp, web development, DBC, blog, jekyll, shane biggs]
image:
  feature: abstract-5.jpg
  credit: dargadgetz
  creditlink: http://www.dargadgetz.com/ios-7-abstract-wallpaper-pack-for-iphone-5-and-ipod-touch-retina/ 
comments: true
share: true
---

### Classy Ruby

Today we are going to take a look at creating a Ruby class. Ruby uses class statements which contain methods that work on the object. As your programs gets larger and more complicated Ruby needs classes so that you can have several of the same methods being performed on different objects. When you call the method later Ruby will know exactly which methods you are trying to perform because they have been defined by their class.<

<div class="box" class="links"><img src="/images/week_5/tech_1.png" alt="CSS Box Model"><p></div>

In the image above you can see the beginnings of our very simple Person class we will use to store information about people. This class will need three things for input to be able to create the new person: first_name, last_name, and age. We need to use the initialize method here so we can call these variables later in our program. These are called instance variables and are denoted by using the @ symbol.
							

<div class="box" class="links"><img src="/images/week_5/tech_2.png" alt="CSS Box Model"><p></div>

We can now use this class statement to create as many new Person's as we like. Let's go through "p1" and take at look at its format. First you give the new object a name (p1 or whatever you like it's up to you) and then call the Person.new class and provide the required information which in this case is their first name, last name , and age.
						
<div class="box" class="links"><img src="/images/week_5/tech_3.png" alt="CSS Box Model"><p></div>

With the new persons created you can now use the Person class to do many cool things with the information you have stored. We've gone back and added a new method called "person_info" to the class. We can know take the information you have entered for each new person and have Ruby print out a nice little sentence using that information. In this case Ruby should tell us the person's first and last name and their age. 

							
<div class="box" class="links"><img src="/images/week_5/tech_4.png" alt="CSS Box Model"><p></div>

As you can see from the above image, Ruby prints out a nice little sentence about each person. Man Bill Murray is getting up there in years but he's still awesome! This was just a very simple and basic example of what you can do with a Ruby class. You can add as many methods as you like to perform all sorts of creative functions on the objects. Go ahead and give it try!