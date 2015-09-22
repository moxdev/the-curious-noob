---
layout: post
title: "A Dangerous Game of SQL Injection"
description: "DBC week 7 tech blog"
modified: 2014-08-19 11:32:29 -0700
image:
  feature: abstract-5.jpg
  credit: dargadgetz
  creditlink: http://www.dargadgetz.com/ios-7-abstract-wallpaper-pack-for-iphone-5-and-ipod-touch-retina/ 
comments: true
share: true
---

### Injection Protection

The Internet provides the world with a single point of access to seemingly unlimited resources of knowledge and entertainment.To most of us it is simply a matter of browsing to our preferred website, logging in with our username and password, and then going about our business. Most of us take for granted the code behind the scenes that makes all of this work.  
						
When you make a new user account for a website your information is stored in a database so it can be accessed later. This information is mostly likely stored in what is called an SQL database. These SQL databases can be used by hackers for nefarious purposes. SQL commands are simple text only inputs but in the wrongs hands they can be powerful tools used to steal user information, delete database information, or even cripple websites. Hackers can use "SQL Injection" to "inject" malicious SQL commands via webpage input. These malicious commands can compromise the security of a web application. A smart hacker can literally insert a new character or two and gain access to private information such as user logins. SQL injections can also be used to redirect users to malicious websites. If your web application becomes infected users may lose confidence in your ability to protect their data and stop using your services.
							
Check out this website <a href="http://sqlzoo.net/hack/" target="_blank">SQLZoo</a> for hands on demonstration of how hackers can use SQL injection to compromise your web application.