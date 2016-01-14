The *Simplicity* styleguide lists all available elemnts to style your content.

<!--more-->


## Colors

*Simplicity* allows you to change the colors to your taste quickly. Just open *_sass/_01_colors.scss* and tune your colors.

Four possible brand colors and four colors to style alerts.

<div class="ci-1-bg text-center" style="float: left; line-height: 7em;width: 7em;height:7em">CI-1</div>
<div class="ci-2-bg text-center" style="float: left; line-height: 7em;width: 7em;height:7em">CI-2</div>
<div class="ci-3-bg text-center" style="float: left; line-height: 7em;width: 7em;height:7em">CI-3</div>
<div class="ci-4-bg text-center" style="float: left; line-height: 7em;width: 7em;height:7em">CI-4</div>

<div class="alert-color-bg text-center" style="float: left; line-height: 7em;width: 7em;height:7em">alert</div>
<div class="success-color-bg text-center" style="float: left; line-height: 7em;width: 7em;height:7em">success</div>
<div class="warning-color-bg text-center" style="float: left; line-height: 7em;width: 7em;height:7em">warning</div>
<div class="info-color-bg text-center" style="float: left; line-height: 7em;width: 7em;height:7em">info</div>
<div style="clear:both;"></div>



## Alerts

With alerts you insert warnings, info-boxes or hints. Use the *alert*-include in *_includes/*.

{% include alert warning='This is a warning with a <a href="http://phlow.github.io/feeling-responsive/">Link</a> and <em>italic</em> and <strong>bold</strong> text.' %}
{% include alert info='An info box with a <a href="http://phlow.github.io/feeling-responsive/">Link</a> and <em>italic</em> and <strong>bold</strong> text.' %}
{% include alert success='A success box with a <a href="http://phlow.github.io/feeling-responsive/">Link</a> and <em>italic</em> and <strong>bold</strong> text.' %}
{% include alert alert='An alert box with a <a href="http://phlow.github.io/feeling-responsive/">Link</a> and <em>italic</em> and <strong>bold</strong> text.' %}
{% include alert terminal='jekyll -serve' %}
{% include alert text='Just a note with a <a href="http://phlow.github.io/feeling-responsive/">Link</a> and <em>italic</em> and <strong>bold</strong> text.' %}



## Buttons

Use them with `<a>` or `<button>`.

<a class="button" href="#">Button</a>
<a class="button alert" href="#">Alert Button</a>
<a class="button info" href="#">Info Button</a>
<a class="button success" href="#">Success Button</a>
<a class="button warning" href="#">Warning Button</a>
<a class="button grey" href="#">Grey Button</a>

