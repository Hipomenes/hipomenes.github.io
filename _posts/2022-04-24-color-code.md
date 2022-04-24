---
layout: post
title: "Automatic Color Coded Notes in Vim"
published: true
categories: think
---

I have used a color code in my hand written notes since the grad school.
I experimented with several "syntax highlighting" schemes (i.e. definitions of what should be highligted in ), as well as colors to reflect this syntax: from as many as 5, which of course was unwieldy, to as minimum of two, which I still tend to use when writing with fountain pens.
For several years, I used the same color code in my hand written notes and in RTF text files, which in retrospective sounds maddeing: I had to manually edit the color attribute of text files. 

When I adopted Markdown + Pandoc method around 2016, and then learned to use VIM, I abondend my old color code scheme and settled for Vim-Panoc's beautiful syntax highligting. 
The structure text that these creates by default is good enough, and preserves the inmense advantage of color coding, which is to allow you identify semantically relevant fields at a glance, even if most of them have to do with the Markdown syxtax (an exception to this is the default coloring of strings of text in cursive, which tend to be titles, text within foonotes, and block quotes.)

But I recently decided to try my hand at enriching vim-Pandoc syntax highlighting with some custom definitions that recover part of my original color code.
In my hand notes, I always use a different ink (generally blue) to indicate quoted words; words that are not mine.
This should be easy, considering that quoted text is are conventionally written... surounded by quotes.
So after a few hours tinkering with Vim I was able to have this working custom syntax added to the standard (and excellent) Vim-Pandoc-Syntax.
The key is to add this rules to a new file: `~/.vim/after/syntax/pandoc.vim`

![pandoc.vim](/assets/sc1.png)

These commands simply define a new highliting group (`inlineQuote`) based on a simple regex. (TODO: simply this regex as much as possible), and then assign it the highliting color `Constant`.

The result is this beatiful combination of markdown syntax highliting (using the Vim's conceal function) plus the fundamental element of my old color code: anything that is a quoted text should be in a different color.

![pandoc.vim](/assets/sc2.png)

## Todo

- Simply the regex as much as possible, and try to avoid potential conflict with Markdown's footnote syntax.
- Maybe implement a highliting group that identifies proper names (techicanlly, two or three words in a row that begin with a capital letter), the second most important element of my note-taking color code.
