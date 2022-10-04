## VDL to HTML
vista document library to html




### docx to html
stores images to media file, and styles html with css
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
