---
title: A Breadbaker’s Notebook
image: breadbakers-notebook.png
year: 2017–
summary: 'One passion meets another: I’m doing an ongoing experiment with Git to document the development of my bread recipes, alongside a simple cookbook-style website for the final recipes.'
external_link:
  url: https://github.com/dananjohnson/breadbakers-notebook
  title: View on Github
order: 2
---

Like probably most home bakers, I have a notebook filled with the bread formulas I’ve developed, tested, tried to preserve, and mostly forgotten about. As much as I love handwritten recipes, I became frustrated trying to track down an old formula, and, most of all, adequately tracking how a formula evolved over time. I know others use spreadsheets for these reasons. I hate spreadsheets.

I began thinking about the potential of Git’s versioning and archiving power and a simple data format like YAML to create a durable, flexible, living repository for my formulas.

My formulas don't develop linearly. While there may be a “master” version, ingredients, quantities, and methods change from bake to bake without necessarily replacing the previous version of the recipe. Some turn into new recipes, others dead ends, while still others become alternatives — riffs on a theme.

{% include responsive-img.html.liquid src="bread-formula-log.png" alt="The bread formula repository with commit history and branches" %}

This [GitHub repository](https://github.com/dananjohnson/bread-formulas) attempts to document the riverine development of these formulas. Recipe experimentation and evolution are tracked in branches, one branch per recipe. All recipes are at some stage of development; some are close but need minor tweaking, others may be disasters. If I make a second attempt at a recipe, I track that attempt on a new branch; if it’s successful, I merge it into the main branch for that recipe; if not; it simply stays put, but preserved.

The recipes that I consider *good enough* — an amorphous, perfectionistic, and excessively subjective classification — are merged into the master branch, and then published on [A Breadbaker’s Notebook](https://github.com/dananjohnson/breadbakers-notebook), a simple, Jekyll-based “cookbook” website.

{% include responsive-img.html.liquid src="breadbakers-notebook.png" alt="An example recipe on A Breadbaker’s Notebook" %}

I’ve created A Breadbaker’s Notebook as a more user-friendly GUI for the project, an attractive place for good recipes to reside. Think of it as the equanimous facade for the chaotic laboratory. I use [Jekyll](https://jekyllrb.com/) for site generation and [Travis CI](https://travis-ci.org/) for continuous deployment, and the recipe formatting employs structured data to maximize readability to search engines and other third parties.

Both the website code and the recipes are released under the MIT license, and, like a well-fed sourdough starter, are undergoing continuous development.

*[YAML]:
*[GUI]:
*[MIT]:
*[CI]:
