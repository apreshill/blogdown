# blogdown <a href='https://pkgs.rstudio.com/blogdown'><img src='man/figures/logo.png' align="right" height="139" /></a>

<!-- badges: start -->
[![R-CMD-check](https://github.com/rstudio/blogdown/workflows/R-CMD-check/badge.svg)](https://github.com/rstudio/blogdown/actions)
[![CRAN status](https://www.r-pkg.org/badges/version/blogdown)](https://CRAN.R-project.org/package=blogdown)
[![Coverage status](https://codecov.io/gh/rstudio/blogdown/branch/master/graph/badge.svg)](https://codecov.io/github/rstudio/blogdown?branch=master)
<!-- badges: end -->

An open-source (GPL-3) R package to generate static websites based on [R Markdown](https://rmarkdown.rstudio.com) and [Hugo](https://gohugo.io). 

## Book

<a href="https://bookdown.org/yihui/blogdown/"><img src="https://bookdown.org/yihui/blogdown/images/cover.png" alt = "blogdown: Creating Websites with R Markdown" height="400"></a>

## Installation

You can install the package via CRAN as follows:

```r
install.packages('blogdown')
```

If you want to use the development version of the **blogdown** package, you can install the package from GitHub via the [**remotes** package](https://remotes.r-lib.org):

```r
remotes::install_github('rstudio/blogdown')
```
## Usage

You may create a new site via the function `blogdown::new_site()` under an _empty_ directory. It will create a skeleton site, download a Hugo theme from Github,  add some sample content, launch a web browser and you will see the new site. The sample blog post `hello-world.Rmd` should be opened automatically, and you can edit it. The website will be automatically rebuilt and the page will be refreshed after you save the file.

If you use RStudio, you can create a new RStudio project for your website from the menu `File -> New Project -> New Directory -> Website using blogdown`.

The function `blogdown::serve_site()` may be the most frequently used function in this package. It builds the website, loads it into your web browser, and automatically refreshes the browser when you update the Markdown or R Markdown files. Do not use the command line `hugo server` to build or serve the site. It only understands plain Markdown files, and cannot build R Markdown.

You may not be satisfied with the default site created from `new_site()`. There are two things you may want to do after your first successful experiment with **blogdown**:

1. Pick a Hugo theme that you like from https://themes.gohugo.io. All you need is its Github user and repository name, to be passed to the `theme` argument of `new_site()`.
2. Add more content (pages or posts), or migrate your existing website.

## Getting help

There are two main places to get help:

1. The [RStudio community](https://community.rstudio.com/tags/c/R-Markdown/10/blogdown) is a friendly place to ask any questions about **blogdown**. Be sure to use the `blogdown` tag.

1. [Stack Overflow](https://stackoverflow.com/questions/tagged/blogdown) is a great source of answers to common **blogdown** questions. Use the tags [`[r][blogdown]`](https://stackoverflow.com/questions/tagged/blogdown+r) if you ask a question.
