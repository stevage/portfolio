---
title: Wikitext grammar
subtitle: A formal grammar for Wikipedia's markup language, in ANTLR.
layout: default
modal-id: 3
date: 2008-02-11
img: wikitext-grammar.png
thumbnail: thumbs/wikitext-grammar-thumb.png
alt: 
project-date: February 2008
tech: ANTLR
category: Personal project
description: 
---
Wikitext, the markup language in which Wikipedia is written, is notoriously hard to parse, and is poorly defined. I embarked on the fool's errand of writing a formal grammar, in [ANTLR](http://www.antlr.org/), a Java-based tool which generates parsers from grammars. The parser was able to handle approximately 90% of existing pages. Which, in real world terms, is completely useless.

It is preserved [here](https://www.mediawiki.org/wiki/Markup_spec/ANTLR/draft).