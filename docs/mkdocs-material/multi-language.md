# Multi-language

!!! note "多語系問題"

    MKDocs 的md內容無法即時翻譯，多語問題，得分開不同document project， 並在`mkdocs.yml` 設定導引。(預計2024 會有更佳的體驗)

```yml title="mkdocs.yml"
extra:
  alternate:
    - name: English
      link: /en/ 
      lang: en
    - name: 中文正體
      link: /zh-TW/
      lang: zh-TW
```

