---
layout: page_hide-title
title: Bio
permalink: /about/
---

{{ site.description }}

You can also find me on {% for item in site.data.links.social %}{% if forloop.last %}and {% endif %}[{{ item.title }}]({{ item.url }}){% unless forloop.last %}, {% endunless %}{% endfor %}.

---

## Projects & Collaborations
{% assign sorted = site.projects | sort: 'order' %}
{% for project in sorted %}
* [{{ project.title }}]({{ project.url }}){% endfor %}
* Major redesign of the journal *Sagar* and the establishment of a coherent visual language spanning the printed publication, promotional materials, and [website](http://sagarjournal.org).
* An [XML-based, multimedia re-release](https://quod.lib.umich.edu/cgi/t/text/text-idx?c=acls;cc=acls;view=toc;idno=heb90059.0001.001;rgn=full%20text) of Hindi scholar Kathryn Hansen’s 1992 book, *Grounds for Play: the Nauṭaṅkī Theatre of North India*, for the [Humanities E-Book](http://www.humanitiesebook.org/) collection of the American Council of Learned Societies. The revised e-book was released in February 2015.

---

## Background

### Professional
I have been working as a freelance designer and developer for over five years. I spend a lot of my time running [Sloop Creative](http://www.sloopcreative.com/) with my partner, Moeko Crider. We’re a community-minded creative studio located in the beautiful Skagit Valley, Washington. Prior to this, I served as the Managing Editor of [*Art in Print*](http://artinprint.org), the premier American publication on the the artist’s print. I also worked as Assistant Media Coordinator at UT-Austin’s Hindi–Urdu Flagship from 2012–13.

### Academic
I completed my M.A. in Asian Cultures and Languages from The University of Texas at Austin in 2013. There, I worked on the topics of masculinity, asceticism, and medicine in South Asian history; I also studied Sanskrit, Pali, and Hindi. My Master’s Thesis, “Reckoning Up the Body: Logics of Enumeration and Arrangement in Buddhist and Ayurvedic Inventories of Anatomy,” was a deep comparative reading of anatomical inventories in *Visuddhimagga*, *Caraka-saṃhita*, and *Suśruta-saṃhita*. I argued, against the gloss that these accounts are either “religious” or “medical” in nature, that they carve up the materiality of the human body in a constellation of complex and often overlapping ideologies and epistemologies. The thesis was a finalist for the UT-Austin Graduate School’s Outstanding Master’s Thesis Award.

I earned my B.A. (Religious Studies) from Whitman College in 2008.

---

## Skills

### Markup & Programming Languages
HTML, CSS, Sass, Markdown, HAML, XML, XSLT; JavaScript/jQuery, PHP, Liquid

### Frameworks/CMS
Jekyll, WordPress

### Other Development Skills
A11y, version control with Git & Github, BEM methodology, Continuous Integration

### Design
*Web:* wireframing, high-fidelity mockups, living style guides; *Print:* long documents, marketing materials, InDesign templates, proofing

### Applications
Sketch, Adobe Creative Cloud (Ai, Id, Ps, Lightroom), Vagrant, Oxygen XML, Trello, Slack

### Natural Languages
English: native; Hindi, Sanskrit, Pali: intermediate

### Other
Copyediting

### Always Learning…
Currently hitting the books on: prototyping, React, LaTeX

---

## Contact
[Drop me a line](mailto:{{ site.author.email }}) if you’d like to collaborate, or simply to say hello. I’m also on {% for item in site.data.links.social %}{% if forloop.last %}and {% endif %}[{{ item.title }}]({{ item.url }}){% unless forloop.last %}, {% endunless %}{% endfor %}.

---

## Colophon
The design of this site is an experiment in achieving rhythm, harmony, hierarchy, and readability through simple variations in typography and layout. It’s inspired by [Dean Allen’s appeal](https://web.archive.org/web/20010409223650/http:/www.textism.com:80/resources/index.html?id=7) to treat words first and foremost as things that we *read*, not just look at. I'm using [Adobe Caslon](https://typekit.com/fonts/adobe-caslon), and occasionally [Source Code Pro](https://typekit.com/fonts/source-code-pro) for code snippets.

The site runs on [Jekyll](https://jekyllrb.com/) and is coded in Markdown, Liquid, HTML, and Sass. You can find the repository on [Github]({{ site.repository }}).

*[M.A.]:
*[B.A.]:
*[CMS]:
*[HTML]:
*[HAML]:
*[CSS]:
*[JS]:
*[YAML]:
*[PHP]:
*[XML]:
*[XSLT]:
*[BEM]:
*[CC]:
*[JAF]:
*[UT]:
*[FRIDA]:
