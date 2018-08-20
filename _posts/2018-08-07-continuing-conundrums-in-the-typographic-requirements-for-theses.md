---
layout: post
title: Continuing Conundrums in Typographic Requirements
published: true
categories: think.stack
---

I think it's a safe bet to assume that extremely few people are likely to read or perhaps even open the 600 page manual of the LaTeX Memoir Class (last revision, 2018/04/04). Unbeknownst to the Word-loving masses, Peter Wilson, the mastermind behind this, one of the all-time classics of LaTeX typography and its painstakingly detailed manual, was not only a devoted typographer but was also endowed with a bitter sense of humor. The hefty manual is full of sneers at what Wilson considered the repeating offenders of typographic good taste. And among the vast numbers of them, no one received more gibes than dissertations requirement committees.

![Peter Wilson's example of a dissertation title page. Nice.]({{"/assets/wilson.jpg" | absolute_url}})

This of course is hardly surprising. After devoting thousands of hours to the careful crafting of a high-level typographic framework such as the Memoir class, the standard requirements of American university dissertations must appear as an abomination. Even for someone with an basic typographic literacy as yours truly, it's easy to see that the idea of typesetting a work of careful scholarship into a format that looks like a sales-team memo written in a type writer is upsetting. If anything, sales-team memos from the typewriter age were single spaced, and thus exempted from what Wilson considers the cardinal sin of dissertation requirements: double spacing. The horrid, unreadable and wasteful double spacing.

Lets consider, for instance, the opening remarks of section 3.2.2 of the Memoir class manual (let me insist: a technical manual), devoted to the Horrid Double Space:

>"Some of those that have control over the visual appearance of academic theses like them to be ‘double spaced’. This, of course, will make the thesis harder to read but perhaps that is the purpose, or maybe they have stock (shares) in papermills and lumber companies, as the theses were usually required to be printed single sided as well."

The section that is meant to provide technical instruction to the humble student trying to figure out the way to comply with his university requirements thus begins with an incipit that denounces a cabal formed by shadowy academic administrators and paper mill stock holders. Sweet.

This is not to say that Wilson fails to accommodate for the typographic requirements of the Secret Cabal of Bad Typographic Taste. In this, as in everything else, he's minute to the point of obsession. In fact, one of the most detailed examples of the Memoir manual is the one devoted precisely to an hypothetical thesis, that spans over dozens of pages and illustrates the way to use LaTeX almost against itself to produce the capricious and ugly format of a Standard Dissertation. But even in doing so, Wilson's jabs never cease. Consider, for example, the dissertation's title, that is also the title of this blog post. 

But my favourite jab against the Secret Cabal appears in a footnote to the double space command,[^2] in which Wilson notes the ultimate paradox of dissertation requirement committees: by stating their capricious rules in a different format, they inevitably undermine their own authority. Lest I'm not believed, I transcribe this precious moment of Borgesian poetry:

![Committes apply the rules except for themselves.]({{"/assets/wilson-fn.jpg" | absolute_url}})

Let me formulate this self-defeating paradox as a question: Why are dissertation requirements prescribing double-space text invariably typed in single space?[^1]

Oh, Wilson.

[^1]: Which, by the way, reminds me of a famous apothegm that only makes sense in Spanish: "¿Por qué 'todo junto' se escribe separado y 'separado' todo junto?"
[^2]: For those unlikely to be interested, the correct Memoir command is ``\DoubleSpacing``.
