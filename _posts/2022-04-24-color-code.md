---
layout: post
title: "Automatic Color Coded Notes in Vim"
published: true
categories: think
---

I have used a color code in my hand-written notes since grad school.
I experimented with several "syntax highlighting" schemes (i.e. definitions of what should be highligted, such as quotes, references, concepts, etc. ), as well a color palette to reflect the syntax. These palettes have ranged from as many as five colors, which of course was unwieldy, to a minimum of two, which I still tend to use when writing with fountain pens.

For several years, I used the same color code in my hand-written notes and in RTF text files, which in retrospect sounds maddening: I had to manually edit the color attribute of every string. (At the time I was frankly obsessive about this, and even used small caps for titled, etc.)
Here's a recent note with somewhat lazy color coding:

![notas](/assets/IMG_0183.jpg)

When I adopted Markdown + Pandoc as my scholarship writing method in 2017, and then learned to use Vim, I abondend my old color code scheme and settled for Vim-Panoc's beautiful syntax highligting. (I kept using it, though, in my hand-written notes.)
The structured text that this creates by default is good enough, and preserves the inmense advantage of color coding, which is to allow you to identify semantically relevant fields at a glance, even if most of these have to do with the Markdown syxtax (an exception to this is the default coloring of strings of text in cursive, which tend to be titles; text within foonotes; and block quotes.)

But I recently decided to try my hand at enriching Vim-Pandoc syntax highlighting with some custom definitions that recover part of my original color code.
In my hand notes, I always use a different ink (generally blue) to indicate quoted words; words that are not mine and that I want to be able to spot at a glance.
This should be easy, considering that quoted text is conventionally written... surounded by quotes.
So after a few hours tinkering with Vim I was able to have this working custom syntax added to the standard (and excellent) Vim-Pandoc-Syntax.
The key is to add these rules to a new file: `~/.vim/after/syntax/pandoc.vim`, wich Vim reads after having read the standard pandoc syntax script.

![pandoc.vim](/assets/sc1.png)

These commands simply define a new highliting group (`inlineQuote`) based on a simple regex, and then assigns it the highliting color `Constant`, which looks good in most colorschemes (here I'm using Seoul).

The result is a beatiful combination of markdown syntax highliting (using the Vim's conceal function) plus the fundamental element of my old color code: anything that is a quoted text should be in a different color. Notice also all text in cursive (including book titles and words in a foreign language) highlighted in orange.

![pandoc.vim](/assets/sc2.png)

## Todo

- Simply the regex as much as possible, have it ignore the actual quote signs, and try to avoid potential conflict with Markdown's footnote syntax.
- Maybe implement a highliting group that identifies proper names (techicanlly, two or three words in a row that begin with a capital letter), the second most important element of my note-taking color code.
