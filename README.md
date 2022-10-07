# Web documentation toolchains


### Micorosoft toolchain

Microsoft documentatioin toolchain:
https://github.com/MicrosoftDocs



### Pandoc toolchain
Vista document library converson to web-friendly forms using pandoc. Images stored in external images/media folder; html styles in styles.css file.  Reference: https://blog.atwork.at/post/Convert-documents-with-Pandoc

```text
Word to html:
pandoc --extract-media=images -s INPUT.docx -t html -c styles.css -o OUTPUT.html

Word to markdown:
pandoc --extract-media=images -s INPUT.docx -t markdown -o OUTPUT.md

Word to github markdown:
pandoc --extract-media=images -s INPUT.docx -t gfm -o OUTPUT.md

Styles.css:
html {
    line-height: 1.0;
    font-family: sans-serif;
    font-size: 12px;
    color: #1a1a1a;
    background-color: #fdfdfd;
 }
```

