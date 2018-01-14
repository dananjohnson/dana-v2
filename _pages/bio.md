---
layout: page_hide-title
title: Bio
permalink: /about/
---

{:.lead}
{{ site.description }}

{:.lead}
You can also find me on {% for item in site.data.links.social %}{% if forloop.last %}and {% endif %}[{{ item.title }}]({{ item.url }} "Dana Johnson on {{ item.title }}"){% unless forloop.last %}, {% endunless %}{% endfor %}.

---

## Projects & Collaborations
{% assign sorted = site.projects | sort: 'order' %}
{% for project in sorted %}
* [{{ project.title }}]({{ project.url }} "{{ project.title }}"){% endfor %}
* Major redesign of the journal *Sagar* and the establishment of a coherent visual language spanning the printed publication, promotional materials, and [website](http://sagarjournal.org "Sagar Journal").
* An [XML-based, multimedia re-release](https://quod.lib.umich.edu/cgi/t/text/text-idx?c=acls;cc=acls;view=toc;idno=heb90059.0001.001;rgn=full%20text "Grounds for Play: the Nauṭaṅkī Theatre of North India") of Hindi scholar Kathryn Hansen’s 1992 book, *Grounds for Play: the Nauṭaṅkī Theatre of North India*, for the [Humanities E-Book](http://www.humanitiesebook.org/ "Humanities E-Book") collection of the American Council of Learned Societies. The revised e-book was released in February 2015.
* Material design for Punctum Records, plus a number of concert posters while living in Austin.

---

## Background

### Professional
I have been working as a freelance designer and developer for over five years. I spend a lot of my time running [Sloop Creative](http://www.sloopcreative.com/ "Sloop Creative") with my partner, Moeko Crider. We’re a community-minded creative studio located in the beautiful Skagit Valley, Washington. Prior to this, I served as the Managing Editor of [*Art in Print*](http://artinprint.org "Art in Print"), the premier American publication on the the artist’s print. I also worked as Assistant Media Coordinator at UT-Austin’s Hindi–Urdu Flagship from 2012–13.

### Academic
I completed my M.A. in Asian Cultures and Languages from The University of Texas at Austin in 2013. There, I worked on the topics of masculinity, asceticism, and medicine in South Asian history; I also studied Sanskrit, Pali, and Hindi. My Master’s Thesis, “Reckoning Up the Body: Logics of Enumeration and Arrangement in Buddhist and Ayurvedic Inventories of Anatomy,” was a deep comparative reading of anatomical inventories in *Visuddhimagga*, *Caraka-samhita*, and *Suśruta-samhita*. I argued, against the gloss that these accounts are either “religious” or “medical” in nature, that they carve up the materiality of the human body in a constellation of complex and often overlapping ideologies and epistemologies. The thesis was a finalist for the UT-Austin Graduate School’s Outstanding Master’s Thesis Award.

I earned my B.A. (Religious Studies) from Whitman College in 2008.

---

## Skills

* Responsive, accessible front-end development with HTML5, CSS3, SASS, JS
* plain text encoding in Markdown & YAML
* templating in Liquid & PHP
* versioning and collaboration with Git
* XML/XSLT
* Adobe CC (InDesign, Photoshop, Illustrator)
* Sketch
* Always learning. Currently hitting the books on:
  * JavaScript frameworks
  * LaTeX
  * Ruby on Rails

---

## Colophon
This site runs on [Jekyll](https://jekyllrb.com/ "Jekyll") and is coded in Markdown, Liquid, HTML, and CSS. The text is set in Tim Ahren’s [JAF Lapture Display](https://justanotherfoundry.com/lapture "JAF Lapture") and Paul D. Hunt’s [Source Sans](https://typekit.com/fonts/source-sans "Source Sans on Typekit"). You can view the site repository on [Github]({{ site.repository }}).
