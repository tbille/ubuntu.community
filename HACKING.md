# How to contribute to this site!?

## Run the site

This site is using the static site generator [Jekyll](https://jekyllrb.com/). 
You will need [ruby](https://www.ruby-lang.org/en/) to be installed on your system to run the site.
Here is the list of steps to run the site:

- Open a terminal
- Clone the project to your local machine: `git clone https://github.com/ubuntu-dot-community/ubuntu.community.git`
- Move to the project's folder: `cd ./ubuntu.community`
- Install bundler and jekyll: `gem install bundler jekyll`
- Run the site: ` bundle exec jekyll serve`
- Open a browser to: http://localhost:4000

## Add a new section to the site

If you want to add new section:

- Create a folder at the root of the project: `mkdir foo`
- The folder name will be the root of the url, for example if the folder is called foo, the base url will be `/foo`
- In this folder create an index file: `mkdir foo/index.md`
- This file will contain the content of the section's landing page

```md
---
layout: section
title: My awesome new section
---

Here is the content of my page. This is markdown!
```

- You can now start adding other content pages in the same folder: `mkdir foo/my-section.md`
- Those pages will become accessible from the url: `/foo/my-section`

```md
---
layout: default
title: My awesome content
---

Here is the content of my other page. This is markdown!
```
- If you want to link it from the index page of the section, you will need to add the order of the pages in the frontmatter of the index topic:

```md
---
layout: section
title: My awesome new section
order:
  - my-section.md
  - my-section-2.md
  - my-section-3.md
---

Here is the content of my page. This is markdown!
```
- This will directly add the pages linked from the index page and give them an order
- You can now open a pull-request on the repository!