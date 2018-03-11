This repository contains the source code for my personal site,[davidcolmenares.org](davicolmenares.org). 

### Credits
This site is a fork of Dennis Tenen's Tachyons-based theme, used for his own [personal site](http://denten.plaintext.in). 

### Site structure
```
_pages/         # contains page content in .md
_layouts/       # contains page templates in .html
_posts/         # contains post content in .md 
_includes/      # contains partial reusable snippets like header, sidebar, footer etc.
_data/          # contains arbitrary data .yml
```
### Notes 

- Index page is slightly different from others, in that it needs to live in the root.
- To add pages create a new file in _pages/ and specify the template. Omit the title to exclude it from sidebar navigation. 
- Add a page to _pages for each new category, using the categories template.
- There are different templates for posts in different categories. This allows us to format Talks in a different way from Publicaitons, for example.


