---
title: Modelica Language 3.6 being released
author: MAP Lang
category: association
---

#### Modelica Language Specification 3.6 being released on

The new Modelica Language Specification has been accepted by MAP-Lang and will later be voted on by Modelica Association.

It provides three main new highlights to ease the development of Modelica models, and 100+ minor improvements.
https://specification.modelica.org/master/modelica-revision-history.html#main-changes-in-modelica-3-6

The following is a short description of those highlights, but each comes with a rationale giving more details and additional uses.
* [Undefined modification](https://specification.modelica.org/master/inheritance-modification-and-redeclaration.html#removing-modifiers-break) - this allows making a parameter undefined, e.g., to force users of the model to explicitly set it.
* [Selective Model Extension](https://specification.modelica.org/master/inheritance-modification-and-redeclaration.html#selective-model-extension) - this allows inheriting a model and removing some parts, e.g., to remove a simple connection to replace it by a filter. See also the [conference paper](https://ep.liu.se/en/conference-article.aspx?series=ecp&issue=157&Article_No=29).
* [Multilingual support of Modelica](https://specification.modelica.org/master/packages.html#multilingual-descriptions) - this allows providing for instance a German translation of a Modelica Library without changing the Library itself.

Several tools have already developed full implementations or protypes for these features, including the user experience (e.g., making modifiers undefined or deselecting components in the user interface).

The Multilingual support in the language is intended as a first step to allow library developers to provide translations in a tool-independent way.

##### Modelica Assocation Project Language

Webpage: [Github page](https://github.com/modelica/ModelicaSpecification).
