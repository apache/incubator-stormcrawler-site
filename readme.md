# Storm Crawler website

Built using Jekyll. To build and run server locally type 'jekyll serve'. The site can then be accessed at localhost:4000.

## How to use...

### Header nav highlighting

When a new page is added to the menu in _includes/header.html, you can highlight it when active by following these steps:

1. Add a slug to the file's YAML front-matter e.g. "slug: about". (see existing pages for working example of this.)
2. Add a rule in the Sass file (css/main.scss) using this slug as a class, and nth-child to determine which item should be highlighted.
