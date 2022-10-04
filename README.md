## VDL to HTML
vista document library to html




### docx to html
converts docx to html; stores images to external media folder; adss css styling
```
pandoc --extract-media=. -s INPUTFILE.docx -t html -c styles.css -o OUTPUTFILE.html
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
