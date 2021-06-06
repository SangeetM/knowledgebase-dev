# A guide to hosting your first useR! Conference

__Project Title:__ useRknowledgebase


This guide is a work in progress, proper description will be added in the coming weeks once the initial roadmap is finalized.

## Technical details

It is currently tested locally and have not been deployed. To see the local version, follow the below steps:

1. Clone this git repo: git clone `https://gitlab.com/rconf/userknowledgebase/-`
1. Git checkout branch `v21.05.01`
1. Browse to the `index.Rmd`, using your terminal or prefered R editor (Rstudio, vscode etc.)
1. Execute `bookdown::render_book("index.Rmd")` to build the `bookdown` site
1. Navigate to `/docs/` and open `index.html` to view this version locally

### Build a Deployable Version

1. Make your required changes
1. Render the site locally `rmarkdown::render_site(encoding = 'UTF-8')`
1. Remove unnecessary files `bookdown::clean_book()`, although CI/CD will take care of this if you miss
1. Push a version to master / main branch and it will get deployed

Once a initial version is complete, future deployment will be done via Travis CI:

1. Any push to master will build the book and its content will be found in the `docs` directory.
1. In the upcoming days, this will be deployed using [GitHub pages](https://pages.github.com/)

## Background Resources

Details about this project can be found here [useR! Knowledgebase](https://github.com/rstats-gsod/gsod2021/wiki/useR!-knowledgebase).

## Contributing

### Without write access

Corrections, suggestions and general improvements are welcome as [issue submissions](https://gitlab.com/rconf/userknowledgebase/-/issues).

You can also suggest changes by editing the .Rmd files that are at the root of this repository and submitting a pull request. Please target your pull requests to the `master` branch.

### With write access

You can push directly to `master` for small fixes. Please use PRs to `master` for discussing larger updates - try to limit to one section or at least one chapter in each PR, so that changes are easier to review.

## Acknowledgements

This book was started using Sean Kross' [minimal bookdown example](https://github.com/seankross/bookdown-start) as described on their [blog](http://seankross.com/2016/11/17/How-to-Start-a-Bookdown-Book.html).

This README borrowed ideas from [ropensci/dev_guide](https://github.com/forwards/first-contributions)

## Changelogs
### v21.05.01
* [TODO] Setting up bookdown
* [TODO] Create issues for current milestone

## v21.05.02
* [TODO] Collate the structure information from previous conferences

## References

* [Previous Conferences](https://www.r-project.org/conferences/)
* [Bookdown homepage](https://bookdown.org/)
* [How to get started with Bookdown](https://bookdown.org/yihui/bookdown/get-started.html)
* [KnowledgeBase Project Idea](https://github.com/rstats-gsod/gsod2021/wiki/useR!-knowledgebase)
* [set of HOWTOs written by Forwards](https://github.com/forwards/conferences)
* [event best practices written by Forwards](https://github.com/forwards/event_best_practices)
* [blog post by the useR! 2021 diversity team](https://user2021.r-project.org/blog/2021/02/17/preparing-for-an-accessible-conference/)
* [satRdays knowledgebase](https://knowledgebase.satrdays.org/)
* [DISCOVER cookbook](https://discover-cookbook.numfocus.org/)
