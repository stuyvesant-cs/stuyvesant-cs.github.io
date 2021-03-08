* Basic github pages setup guide (no local dev):http://jmcglone.com/guides/github-pages/

* Jekyll github pages page: https://jekyllrb.com/docs/github-pages/

* Setting up local Jekyll development: https://help.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll

* Things not included in these instructions:
  - When they say: `bundle exec jekyll VERSION new .`
    - they mean: `jekyll _3.8.5_ new . --force` (this may not be true anymore. haven't used this command in a long time)
  - When they say (in the Gemfile): `gem "github-pages", "~> VERSION", group: :jekyll_plugins`
    - they mean: `gem "github-pages", "~> 204", group: :jekyll_plugins`
    - update (3/8/21), looks like they mean: `gem "github-pages", group: :jekyll_plugins`
      - keeping the version info there led to the gem not being updated, therefore the locally served version did not match what gh was serving. [more info here](https://github.com/github/pages-gem)

* Using bootstrap with jekyll: http://veithen.io/2015/03/26/jekyll-bootstrap.html

* Creating navbar with bootstrap + jekyll: https://mycyberuniverse.com/jekyll-bootstrap-dynamic-navigation-highlighting-active-element.html Further information on auto navbar stuff: https://jekyllrb.com/tutorials/navigation/

* good looking math:
  - gh pages uses the kramdown markdown interpreter, this includes some built-in functionality for [mathjax](https://kramdown.gettalong.org/math_engine/mathjax.html)
  - To use mathjax, include this `<script>` tag: `<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>` [source](https://docs.mathjax.org/en/latest/web/start.html)
  - kramdown will translate any latex expression between `$$ MATH HERE $$`. If there is text on at least one side of the `$$`, the expression will be _inline_. If there are newlines on _both_ ends, the expression will be _display_, creating a separate block element and centering it [source](https://chrisyeh96.github.io/2020/03/29/mathjax3.html).
  - For the uneducated, a simple onine latex editor: <https://www.codecogs.com/latex/eqneditor.php>
