## VDL to web-friendly form
vista document library converson to web-friendly forms



#### docx to html
converts docx to html; stores images to external media folder; adds css styling
```
pandoc --extract-media=images -s mydoc.docx -t html -c styles.css -o mydoc.html
```


#### docx to markdown
converts docx to markdown; stores images in folder
```
pandoc --extract-media=images -s mydoc.docx -t markdown -o mydoc.md
```


#### docx to github markdown
converts docx to github-friendly markdown; stores images in folder
```
pandoc --extract-media=. -s mydoc.docx -t gfm -o mddoc.md
```


#### references
https://blog.atwork.at/post/Convert-documents-with-Pandoc


#### styles.css
```css
html {
    line-height: 1.0;
    font-family: sans-serif;
    font-size: 12px;
    color: #1a1a1a;
    background-color: #fdfdfd;
 }
```
