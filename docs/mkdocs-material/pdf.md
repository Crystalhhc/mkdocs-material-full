# PDF Output

- 安裝[mkdocs-pdf-export-plugin](https://github.com/zhaoterryy/mkdocs-pdf-export-plugin) 

!!! Note 
    - only available for `mkdocs-material` theme
    - 核心使用WeasyPrint

```sh
pip install mkdocs-pdf-export-plugin
```

``` yml title="mkdocs.yml"
plugins:
    - pdf-export:
        verbose: true
        media_type: print
        enabled_if_env: ENABLE_PDF_EXPORT
```

```css title="extra.css"
@page {
    size: a4 portrait;
    margin: 25mm 10mm 25mm 10mm;
    counter-increment: page;
    font-family: "Roboto","Helvetica Neue",Helvetica,Arial,sans-serif;
    white-space: pre;
    color: grey;
    @top-left {
        content: '© 2018 My Company';
    }
    @top-center {
        content: string(chapter);
    }
    @top-right {
        content: 'Page ' counter(page);
    }
}

```