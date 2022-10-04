## VDL to web-friendly form
Vista document library converson to web-friendly forms using pandoc. 

Images are stored in external 'images' folder; styling is referenced to in styles.css file. 



__Word to html__
```
pandoc --extract-media=images -s mydoc.docx -t html -c styles.css -o mydoc.html
```

__Word to markdown__
```
pandoc --extract-media=images -s mydoc.docx -t markdown -o mydoc.md
```

__Word to github markdown__
```
pandoc --extract-media=images -s mydoc.docx -t gfm -o mddoc.md
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
    
### Heading
    
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>
