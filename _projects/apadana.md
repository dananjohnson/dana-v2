---
title: Legends of the Buddhist Saints
image: apadana_1.png
year: 2017–18
summary: I led the creation of an interactive, open-access digital publication for the first-ever translation of the Apadāna into English.
external_link:
  url: http://beta.apadanatranslation.org/
  title: View Website
order: 1
---

*Apadāna* is a collection of roughly 600 early Buddhist poems, composed in Pāli around the second century, B.C.E. It has always been the only part of the Pāli Canon that had never been fully translated into English. Beginning in Spring 2017, I worked with Dr. Jonathan S. Walters, with funding from Whitman College, to create an open access digital publication of his translation of the text, entitled *Legends of the Buddhist Saints*.

{% include responsive-img.html.liquid src="apadana_4.png" alt="Screenshot of Legends of the Buddhist Saints website" %}

The goals of the project were as follows: to convert the 2,000-page translation out of a word processor file and into something more durable and useable; to devise a best course of action for publishing the text online; and, to build an interface that allowed readers of differing levels to engage with the text at different levels.

As of November 2017, the project is in beta testing.

### Interface design
{% include responsive-img.html.liquid src="apadana_1.png" alt="Screenshot of Legends of the Buddhist Saints website" %}

A priority of Dr. Walters’, in conjunction with releasing the publication open-access, was to limit barriers of entry based on prior knowledge of Buddhism or Pāli. Scholars, teachers, students, purveyors of poetry, practicing Buddhists, and casual readers alike should be able to engage with the text at their desired level. To this end, Dr. Walters envisioned offering two versions of the text, one with just the text of the translation, and the other with all the essential aspects that a scholarly translation includes: diacritics, footnotes, and verse numbers referencing the source text. In fact, for a long time he was maintaining two .doc files to make this possible.

When I came onboard, I felt strongly that the dual-manuscript solution was not sustainable, and could lead to problems maintaining a stable repository in the future. Not only that, but it wasn’t necessary. I wrote a JavaScript function that uses `grep` to identify the “scholarly” components of the text and apply an tag them with an HTML tag that can then be toggled on and off in the user interface. (I’ll write more about this in a blog post.) This has tremendous benefit to both reader and author. On Dr. Walters’ end, he need only maintain one copy of the text. And for the user, she can choose the level of reading she is comfortable with, or try out features she may not be familiar with yet.

{% include responsive-img.html.liquid src="apadana_2.png" alt="Screenshot of Legends of the Buddhist Saints website" %}

In addition to the toggles for text features, the online interface also includes on-the-fly search of the entire translation, downloads in PDF and ePub, and quick links to cite a poem or share it on social media.

{% include responsive-img.html.liquid src="apadana_3.png" alt="Screenshot of Legends of the Buddhist Saints website" %}

The text is set in [Rosetta Type Foundry](https://www.rosettatype.com/ "Rosetta Type Foundry")’s [Skolar](https://www.rosettatype.com/Skolar "Skolar") and [Skolar Sans](https://www.rosettatype.com/SkolarSans "Skolar Sans"), which, besides being both modern and elegant yet pleasingly quirky typefaces, also feature Indic diacritics.

### Publishing workflow

{% asset 'apadana_6.svg' alt='Screenshot of Legends of the Buddhist Saints website.' %}

In building this publishing ecosystem, I was guided by the [principles](https://go-dh.github.io/mincomp/thoughts/2016/10/03/tldr/ "Minimal Definitions (tl;dr version)") of [Minimal Computing](https://go-dh.github.io/mincomp/ "Minimal Computing"), particularly those of Minimal Maintenance, Minimal Obsolescence, Maximum Access, and Maximum Accessibility. I chose [Markdown](https://daringfireball.net/projects/markdown/syntax "Markdown"), a minimal plain-text syntax, as the file format for encoding the translation. Unlike documents composed in word processors like Microsoft Word, Markdown does not confuse content with design features like font choice and margin size. Nor does it muddle the text with layers of unseen file data. It also does not require proprietary software to be read or edited. The result is a highly flexible and sustainable file format.

{% asset 'apadana_5.png' alt='Screenshot of Legends of the Buddhist Saints website.' %}

The translation is stored in a [public repository on Github](https://github.com/apadana-translation/apadana-site). This offers many benefits: changes to the translation are documented and archived, and the raw text of the publication is made freely available to others under the [CC-BY-NC-SA license](https://creativecommons.org/licenses/by-nc-sa/3.0/us/).

We’re using [Pandoc](http://pandoc.org/index.html) and [Jekyll](https://jekyllrb.com/) to convert the text into HTML, PDF, and ePub formats. Through [Travis CI](https://travis-ci.org/), this happens automatically any time a commit is made to the Github repository.

The result is a stable, portable, accessible publication of an important work of scholarship. Dr. Walters can manage the source text in a format that is minimal in both size and sophistication. Interested readers can engage with the project in a format of their choosing, free of charge.

### Future plans
Plans for further development of the project center around enriching the text with multimedia and deepening resources for understanding the *Apadāna*. The first enhancement will be to make available audio recordings to show the cadence and rhythm of the metered poetry. In the spirit of the text — about a community of beings moving towards enlightenment together — the plan is for 600+ members of the Whitman College community to each record one poem. We also plan to compile a visual glossary of flora and fauna and other textual references that may be unfamiliar to the reader.

*[B.C.E.]:
*[HTML]:
*[PDF]:
*[CC-BY-NC-SA]:
*[CI]:
