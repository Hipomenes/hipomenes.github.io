---
layout: post
title: "Brinton's Scholarly Output"
published: true
categories: think.stack
---

![](/assets/brinton-output.jpg)

*No comments.*

# Testing Code Block

```
" DAVID'S IRE - Color Code
" An implementation of my old note taking color code through 
" an extended Vim-Pandoc-Syntax file

hi! link pandocEmphasis ModeMsg 

" Experimental quoted string matching. Ideally, it would not highlight footnotes.
" This baby is working! By mindful of possible lags, and study the REGEX
" for possible simplication, for example, adding typographic quotes.

syn match inlineQuote '\v(").{-}\1'
hi! link inlineQuote Constant 
```
