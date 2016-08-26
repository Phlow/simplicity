---
title: "Highlighting Code"
meta_description: "*Simplicity* is GitHub Pages-ready, that means, it uses Rouge for syntax highlighting."
---
*Simplicity* is GitHub Pages-ready, that means, it uses Rouge for syntax highlighting. To adjust the code highlighting to your taste, Just open *_sass/_07_syntax_highlighting.scss* and tune the colors to your taste.
<!--more-->

To learn more, read [»Mixing Color for the Web with Sass«](http://alistapart.com/article/mixing-color-for-the-web-with-sass) or check out the [Sass-manual with all the functions](http://sass-lang.com/documentation/Sass/Script/Functions.html).

## Rouge

To render a code block with syntax highlighting, surround your code as follows:


{% highlight ruby %}
{% raw %}{% highlight ruby %}{% endraw %}
def foo
  puts 'foo'
end
{% raw %}{% endhighlight %}{% endraw %}
{% endhighlight %}

If you need lines, add `linenos`…

{% highlight ruby linenos %}
{% raw %}{% highlight ruby linenos %}{% endraw %}
def foo
  puts 'foo'
end
{% raw %}{% endhighlight %}{% endraw %}
{% endhighlight %}


