This Hugo theme was ported from [Ivy](https://github.com/dmulholland/ivy), a minimalist website generator built in Python. I don't have time to document it. You have to read the source code to understand what it can do. Like Ivy, this theme is also released under [the Unlicense](https://en.wikipedia.org/wiki/Unlicense), which basically means you just do whatever you want.

## New features added by Alvin

This is a [hugo](https://github.com/gohugoio/hugo) theme forked from [yihui/hugo-ivy](https://github.com/yihui/hugo-ivy). Alvin has added some new features as below:

- Support Latex with [Mathjax](https://docs.mathjax.org/en/latest/configuration.html). See more details [here](https://idealvin.github.io/coding/2018/08/hugo/).

- Support [gitalk](https://github.com/gitalk/gitalk). You need modify `layouts/partials/comments.html` by yourself.

- Support `toc`(table of contents) as a `sidebar`. Just put `toc: true` at the front matter of your markdown files.
  ```yaml
  ---
  title: "xxx"
  toc: true
  ---
  ```

- Support hidding the scroll bar by adding `hide_scroll_bar: true` at the front matter of your markdown files.
  ```yaml
  ---
  title: "xxx"
  hide_scroll_bar: true
  ---
  ```
