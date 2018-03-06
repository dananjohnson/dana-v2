---
title: FRIDA 2016 Annual Report
image: frida-2016_2.png
year: 2017
summary: 'At Sloop Creative, I worked with FRIDA | The Young Feminist Fund on a digital annual report. Built as a static microsite, the report features a bold design and a number of creative frontend solutions.'
external_link:
  url: http://annualreport2016.youngfeministfund.org/
  title: View Website
order: 3
---

In the fall of 2017, Sloop Creative worked with regular client [FRIDA \| The Young Feminist Fund](https://youngfeministfund.org/) on their, and our, first *digital* annual report. Designed as a static microsite in six chapters, the report features loads of images, animated charts, and, as with all the work we’ve done for FRIDA, bold patterns and colors.

{% include responsive-img.html.liquid src="frida-2016_2.png" alt='Screenshot of “Powerful Patterns: FRIDA 2016 Annual Report”' %}

The site was coded in HTML, Markdown, Liquid, Sass, YAML, and jQuery, and compiled with Jekyll. It was a true test of my skills as a frontend developer. Often, Moeko would share a design idea, asking, “Can you code this?,” and I would reply, “I don’t know. Let’s find out!” I utilized flexbox extensively to build responsive, interactive modules like expanding accordions and sliders without any JavaScript. I learned a number of new properties and techniques in CSS, including layering and blending background images with `background-blend-mode`. I also developed a technique with Sass to dynamically generate a three-color visual theme, which could be modified for each chapter with just a few variables. ~~Stay tuned for a blog post about that.~~ I wrote about this in detail in [this blog post]({{ site.baseurl }}{% post_url 2018-03-06-managing-complex-color-schemes-with-sass %}).

{% include responsive-img.html.liquid src="frida-2016_3.png" alt='Screenshot of “Powerful Patterns: FRIDA 2016 Annual Report”' %}
{% include responsive-img.html.liquid src="frida-2016_5.png" alt='Screenshot of “Powerful Patterns: FRIDA 2016 Annual Report”' %}

One other real source of learning on this project was using Jekyll to generate visualizations from YAML data. The report contained a lot of metrics about FRIDA’s finances and programming. I wanted to keep this data separate for sustainability and accessibility, and Liquid proved perfect for templating Javascript to generate bar and pie charts. So, data could be simply stored like this —

{% highlight yaml %}
- id: chart_1
  type: bar
  high: 12
  data:
  - label: Latin America & Caribbean
    number: 10
  - label: Asia & the Pacific
    number: 11
  - label: Central Europe, Caucasus, Central Asia
    number: 8
  - label: Middle East & North Africa
    number: 8
  - label: Sub-Saharan Africa
    number: 11
{% endhighlight %}

— and outputted as an animated, themed chart.

{% include responsive-img.html.liquid src="frida-2016_6.png" alt='Screenshot of “Powerful Patterns: FRIDA 2016 Annual Report”' %}

We used [Chartist.js](https://gionkunz.github.io/chartist-js/), but this technique could work equally well with [D3](https://d3js.org/) or [Chart.js](http://www.chartjs.org/).

Overall, this project put Jekyll and Sass through the ringer, and I was more than impressed with their performance.

*[HTML]:
*[YAML]:
*[JS]:
*[CSS]:
*[FRIDA]:
*[D3]:
