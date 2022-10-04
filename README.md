## VDL to web-friendly form
vista document library converson to web-friendly forms



### Word to html
converts docx to html; stores images to external media folder; adds css styling
```
pandoc --extract-media=images -s mydoc.docx -t html -c styles.css -o mydoc.html
```

### Word to markdown
converts docx to markdown; stores images in folder
```
pandoc --extract-media=images -s mydoc.docx -t markdown -o mydoc.md
```

### Word to github markdown
converts docx to github-friendly markdown; stores images in folder
```
pandoc --extract-media=. -s mydoc.docx -t gfm -o mddoc.md
```



### references
https://blog.atwork.at/post/Convert-documents-with-Pandoc


### styles.css
```css
html {
    line-height: 1.0;
    font-family: sans-serif;
    font-size: 12px;
    color: #1a1a1a;
    background-color: #fdfdfd;
 }
```


<details>
  <summary>Reference Section</summary>
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>
