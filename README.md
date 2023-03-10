# Markdown Tutorial 
This is a quick tutorial / reference for Markdown, specifially [GitHub Flavored Markdown](https://github.github.com/gfm/).

### Index
- [Introduction](#wave-introduction-to-markdown)
- [Text Basics](#pencil2-text-basics-with-markdown)
- [Links](#zap-links-in-markdown)
- [Lists](#scroll-lists-in-markdown)
- [Tables](#briefcase-tables-in-markdown)
- [Images](#sunflower-images-in-markdown)
- [Math and Science](#test_tube-math-and-science-in-markdown)
- [Emojis](#smile-emojis-in-markdown)

###### :calendar:Created February 2023

***
## :wave: Introduction to Markdown

- Markdown is a lightweight markup language created in 2004 and used to format digital content. It helps you control the size and position of text and images. It also allows you to create tables, lists and links.
- Markdown is converted to HTML in order to be displayed in the browser or other applications. 
- There are different flavors of Markdown such as [GitHub Flavored Markdown](https://github.github.com/gfm/), [Reddit Flavored Markdown](https://www.reddit.com/wiki/markdown/), [Markua](http://markua.com/#the-magical-typewriter-m-) and [more](https://en.wikipedia.org/wiki/Markdown#Variants). This tutorial will focus on [GitHub Flavored Markdown](https://github.github.com/gfm/).
- To create a Markdown file you can use notepad and save the file with the `.md` extension. Open it with your browser to view it. You could also just create a repo on GitHub and practice your GFM (GitHub Flavored Markdown) in a `README.md`.
- HTML can be embedded within Markdown.

***

## :pencil2: Text Basics with Markdown

Markup languages use symbols and specific syntax rules to format content. You can think of it as adding marks or 'marking up' 
text to modify how it is displayed after conversion.
 
Here is a reference for marking up text...

| Markdown | Output | HTML Equivalent |
|:--------:|:------:|:---------------:|
| `normal text` | normal text | `normal text` |
| `# Header One` | <h1>Header One</h1> | `<h1>Header One</h1>`|
| `## Header Two` | <h2>Header Two</h2> | `<h2>Header Two</h2>`|
| `### Header Three` | <h3> Header Three </h3> | `<h3>Header Three</h3>`|
| `#### Header Four` | <h4> Header Four </h4> | `<h4>Header Four</h4>` |
| `##### Header Five` | <h4> Header Five </h5> | `<h5>Header Five</h5>`|
| `###### Header Six` | <h6> Header Six</h6> | `<h6>Header Six</h6>`|
| `*italic text*` | *italic text* | `<em>Italic Text</em>`
| `**bold text**` | **bold text** | `<strong>bold text</strong>`|
| `***bolid italic text***` | ***bold italic text*** | `<strong><em>bold italic text</strong></em>`|
| `>blockquote text` | <blockquote>blockquote text</blockquote> | `<blockquote>blockquote text</blockquote>`|
| `~~strikethrough~~` | <s>strikethrough</s> | `<s>strikethrough</s>`|

<table>
 <tr>
  <td>&#10071;</td>
  <td>
   </br>
   Some Markdown elements such as <code># headers</code> are required to be the first characters on the lines which they appear. 
   </br></br>
   &nbsp;&#10060;<code>text # header text</code>
   </br>
   </br>
   This is because headers are known as <a href ="https://www.w3schools.com/html/html_blocks.asp"> block elements </a> in both HTML and Markdown. 
   </br>
   </br>
  </td>
 </tr>
</table>

#### Line breaks and Horizontal Rules

To form a line break in Markdown end a line with two spaces and then press 'enter' or 'return'.

Horizontal rules such as those you see sepearating sections in this tutorial are created by typing `***` on the start of a line.

***

## :zap: Links in Markdown

#### Formula

` [Link Text] (link url "Link Title") `

#### Markdown

` Go to the [index](#index "md-tutorial index") of this page. `

#### Output

Go to the [index](#index "md-tutorial index") of this page.

#### HTML Equivalent

`Go to the <a href = #index>index</a> of this page.`

***

## :scroll: Lists in Markdown
Here we will go over three types of lists. Please note that there is a space between the text and list item marker for every example.

### Unordered Lists
Unordered lists have each list item demarcated by a bullet point.

#### Markdown 
```
- item one
- item two 
- item three
```

#### Output 
- item one
- item two 
- item three

#### HTML Equivalent 
```html
<ul>
 <li>item one</li>
 <li>item two</li>
 <li>item three</li>
</ul>
```

***

### Ordered Lists

Ordered lists have each list item demarcated by numbers 1, 2, 3 etc... If an ordered list is nested each list item is then demarcated by a roman numeral i, ii, iii etc... We'll talk about [nested lists](#nested-lists) later.

#### Markdown 
```
1. item one
2. item two
3. item three
```

#### Output 
1. item one
2. item two
3. item three

#### HTML Equivalent 
```html
<ol>
 <li>item one</li>
 <li>item two</li>
 <li>item three</li>
</ol>
```


***

### Task Lists

Note for task lists that there are a total of 3 spaces, one between the dash and the left bracket, one between brackets (unless checked) and one between the right bracket and the text.

#### Markdown 
```
- [x] item one
- [ ] item two
- [ ] item three
```
#### Output 
- [x] item one
- [ ] item two 
- [ ] item three 

#### HTML Equivalent
```html
<input type="checkbox" id="itemOne" name="itemOne" value="itemOne" checked/>
<label for="itemOne"> item one </label>
<br>
<input type="checkbox" id="itemTwo" name="itemTwo" value="itemTwo"/>
<label for="itemTwo"> item two </label>
<br>
<input type="checkbox" id="itemThree" name="itemThree" value="itemThree"/>
<label for="itemThree"> item three </label>
```

***

### Nested Lists

In order to nest a list or other element such as a blockquote within a list an indentation of 4 spaces is required.

#### Markdown

```md
- item one
    - nested item one
- item two
    - nested item two
- item three
    1. nested item three
    2. nested item four
```

#### Output

- item one
    - nested item one
- item two
    - nested item two
- item three
    1. nested item three
    2. nested item four
    
#### HTML Equivalent

```html
<ul>
  <li>item one</li>
  <ul>
    <li>nested item one</li>
  </ul>
  <li>item two</li>
  <ul>
    <li>nested item two</li>
  </ul>
  <li>item three</li>
  <ol>
    <li>nested item three</li>
    <li>nested item four</li>
  </ol>
</ul>
```
***
## :briefcase: Tables in Markdown

#### Markdown

```
|Column Heading One|Column Heading Two|Column Heading Three|
|---|---|---|
|Row: 1 Column: 1|Row: 1 Column: 2|Row: 1 Column: 3|
|Row: 2 Column: 1|Row: 2 Column: 2|Row: 2 Column: 3|
|`code example`|[link example](#briefcase-tables-in-markdown)|***italic example***|
```

#### Output

|Column Heading One|Column Heading Two|Column Heading Three|
|---|---|---|
|Row: 1 Column: 1|Row: 1 Column: 2|Row: 1 Column: 3|
|Row: 2 Column: 1|Row: 2 Column: 2|Row: 2 Column: 3|
|`code example`|[link example](#briefcase-tables-in-markdown)|***italic example***|

#### HTML Equivalent

```html
<table>
 <thead>
   <tr>
     <th>Column Heading One</th>
     <th>Column Heading Two</th>
     <th>Column Heading Three</th>
   </tr>
 </thead>
 <tr>
   <td>Row: 1 Column: 1</td>
   <td>Row: 1 Column: 2</td>
   <td>Row: 1 Column: 3</td>
 </tr>
 <tr>
   <td>Row: 2 Column: 1</td>
   <td>Row: 2 Column: 2</td>
   <td>Row: 2 Column: 3</td>
 </tr>
 <tr>
   <td><code>code example</code></td>
   <td><a href="#briefcase-tables-in-markdown">link example</a></td>
   <td><em>italic example</em></td>
 </tr>
</table>
```

***
## :sunflower: Images in Markdown

#### Markdown

`![sunflower](https://studyfinds.org/wp-content/uploads/2021/08/AdobeStock_276084943-604x385.jpeg "Sunflower")`

#### Output

![sunflower](https://studyfinds.org/wp-content/uploads/2021/08/AdobeStock_276084943-604x385.jpeg "Sunflower")

#### HTML Equivalent

```HTML
<img src="https://studyfinds.org/wp-content/uploads/2021/08/AdobeStock_276084943-604x385.jpeg" alt="sunflower">
```

***
## :test_tube: Math and Science in Markdown

### Subscript

#### Markdown

` Not available in GitHub Flavored Markdown, use inline HTML `

#### Output

H<sub>2</sub>O

#### HTML Equivalent

`H<sub>2</sub>O`

### Superscript

#### Markdown

` Not available in Github Flavored Markdon, use inline HTML `

#### Output

x<sup>2</sup>

#### HTML Equivalent

`x<sup>2</sup>`

***
## :smile: Emojis in Markdown

#### Markdown

`:smile:`

#### Output

:smile:

#### HTML Equivalent

`<p>&#128516</p>`

***
