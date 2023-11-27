## Intro

A simple Hexo Theme based [hexo-theme-zero](https://github.com/loveminimal/hexo-theme-zero.git)

Here is a [Demo](nefelibata.icu/blog).

## Usage

### Theme Install

```sh
# cd your-blog-root-site
git clone https://github.com/kpl0111/zero.git ./themes/zero
```

### Dependence Install

+ hexo-generator-searchdb

```sh
# cd your-blog-root-site
npm install hexo-generator-searchdb --save
```

### Configuration

1. Edit the site configuration file.
   > Note that: you must disable the =highlight= of site =_config.yml=, and update =theme= fragment as =zero=.

    ```sh
    # root/_config.yml

    # highlight settings
    highlight:
        enable: false
        line_number: false
        auto_detect: false
        tab_replace:

    # theme settings
    theme: zero

    # hexo-generator-searchdb
    search:
        path: search.xml
        field: post
        format: html
    ```

2. Edit the theme configuration file

   ```sh
   # root/themes/zero/_config.yml
   # you can add or subtract menu items there
    menu:
        Nefelibata: ../
        Blog: /
        Gallery: ../gallery
        Github: https://github.com/kpl0111
        About: ../about

    excerpt_link: Read More

    favicon:
        url: /images/favicon.png

    # MathJax Support
    mathjax:
        enable: true
        cdn: https://cdn.jsdelivr.net/npm/mathjax@2.7.8/MathJax.js?config=TeX-AMS-MML_HTMLorMML
    ```
