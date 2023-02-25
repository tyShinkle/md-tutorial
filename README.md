# Markdown Tutorial 
:wave: Hello, this is a quick tutorial / reference for Markdown, specifially [GitHub Flavored Markdown](https://github.github.com/gfm/).

### Index
- [Introduction](#zap-introduction-to-markdown)
- [Text Basics](#zap-text-basics-with-markdown)
- [Lists](#zap-lists-in-markdown)
- [Tables](#zap-tables-in-markdown)
- [Images](#zap-images-in-markdown)
- [Math and Science](#zap-math-and-science-in-markdown)
- [Emojis](#zap-emojis-in-markdown)

###### :calendar:Created February 2023

***
## :zap: Introduction to Markdown

- Markdown is a lightweight markup language created in 2004 and used to format digital content.
- Markdown is converted to HTML in order to be displayed in the browser or other applications. 
- There are different flavors of Markdown such as [GitHub Flavored Markdown](https://github.github.com/gfm/), [Reddit Flavored Markdown](https://www.reddit.com/wiki/markdown/), [Markua](http://markua.com/#the-magical-typewriter-m-) and [more](https://en.wikipedia.org/wiki/Markdown#Variants). This tutorial will focus on [GitHub Flavored Markdown](https://github.github.com/gfm/).
- To create a Markdown file you can use notepad and save the file with the `.md` extension. Open it with your browser to view it. You could also just create a repo on GitHub and practice your GFM (GitHub Flavored Markdown) in a `README.md`.
- HTML can be embedded within Markdown.

***

## :zap: Text Basics with Markdown

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

***

## :zap: Lists in Markdown
Here we will go over three types of lists. Please note that there is a space between the text and list item marker for every example.

### :arrow_down_small: Unordered Lists
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

### :arrow_down_small: Ordered Lists

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
### :arrow_down_small: Task List

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
<input type="checkbox" id="itemOne" value="one">
<label for="itemOne"> item one </label>
```
<input type="checkbox" id="itemOne" name="itemOne" value="one">
<label for="itemOne"> item one </label>

***
## :zap: Tables in Markdown
***
## :zap: Images in Markdown
***
## :zap: Math and Science in Markdown
***
## :zap: Emojis in Markdown
***
