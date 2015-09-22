---
layout: page
permalink: /DBC_basics/
title: "Dev Bootcamp Basics"
description: "Notes for the basics at DBC"
modified: 2014-08-18 00:47
tags: [dev bootcamp, web development, DBC, blog, jekyll, shane biggs]
image:
  feature: abstract-10.jpg
  credit: dargadgetz
  creditlink: http://www.dargadgetz.com/ios-7-abstract-wallpaper-pack-for-iphone-5-and-ipod-touch-retina/ 
comments: true
share: true
---

# The basic need-to-know of hashes for Dev Bootcamp

## Create a new hash
`Hash.new` - creates new hash

{% highlight ruby %}
grades = Hash.new

# or

grades = {}
{% endhighlight %}

### Default value
- can set a default value if the key doesn't not exist
- 2 ways

{% highlight ruby %}
grades = Hash.new(0)  # will set a default value of 0
# or
grades.default = 0	  # will set a default value of 0
{% endhighlight %}


### Adding key values to the new hash

`grades[key] = value`

- add a key with a value to a hash using `variable_name[key] = value`

{% highlight ruby %}
grades = Hash.new
grades[:Shane] = 100
{% endhighlight %}

## Hash Syntax (differences)

- standard

{% highlight ruby %}
grades = {
	"Shane Biggs" => 100,
	"Ayden Biggs" => 97
}
{% endhighlight %}

- keys as symbols (`:` goes in front of key)

{% highlight ruby %}
grades = {
	:Shane Biggs => 100,
	:Ayden Biggs => 97
}
{% endhighlight %}

- alternate (keys are not symbols)

{% highlight ruby %}
grades = {
	Shane_Biggs: 100,
	Ayden_Biggs: 97
}
{% endhighlight %}

## Accessing keys/values

- use the key to find the value

{% highlight ruby %}
grades[:Shane] # => 100
grades[:Ayden] # => 97
{% endhighlight %}

- use the value to find key

{% highlight ruby %}
grades.key(100) # => :Shane
{% endhighlight %}

- access all keys or all values 

{% highlight ruby %}
grades.keys # => [:Shane, :Ayden] # returns an array of keys
grades.values # => [100, 97] # returns an array of values
{% endhighlight %}

## Iterate over a hash

### .each method

- `.each` 

{% highlight ruby %}
grades.each { |key, value| puts "#{key}'s grade #{value}" }

# or

grades.each do |key, value| 
	puts "#{key}'s grade is #{value}"
end

# => Ayden's grade is 97
# => Shane's grade is 100
{% endhighlight %}

### .each_key method

- `.each_key` - iterates and puts the keys

{% highlight ruby %}
grades.each_key { |key| puts key}
# => Ayden
# => Shane
{% endhighlight %}

### .each_value method

- `.each_value` - iterates and puts the values

{% highlight ruby %}
grades.each_value { |value| puts value }
# => 97
# => 100
{% endhighlight %}

#### How to iterate and change the price of an item by 10% (rubymonk.com)

{% highlight ruby %}
restaurant_menu = { "Ramen" => 3, "Dal Makhani" => 4, "Coffee" => 2 }
restaurant_menu.each do |item, price|
  restaurant_menu[item] = price + (price * 0.1)
  # access the [item] key to change price
end

# => {"Ramen"=>3.3, "Dal Makhani"=>4.4, "Coffee"=>2.2}
{% endhighlight %}

### .select method

- `.select` - iterates and returns a new hash of entries for which the block returns true

{% highlight ruby %}
grades.select { |key, value| value > 90 }
# => {:Ayden=>97, :Shane=>100}
# these are true because they are > 90
{% endhighlight %}

### .reject method

- `.reject` - iterates and returns a new hash of entries for which the block returns false

{% highlight ruby %}
grades.reject { |key, value| value < 90 }
# => {:Ayden=>97, :Shane=>100}
# these are false because they are not < 90
{% endhighlight %}


