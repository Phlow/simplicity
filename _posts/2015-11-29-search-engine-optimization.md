*Simplicity* offers you lots of options to optimize your content for search engines like Google.

<!--more-->

- `meta_title:`
- `meta_description:`
- `permalink:`
- `sitemap.xml`
- *Simplicity's* HTML-Code uses schema.org-meta data



## Optimize Your Articles

*Simplicity* uses `title: Your Post Title` by default for generating the `<title>`. You can overwrite the title with:

{% highlight html %}
meta_title:
{% endhighlight %}

To taylor fit a description for Google & Co. use…

{% highlight html %}
meta_description: 
{% endhighlight %}

…otherwise *Simplicity* will use the excerpt or the first paragraph of your content.

The last important SEO-setting is the URL. By default *Simplicity* uses `permalink: /:categories/:title/` but of course you can change the settings in *_config.yml* or overwrite the URL in front matter with…

{% highlight html %}
permalink:
{% endhighlight %}



## Optimize Your Site

And while we discuss search engine optimization: Submit your site to Google Webmaster Tools/Search Console and Bing and enter the your Google Site Verification ID in *_config.yml*.

{% highlight html %}
google_site_verification:
{% endhighlight %}

{% highlight html %}

{% endhighlight %}

And last but not least, submit your *sitemap.xml* to Google Search Console and Bing Webmaster Tools.