# Web documentation toolchains


## Microsoft toolchain
https://github.com/MicrosoftDocs



## Pandoc toolchain
Vista document library converson to web-friendly forms using pandoc.  
Images stored in external images/media folder; html styles in styles.css file.  
https://blog.atwork.at/post/Convert-documents-with-Pandoc

__Word to html__  
pandoc --extract-media=images -s INPUT.docx -t html -c styles.css -o OUTPUT.html

__Word to markdown__  
pandoc --extract-media=images -s INPUT.docx -t markdown -o OUTPUT.md

__Word to github markdown__  
pandoc --extract-media=images -s INPUT.docx -t gfm -o OUTPUT.md

__Styles.css__   
```
html {
    line-height: 1.0;
    font-family: sans-serif;
    font-size: 12px;
    color: #1a1a1a;
    background-color: #fdfdfd;
 }
```

