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

# CSS
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