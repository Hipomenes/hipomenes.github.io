---
layout: post
title: "David's IRE: quick wiki links"
published: true
categories: dh-tools
---

My transformation has begun: my brain is starting to speak VIM keybindings. 
Today I woke up with a VIM command in mind, and sure enough I went straight to the Terminal to type it down. 
Here it is.

The first command implements a basic wiki function that I had been to lazy to address in `David's IRE`: creating wiki links. 
The following string of VIM commands simply reformat the last two words to look like a wiki link, according to my own minimal convention (hyphenated words, `.md` extention, and doulbe brackets.)

The second command is a modification of the first: after creating the wiki link, it creates a file with the same name (the actual wiki file), and opens in the editor. 
Simple and beutiful.

![Wikilinks]({{"/assets/david-wiki-link.jpg" | absolute_url}})
