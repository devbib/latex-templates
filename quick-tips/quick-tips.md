# Latex Quick Tips

Sebastian Raschka  
Last updated 10/25/2014

LaTeX templates

<br>
<br>

#Sections
- [Removing page numbers](#removing-page-numbers)

<br>
<br>

#### Removing page numbers 
[[back to top](#sections)]
<br>
<br>

The typical default setting for most document types is `\pagestyle{plain}`, which shows page numbers at the bottom of the page. The page numbers can be hidden globally by setting `\pagestyle{empty}`.   

However, if we are only interested in hiding page numbers on e.g., the title page, we can do so by using   
`\clearpage`  
`\thispagestyle{empty}`

Note that `\maketitle` sets the default `\pagestyle{plain}`, so if you use the `\maketitle` command, you need to make sure that it is followed by `\thispagestyle{empty}` to hide the page number of the title page:

`\maketitle`  
`\clearpage`  
`\thispagestyle{empty}`

