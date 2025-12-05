# HTML Complete Notes

## Chapter 0: Introduction

### HTML: Hyper Text Markup Language
* HTML is the language of the web. It is used to create websites.
* We use HTML tags to define look & feel of a website.
* With understanding of these tags and How to put them together, we can create beautiful websites easily!

### Then why CSS & JavaScript
* **HTML** is used for defining layout of a page - A barebone page structure.
* **CSS** is used to add styling to that barebone page Created using HTML.
* **Java Script** is used to program Logic for the page layout eg.
    * What happens when a user hovers on a text, when to hide or show elements etc.

### A Beautiful analogy
* **HTML** = Car body (only metal)
* **CSS** = Car paint, decoration etc.
* **Java Script** = Car engine + Interior logic

We will start learning how to build beautiful layouts in this course.

---

### Installing VS Code
We can use any text editor of our choice. Here I am using VS Code because it is light weight, open source & from Microsoft. [cite: 24-29]

* Go to google, type VS Code & install it.
* **Note:** You can write HTML even in Notepad. Text editors like VS Code just makes these things easier.

---

## Chapter 1 - Creating our first website

We start building a website by creating a file named `index.html`. `index.html` is a special filename which is presented when the website root address is typed.

### A Basic HTML Page

```html
<!Doctype html>
<html>
    <head>                    
        <title> Maya's Website </title>
    </head>
    <body>                    
        <h1> This is a heading </h1>     
        <p> My paragraph </p>            
    </body>                   
</html>
````

A tag is like a container for either content or other HTML tags.

**Processing Flow:**

```text
+---------------+           +-----------+           +---------------+
| HTML Document |  ----->   |  Browser  |  ----->   | Rendered page |
+---------------+           +-----------+           +---------------+
```

### Importent Notes

  * Head & body tags are children of HTML tag.
  * HTML is the parent of Head & Body tags.
  * Most of the HTML elements have opening & closing tag with content in between opening & closing tags.
  * Some HTML tags have no Content. These are called Empty elements eg `<br>`.
  * We can either use `.htm` or `.html` extension.
  * You can use "Inspect Element" or "View Page Source" option from chrome to look into a website's HTML Code.
  * **HTML element** = Start tag + Content + End tag

### Comments in HTML

Comments in HTML are used to mark text which should not be parsed. They can help document the source code.

```html
<!-- html comment —->
```

### Case Sensitivity

HTML is a case insensitive language. `<H1>` and `<h1>` tags are the same.

-----

### Chapter 1 - Practice Set

1.  Inspect your favorite website and change something on the page which is displayed.
2.  Go to your favorite website and try to view the page Source and write the exact lines of code. Does it Clone the website? why?
3.  Write any HTML code inside a text file. Does it work if you write it using notepad?

-----

## Chapter 2 - Basic HTML Tags

We can add elements inside the body tag to define the page layout.

### HTML Element

Everything from starting to the ending tag
`<body>` (Opening tag) -\> Content -\> `</body>` (Closing tag)

### HTML Attributes

Used to add more information corresponding to an HTML tag.

**Example: Anchor tag**

```html
<a href = "https://techtentacles.xyz/"> Tech Tentacles </a>
```

  * `href` attribute
  * We can either use single or double quotes in attributes.

### The Heading Tag

Heading tag is used to mark headings in HTML.
From `h1` to `h6`, we have tags for the most important to the least important heading.

| Tag | Content |
| :--- | :--- |
| `<h1>` | Most Important heading |
| `<h2>` | Another heading H2 |
| `<h3>` | Another heading H3 |
| `<h4>` | Another heading H4 |
| `<h5>` | Another heading H5 |
| `<h6>` | Another heading H6 |

**Note:** We should not use HTML headings to make text thick or bold.

-----

### The Paragraph Tag

Paragraph tags are used to add paragraphs to an HTML page.

```html
<p> This is a paragraph </p>
```

### The Anchor Tag

The Anchor tag is used to add links to an existing Content inside an HTML page.

```html
<a href="https://google.com"> Click me </a>
```

### The img Tag

img tag is used to add images in an HTML page.

```html
<img src="image.jpg" >
```

(relative url of an image)

### Bold, italic and underline tags

We can use bold, italic and underline tags to highlight the text as follows:

  * `<b> This is bold </b>`
  * `<i> This is italic </i>`
  * `<u> This is underline </u>`

### br tag

The br tag is used to create line breaks in an HTML document.

-----

### big and small tags

We can make the text a bit larger and a bit smaller using big and small tags respectively.

### hr tag

`<hr>` tag in HTML is used to create a horizontal ruler often used to separate the content.

### Subscript & superscript

We can add subscript and superscripts in HTML as follows:

  * `<sub> this </sub>` is subscript
  * `<sup> this </sup>` is superscript

### pre tag

HTML always ignores extra spaces and newlines. In order to display a piece of text as is, we use pre tag.

```html
<pre>
  This
     is written
        using pre
               tag
