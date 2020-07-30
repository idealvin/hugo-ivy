This Hugo theme was ported from [Ivy](https://github.com/dmulholland/ivy), a minimalist website generator built in Python. I don't have time to document it. You have to read the source code to understand what it can do. Like Ivy, this theme is also released under [the Unlicense](https://en.wikipedia.org/wiki/Unlicense), which basically means you just do whatever you want.


## New features added by Alvin

This is a [hugo](https://github.com/gohugoio/hugo) theme forked from [yihui/hugo-ivy](https://github.com/yihui/hugo-ivy). [Alvin](https://idealvin.github.io/) has added some new features:

- **[plantuml](https://plantuml.com/)**

  Add `plantuml: true` at the front matter of your markdown file to enable it. [Here](https://idealvin.github.io/coding/2020/07/site_upgrade/#%E6%97%B6%E5%BA%8F%E5%9B%BE-plantuml) is an example.

- **[LaTex](https://www.latex-project.org/)**

  `LaTex` is supported with [Mathjax](https://docs.mathjax.org/en/latest/configuration.html). It has a conflict with markdown on the underscore `_`. See how it was solved [here](https://idealvin.github.io/coding/2018/08/hugo/).

  `Mathjax` is disabled by default. Add `mathjax: true` at the front matter of your markdown file to enable it.

  - [html](https://idealvin.github.io/coding/2018/08/prime-number/)
  - [markdown](https://github.com/idealvin/blog/blob/master/content/coding/2018/08/prime-number.md)

- **[gitalk](https://github.com/gitalk/gitalk)**

  You **must** modify `layouts/partials/comments.html` with your own gitalk info.

  You may add a global config in [config.toml: Params](https://github.com/idealvin/blog/blob/master/config.toml#L52) to disable all comments: `comments = false`.

  You may add `no_comment: true` or `nocom: true` at the front matter of your markdown file to disable comment for a single page.

- **[cnzz](https://www.cnzz.com/)**

  You **must** modify `layouts/partials/cnzz.html` with your own cnzz info.

  You may add a global config in [config.toml: Params](https://github.com/idealvin/blog/blob/master/config.toml#L52) to disable it: `cnzz = false`.

  The cnzz status line was hidden by default. You may replace the `.cnzz: font-size` with a non-zero value in your [style.css](https://github.com/idealvin/hugo-ivy/blob/master/static/css/style.css) to display it.

- **sidebar**

  Sidebar is automatically generated if you put `toc: true` at the front matter of your markdown files.

  - [html](https://idealvin.github.io/coding/2020/07/co_en/)
  - [markdown](https://github.com/idealvin/blog/blob/master/content/coding/2020/07/co_en.md)

- **Hide the scroll bar**

  You may hide the scroll bar by adding `hide_scroll_bar: true` or `hidsb: true` at the front matter of your markdown files.

- **Hiden next button**

  Place the mouse on the gold dividing point on the right edge of the article, and an little button `>>` will appear, click on it to jump to the next article.

## Example site

- [idealvin.github.io](https://idealvin.github.io/).
- [idealvin.gitee.io](https://idealvin.gitee.io/).
- [markdown of idealvin.github.io](https://github.com/idealvin/blog).
- [global config: config.toml](https://github.com/idealvin/blog/blob/master/config.toml).
