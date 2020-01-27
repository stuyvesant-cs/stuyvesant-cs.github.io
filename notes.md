Basic github pages setup guide (no local dev):http://jmcglone.com/guides/github-pages/

Jekyll github pages page: https://jekyllrb.com/docs/github-pages/

Setting up local Jekyll development: https://help.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll

Things not included in these instructions:
    When they say: bundle exec jekyll VERSION new .
        they mean: jekyll _3.8.5_ new . --force
    When they say (in the Gemfile): #gem "github-pages", "~> VERSION", group: :jekyll_plugins
        they mean: gem "github-pages", "~> 204", group: :jekyll_plugins
Using bootstrap with jekyll: http://veithen.io/2015/03/26/jekyll-bootstrap.html

Creating navbar with bootstrap + jekyll: https://mycyberuniverse.com/jekyll-bootstrap-dynamic-navigation-highlighting-active-element.html Further information on auto navbar stuff: https://jekyllrb.com/tutorials/navigation/
