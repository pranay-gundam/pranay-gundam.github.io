## Running the blog
1. Clone this repo
```
git clone https://github.com/michellexliu/pranay-blog
cd pranay-blog
```

2. Installation
Follow the steps at https://www.taniarascia.com/make-a-static-website-with-jekyll/#installing-jekyll

At the step 'create gemfile', skip the first 2 commands, and go directly to `bundle install`. Stop once you get to 'Install jekyll'

3. Run `jekyll serve` in your directory.
You should see the page at https://localhost:4000

## Editing pages
- General info: `_config.yml`
- About page: `_pages/about.md`
- Teaching page: `_pages/teaching.md`
- Blog page: `_pages/blog.md`
- My Work page: `_pages/publications.md`
- More: `_pages/cv.md`

## Editing the blog
Create a new post by adding a new file in _posts. There's an example file in the folder already. Additionally, there are some additional unpublished examples in the _examples folder. These have examples of different add-ons you can include or unique things you can do with the blog, such as adding images, comments, diagrams, etc.

## Editing projects
Projects can be created or edited in the _projects folder. Currently, the "my work" page only shows projects where the category is 'work'. You can display more categories by editing `display_categories` in `_pages/publications.md`.

## Editing papers
Papers can be edited in `_bibliography/papers.bib`. You can edit or delete any of the desired attributes. To create a new one, copy-paste the example paper and edit it. 

## Deployment
I'm assuming you want this project hosted on your own github— here are some directions for doing so https://github.com/michellexliu/pranay-blog/blob/master/INSTALL.md#deployment. If you'd like me to help with this, let me know and we can figure something out.