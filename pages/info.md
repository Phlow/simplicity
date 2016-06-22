---
subheadline: 'Info'
title: 'Why I designed *Simplicity*'
permalink: /info/
---
The idea behind *Simplicity* is to build a theme which is elegant, ver&shy;satile but still fast, without any clutter and the pur&shy;pose to make blogging and publishing as easy as possible.

<!--more-->

While sketching *Simplicity* I asked myself: »How much can I strip down from a post. How much [front matter][3] is truly needed?« And the answer is really simple: For pages or posts you need **no front matter at all**. You create a file, name it and Jekyll uses the file name automatically if you don't add `title` to front matter.


## *Simplicity* chooses the layout for you

And because you can define the default-layout in *_config.yml*. You don't need to add *title:* to front matter either. But what makes this theme truly elegant is, that if you need some tasty video on top of your posting or a nice image, you do it like this…

{% highlight html %}
---
youtube: https://www.youtube.com/watch?v=8pQAWOCofXo
---
{% endhighlight %}

or that…

{% highlight html %}
image: image-on-top-of-post.jpg
{% endhighlight %}

The layout figures out what to do :)

And if you are a blogger who enjoys spicing up his posts, there are plenty of possibilities. Maybe like this?!?

{% highlight html %}
subheadline:    I love'em
title:          Your Title
header_image:   amazing_header_image.jpg
comments:       true
show_meta:      true
embed:          <iframe>…</iframe>
{% endhighlight %}

For more options, [download *Simplicity*][4] and check out its well-documented templates, includes and layout-options.

All the best from [Cologne][1], [Moritz »mo.« Sauer][2]






[1]: https://www.google.de/maps/place/K%C3%B6lner+Dom/@38.5398373,2.1154583,4z/data=!3m1!5s0x47bf25baabc20433:0x312b7d4db7d02b48!4m2!3m1!1s0x47bf25a5369c3d2f:0x29ec913896e3a9c6
[2]: http://moritz.sauer.io
[3]: https://jekyllrb.com/docs/frontmatter/
[4]: https://github.com/Phlow/simplicity