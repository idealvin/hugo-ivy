This Hugo theme was ported from [Ivy](https://github.com/dmulholland/ivy), a minimalist website generator built in Python. I don't have time to document it. You have to read the source code to understand what it can do. Like Ivy, this theme is also released under [the Unlicense](https://en.wikipedia.org/wiki/Unlicense), which basically means you just do whatever you want.


## New features added by Alvin

This is a [hugo](https://github.com/gohugoio/hugo) theme forked from [yihui/hugo-ivy](https://github.com/yihui/hugo-ivy). [Alvin](https://idealvin.github.io/) has added some new features:

- **[LaTex](https://www.latex-project.org/)**  
  `LaTex` is supported with [Mathjax](https://docs.mathjax.org/en/latest/configuration.html). It has a conflict with markdown on the underscore `_`. See how it was solved [here](https://idealvin.github.io/coding/2018/08/hugo/).

- **[gitalk](https://github.com/gitalk/gitalk)**  
  - You **must** modify `layouts/partials/comments.html` with your own gitalk info. 
  - You may add a global config in [config.toml: Params](https://github.com/idealvin/blog/blob/master/config.toml#L46) to disable all comments: `comments = false`.
  - You may add `no_comment: true` or `nocom: true` at the front matter of your markdown file to disable comment of a single page.

- **[cnzz](https://www.cnzz.com/)**  
  - You **must** modify `layouts/partials/cnzz.html` with your own cnzz info.
  - You may add a global config in [config.toml: Params](https://github.com/idealvin/blog/blob/master/config.toml#L46) to disable it: `cnzz = false`.
  - The cnzz status line was hidden by default. You may replace the `.cnzz: font-size` with a non-zero value in your [style.css](https://github.com/idealvin/hugo-ivy/blob/master/static/css/style.css#L364) to display it.

- **sidebar**  
  Sidebar is automatically generated if you put `toc: true` at the front matter of your markdown files.
  ```yaml
  ---
  toc: true
  ---
  ```
  [Here](https://idealvin.github.io/coding/2020/07/co_en/) is a example.

- **Hide the scroll bar**  
  You may hide the scroll bar by adding `hide_scroll_bar: true` or `hidsb: true` at the front matter of your markdown files.
  ```yaml
  ---
  hide_scroll_bar: true
  ---
  ```


## Example site

- [idealvin.github.io](https://idealvin.github.io/).
- [markdown of idealvin.github.io](https://github.com/idealvin/blog).
- [global config: config.toml](https://github.com/idealvin/blog/blob/master/config.toml).
