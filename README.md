## VDL to web-friendly form
Vista document library converson to web-friendly forms using pandoc.  
Images stored in external images/media folder; html styles in styles.css file. 



__Word to html__
```
pandoc --extract-media=images -s INPUT.docx -t html -c styles.css -o OUTPUT.html
```

__Word to markdown__
```
pandoc --extract-media=images -s INPUT.docx -t markdown -o OUTPUT.md
```

__Word to github markdown__
```
pandoc --extract-media=images -s INPUT.docx -t gfm -o OUTPUT.md
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