</pre>
```
-----

### Chapter 2 - Practice Set

1.  Create an HTML page with a heading (title heading), a primary heading and a subheading. Which tags did you use?
2.  Create a page with 5 wallpaper images taken from the internet.
3.  Use `br` and `hr` tags to display a piece of text with linebreaks.
4.  Try to write the following Chemical equation using HTML.
    C + O2 -\> CO2
5.  Try to write a wikipedia article using HTML.

-----

## Chapter 3 - Creating a page layout

When we use the right tag in right place, it results in a better page layout, better indexing by search engines and better user experience.

We use the following tag to get the job done.

**Page Layout Structure:**

```text
+---------------------------------------------+
|                  <header>                   |
|            (Contains nav tag)               |
+---------------------------------------------+
|                   <main>                    |
|              (Website layout)               |
|                                             |
|   [<section>]     [<article>]     [<aside>] |
| (A page section) (Self contained) (Ads etc) |
|                                             |
+---------------------------------------------+
|                  <footer>                   |
+---------------------------------------------+
```

**Inside the main tag we insert the following tags:**

  * `<main>` -\> The main opening tag
  * `<section>` -\> A page section.
  * `<article>` -\> a self contained content.
  * `<aside>` -\> Content aside from the content (eg. Ads etc)
  * `</main>` -\> The main closing tag

Creating a page like this is not necessary but it creates a readable & structured layout.
Also they are useful for SEO.

### Link attributes

  * `<a href = "/Contact" > Contact us </a>` -\> Contact page opens in Same tab
  * `<a href = "/ Contact" target="_blank"> Contact us </a>` -\> opens in a new tab

We can put any content inside an anchor tag (images, headings etc are all allowed).

-----

If the page is inside a directory, we need to make sure that we link to the correct page. Same applies to img tag as well.

We can add links to images like this:

```html
<a href = "/about"> <img src='a.jpg' width="120" > </a>
```

(Height will be set automatically)

### The Div tag

`div` tag is often used as a container for other elements.
`div` is a block level element. Always takes full width.

### The Span tag

`span` tag is an inline Container. Takes as much width as necessary.

-----

### Chapter 3 - Practice Set

1.  Create an SEO friendly wesbite using HTML.
2.  Create an HTML page which opens google when Clicked on an image.
3.  Create a website which has your 5 top used websites bookmarked. The links should open in a new tab.

-----

## Chapter 4 - Lists, tables & forms

### Lists

Lists are used to display content which represents a list.

  * **Unordered list:** Used to list unordered items

    ```html
    <ul>
      <li> Home </li>
      <li> About </li>
    </ul>
    ```

  * **ordered list:** used to list ordered items

    ```html
    <ol>
      <li> Phone </li>
      <li> PC </li>
      <li> Laptop </li>
    </ol>
    ```

### Tables

The `<table>` tag is used to define tables in HTML. It is used to format & display tabular data.

  * `tr` tag: used to display table row
  * `td` tag: used to display table data 
  * `th` tag: used in place of table data for displaying table headers 

We can define as many table rows as we want.

-----

To add a caption to the table, we use `<caption>` tag inside table.

  * `thead` tag: used to wrap table head (Caption & tr with th)
  * `tbody` tag: used to wrap the table body

### Colspan attribute

This attribute is used to create cells spanning multiple Columns.

**Table Colspan Example:**

```text
+-----------------------------+
|            Maya             |  <-- th colspan="3"
+---------+---------+---------+
|    1    |    2    |    3    |  <-- Spans 3 columns
+---------+---------+---------+
```

```html
<th colspan = "3"> Maya </th>
```

### HTML forms

An HTML form is used to collect input from the user.`form` tag is used for the same.

```html
<form>
  </form>
```

There are different form elements for different kinds of user input

  * **input element:** Can be of type text, checkbox, radio, button and Submit. We also have a file type.
  * **textarea element:** Defines a multi line text input. Cols and rows attributes can be used to size the textarea.
  * **select element:** Defines a drop down list.

-----

**Note:**
You dont have to remember all the tags, you will automatically memorize them with practice.

### Embedding Videos

Video tag is used to play videos in HTML.

```html
<video src = 'Maya.mp4' > Error </video>
```

**Attributes for video**

  * **Width:** To adjust width of a video (Height automatically adjusts) 
  * **autoplay / loop:** to autoplay or loop the video.

-----

### Chapter 4 - Practice Set

1.  Create an HTML page with video embedded inside it.
2.  Replace this video in 1 with a YouTube video.
3.  Create an HTML form for a travel website to book a vacation.
4.  Create a table displaying score of cricket players in a match using HTML.

-----

Chapter 5 - SEO

We will focus only on HTML standpoint of SEO. [cite_start]We will not be looking into keyword building and Content optimization aspect of SEO. [cite: 324-328]

### Types of SEO

  * On page SEO
  * Off page SEO

### HTML SEO

\-\> Can be done by HTML developers

HTML developers can implement SEO using the following techniques:

1.  Set the title very nice & to the point.
2.  Set the meta description.

    ```html
    <meta name="description" Content = " ...">
    ```

3.  Set a nice URL Slug.
4.  Set the meta keywords tag.
5.  Set the meta author tag.

    ```html
    <meta name="author" content = "Maya">
    ```

6.  Set a favicon.
7.  Compress images & other resources.
8.  Remove unused HTML/CSS & JS files + Compress them.
9.  Add alt text to images.

<!-- end list -->
