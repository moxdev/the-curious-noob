# Things to change
### Install bundle
- `bundle install` after installing jekyll

### Config
- edit image 300x300 - edit the path in `head.html` to link to Gravitar
- edit URL http://localhost:4000 for local edits
- add background: filename.png to _config.yml (set a background image for the entire site)

### Home Page
- edit feature image on index.html
- edit specific background image for home page on index.html

# New post or page
- `rake new_post` or `rake new_page`
- fill out info
	+ title
	+ tags
- image
	+ feature index.html
		* change credit
	+ crop 1024 x 256
	+ [Jekyll Picture Tag](https://github.com/scottjehl/picturefill)[^2] plugin
	+ keep in /images
	+ example:
	
```
{% highlight yaml %}
image:
  feature: feature-image-filename.jpg
  thumb: thumbnail-image.jpg #keep it square 200x200 px is good
{% endhighlight %}
```
## New page
- edit the config "links"

#### Images

```
<figcaption>Twitter Homepage</figcaption> 
![Twitter Homepage](/images/twitter.png)
```

#### Link

```
<a href="https://www.tumblr.com" target="_blank" title="Tumblr.com"><strong>Tumblr</strong></a>
```

#### Videos
- [FitVids](http://fitvidsjs.com/)
- embeding YouTube vids causes errors in kramdown (possibly others). To fix add space between iframe tags and remove allow fullscreen:


```
{% highlight html %}
<iframe width="560" height="315" src="http://www.youtube.com/embed/PWf4WUoMXwg" frameborder="0"> </iframe>
{% endhighlight %}
```

#### Twitter Cards

Twitter cards make it possible to attach images and post summaries to Tweets that link to your content. Summary Card meta tags have been added to `head.html` to support this, you just need to [validate and apply your domain](https://dev.twitter.com/docs/cards) to turn it on.

# Highlight code blocks
#### Including code blocks in MD
- highlight with line numbers (include proper syntax "html", "ruby", etc.)

```
{% highlight html linenos %}
{% raw %}
code block here
{% endraw %}
{% endhighlight %}
```
- highlight specific code

```
{% highlight ruby %}
code goes here
{% endhighlight %}
```
- standard code block (no highlights)

```
{% raw %}
{% endraw %}
```

# Edit CSS
- assets/css/main.css
- body starts line 278
- 





