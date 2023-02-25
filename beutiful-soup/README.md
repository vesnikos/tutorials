## About

#### The DOM (Document Object Model)
We are all familiar with the web and web pages. If you ever happened to open the source code of a web page, you would propably must have  something like this:

```html
    <html>
        <head>
            <title>Title of webpage</title>gh repo clone vesnikos/tutorials
        </head>
        <body>
            <h1>My first web page</h1>
            <p>My first paragraph.</p>
        </body>
    </html>
```
### Preqrequiments
If you have not installed the `beautifulsoup4` library, you can do so by running the following command in your terminal:
```bash
pip install beautifulsoup4
```

### The HTML
The above text, is the source code of a web page. It is written in a markup language called HTML (HyperText Markup Language), which is very similar to `XML` (xml stands for eXtensible Markup Language). Which like json, is designed to store and transport data. The difference between `XML` and `HTML` is that `XML` is designed to transport and store data, while `HTML` is designed to display data in a web browser.

Both of them can be represented as a `tree`. With the HTML tag at the head node on the top, which contains the `head` and the `body` tags as children. Further more, both of them can contain other tags as children, which they can contain other tags as children as so on. This is called a `tree` structure.

> Note: An html tag is a tag that starts with `<` and ends with `>`. Inside you can find the type of the tag, (i.e `<html>` is an html tag). Inside in each tag you can find attributes, which are key-value pairs, (i.e `<html lang="en">`). You can designate children  by putting them inside the parent tag, (i.e `<html><head></head></html>`), and on.  

> Note: the children do not have to be tags, they can be text as well, (i.e `<html>Some text</html>`).

The `DOM` (Document Object Model) is an interface for HTML. It `represents` the page so that programs can change the document structure, style and content. The DOM represents the document as nodes and objects. That way, programming languages can connect to the page.

> Note: javascript and other programming languanges can connect to the DOM and manipulate it in order to change the page. They can add new elements, change the style of the page, and so on.

> Note: this is in principle, how the `React` library works. It connects to the DOM and manipulates it in order to change the page. It has matured in such a stage that literally the initial DOM (html) it is almost not needed anymore. The `React` library adds elements (or removes, or modifies) on the dynamicaly. 

## Dom and Python
In order to connect to the DOM, we need to use a library. In python, one of the most popular libraries can help us use the DOM is `BeautifulSoup`. 

It can pull data out of HTML (and XML) files.
It works with your a number of parsers to provide idiomatic ways of :
-  navigating,
-  searching,
-  and modifying the parse tree.

> Note: A parser is a program that reads text and produces a data structure. When in the last chapters we talked about `json`, the json library contains a parser, that reads the `json-string` and produces a python object (a dictionary in most cases).

In the following chapters, we will see how we can use `BeautifulSoup` to parse the DOM, navigate through it, and pull out the data that exist in the DOM.

> This is called `web scraping`.  It is a technique to extract data from websites from it's html source.

to extract data, the DOM must be complete. As discussed in a previous note, the DOM usually could start empty and then the javascript code will add the elements. So, if you want to extract data from a website, you must wait until the DOM is complete. To achieve that, you'll need use different approaches. that are note covered in this tutorial. But if you're interested I recommend you do search about `selenium` and `headless browser`. After you have a complete DOM, the techniques that we will see later will work.

> NOTE: to extract data from a website in such way is not always legal. It is legal if the website allows it. If it does not allow it, could be illigal. So, be careful.

Chapters: 
 - [Navigating the DOM](./notebooks/navigating-the-dom.ipynb) 
 - [Searching the DOM](./notebooks/searching-the-dom.ipynb)
 - [Extracting data from the DOM](./notebooks/extracting-data-from-the-dom.ipynb)
 - [A complete example](./notebooks/a-complete-example.ipynb)