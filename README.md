# Class 1

Internet: Interconnected y Network
Network of computers connected all world.

Tim Berners-Lee is the inventor of the `World Wide Web`.
He found the consortium W3C to standardize the development of Internet-based technologies.

## Terminology

* HTTP Hyper Text Transfer Protocol 😕/ (Allows the data transmission among devices)
* URL Uniform Resource Locator: (Address of a website)
* HTML Hyper Text Markup Language (Language to describe the structure of a website )

In 1994 appears CSS Cascade Style Sheets.

# Class 2

<img src="https://static.platzi.com/media/user_upload/HTMLCSSJAVASCRIPT-57ccabed-3d50-4cb9-894c-4a66b75fa62c.jpg" width="400" height="500">

## HTML
Is a markup language, that allow us to structure all our websites.

* https://htmlreference.io/

## CSS
Is a stylesheet language. CSS help us to stylize our website. 

* https://cssreference.io/

# Class 3

## DOM (Document Object Model)
Transcript the HTML instructions to objects readable by the browser.

## CSSOM
Transcript the CSS instructions to objects readable by the browser.

## RENDER TREE
Is a tree integrated by the DOM & CSSOM to render in the browser the HTML & CSS instructions written by the developer.

## RENDER PROCESS (1 -> 2 -> 3 -> 4 -> 5)
1. Bytes: The browser takes the code and transcript it in bytes.
2. Characters: Transcript the **bytes** in characters depending of the coding. E.g. UTF-8.
3. Tokens: Transform the **characters** in tokens, identifying the meaning of the characters relating them to tags that generate certain type of content.
4. Nodes: They are the transformation of the **tokens** in objects that the browser understand and knows how to interpret.
5. DOM: All **nodes** are ordered in a hierarchical tree where each object will have a position depending of its tag.

## BROWSER PROCESS (1 -> 2 -> 3 -> 4 -> 5)
1. Process HTML and builds the DOM.
2. Process CSS and builds the CSSOM.
3. Join the trees (DOM & CSSOM) in a "big" render tree.
4. Executes the render tree and paint it.
5. Print the node to the screen (to the user).

# Class 4

<img src="https://static.platzi.com/media/user_upload/Infografia-Frontend-Javascript-86c602ef-a014-47d7-aadd-1293726d06b2.jpg" width="600" height="650
">

# Class 5

## Anatomy of an html element : Attributes, nesting and empty elements

Is composed by an *opening tag*, *content* and a *closing tag*.

```<h1> Hello world </h1>```

In the above example, we have an **h1** tag (h1 ~ h6).

### Opening tag
* Must contain  the name of the **element** enclosed between `<>`.

### Content
* Here is located the information will be shown.

### Closing tag
* Must contain  the name of the **element** enclosed between `</>`.

## Attributes
An attribute allow us to give an ID to the html element, then with the ID using CSS modify its characteristics.

The attributes always will be located in the **opening tag**

### Structure
< element attribute="value">`

E.g.:

`<h1 class="greeting">`

## Nesting
Some elements could be nested to another ones. 

In the following code, as you can see, < h1 > and < ul > are inside to the < body > element and < li > is nested to < ul >

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>List</title>
</head>
<body>
    <h1>TO-DO List</h1>
    <ul>
        <li>Read half hour</li>
        <li>Meet with my leader</li>
        <li>Create a pull request</li>
        <li>Go to the meetup</li>
        <li></li>
    </ul>
</body>
</html>
```

## Empty elements

Some elements don´t require a content  to be used, nevertheless need some special attributes to render or do something as `img` element.

``` <img src="image.png" alt="My image"> ```

# Class 6

## Anatomy of an html element : DOCTYPE, html, head & body
All done in this class is shown in the file `class6.html`

# Class 7

## Functions of the more important HTML tags

### Adding styles and/or scripts
If you want to add JavaScript and/or CSS implementations the tags `style` and `script` must be added to the HTML code into the root tag (< html >).

```
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Document</title>
</head>
<style>
    /* Here goes CSS */
</style>
<script>
    // Here goes JavaScript
</script>
<body>
  
</body>
</html>
```

## List of empty elements

<ul>
    <li>img</li>
    <li>input</li>
    <li>br</li>
    <li>hr</li>
</ul>

## List of semantic elements

<ul>
    <li>header</li>
    <li>nav</li>
    <li>article</li>
    <li>section</li>
    <li>aside</li>
    <li>footer</li>
    <li>h1...h6</li>
</ul>

## Most used elements
<ul>
    <li>div</li>
    <li>button</li>
    <li>p</li>
    <li>a</li>
    <li>ol</li>
    <li>ul</li>
    <li>li</li>
    <li>form</li>
</ul>

<a href="https://developer.mozilla.org/es/docs/HTML/HTML5/HTML5_lista_elementos">More elements here</a>

# Class 8

## Importance of a semantic code
 
HTML semantic is give a sense and an structure to the design we are developing through the correct usage of the tags, making a code readable for the maintainers.

Below is shown a list of elements could be used to construct a semantic code.

- < header >
- < section >
- < i > , < em > -> italic , emphasis
- < footer >

# Class 9

## HTML errors, debugging and tag validation service

### Type of errors

* Syntax errors: Related to typing errors.

* Logic errors: Correct syntax, but the code does not work as expected.

### Debugging

The browser's interpret correct our type errors, but still being wrong, so for that reason exists a validator, it can be found in https://validator.w3.org/

# Class 10

## CSS declaration: Selectors, properties and values

```
selector {
    declaration
}
```

where

declaration = `property:value;`

**check class10.html** file

# Class 11

## Selector types, pseudo-classes, pseudo-elements

### Types of selectors

There are different types of selectors, following are shown some of them:

* UNIVERSAL
```
* {
    margin : 0;
}
```
* TYPE (not recommendable)
```
<type> {
    color : red;
}
```
* CLASS
```
.className {
    font-size : 2cm;
}
```
* ID (not recommendable)
```
#id {
    border-radius : 20px;
}
```

### Pseudo-classes

Give us styles to specific classes

* Apply some properties to the first child
```
p:first-child {
    color : white;
}
```
* Apply some properties to the last child
```
p:last-child {
    color : white;
}
```
* Apply some properties to the n-child
```
p:nth-child(n+2) {
    color : white;
}
```
<a href="https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes">MDN Pseudo-classes</a>

### Pseudo-elements

Similar to pseudo-classes, nevertheless differ in syntax
```
p::first-letter {
    color: blue;
    text-transform: uppercase;
}
```
<a href="https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-elements">MDN Pseudo-elements</a>

# Class 12

## Box model, relative values and absolute values

ALL HTML elements have a **box model** composed by:

* content
* padding
* border
* margin

This elements can modify all elements we construct.

**check class12.html** file