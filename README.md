## VDL to HTML
vista document library to html


```
pandoc --extract-media=. -s tech_manual.docx -t html -c styles.css -o tech_manual.html
```


## references
https://blog.atwork.at/post/Convert-documents-with-Pandoc


## styles.css
```css
html {
    line-height: 1.0;
    font-family: sans-serif;
    font-size: 12px;
    color: #1a1a1a;
    background-color: #fdfdfd;
 }
```
