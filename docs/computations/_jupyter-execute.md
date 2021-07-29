Note that when rendering an `.ipynb` Quarto **will not** execute the cells within the notebook by default (the presumption being that you already executed them while editing the notebook). If you want to execute the cells you can pass the `--execute` flag to render:

``` bash
quarto render jupyter-document.ipynb --execute
```

You can also specify this behavior within the notebook's YAML front matter:

``` yaml
---
title: "My Document"
execute: true
jupyter: python3
---
```