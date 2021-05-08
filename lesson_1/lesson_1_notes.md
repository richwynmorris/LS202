# LS202 = HTML and CSS

Created: May 5, 2021 9:15 PM
Reviewed: No

## Lesson 1

- HTML - Hyper Text Markup Language - gives the website structure and meaning
- CSS - Cascading Style Sheet - gives the website style and colour - primarily to do with the presentation.

Although HTML and CSS work in hand with one another, they should be considered independent and not be used within on another. HTML should not be used inside CSS and CSS should not be used within HTML. 

An **element** is defined used a `<` and `>` symbol. They are used to define and structure the content on the website Examples of elements are `p`, `h1` , `a` `div`. An element will be self closing or will contain the opening the closing tag and everything within itself. An element is both the tags and the context that exists between them.

A **tag** is the `<` and `>` element that surrounds the element. Tags come as opening, closing  and self closing. However, most tags are not self closing.  

**Attributes**  are the properties of an element which hold information relating specifically to the element. Examples of attributes are `id`, `class`, `href` and `src`. The attributes of an element are contained within the opening tag, after the name of the tag. The attribute will use an `=` sign and be assigned a value which will be within quotation marks `"".`

**HTML Format**

The HTML format uses the following structure; `<DOCTYPE! HTML>`, `<html>`, `<head>` and `<body>`. 

`<DOCTYPE! HTML>` - This is declaration that informs the browser which version of html to use to display the context of the webpage. When unspecified it defaults to the most up to date version. 

`<html>` - This element indicates the start of the html document to the browser.

`<head>` - This element often contains all the metadata needed to be used for the webpage to be displayed but itself does not impact what is displayed on the web page, other than what the webpage name is displayed as in the user's browser. 

`<body>` - This element contains all the visual context the webpage will display. 

Example:

```html
<DOCTYPE! HTML>
  <html>
    <head>
      <body>
         <h1> Hello world! </h1>
      </body>
    </head>
  </html>
```

### CSS

The cascading style sheet has 3 different key components that make up the styling of a webpage. They are **selectors, properties and values.** 

**Selectors** 

Selectors are they of designating specific styles to particular elements that exists on in a html document. 
Selectors come in 3 different qualifiers; **type, class and id.**

**type -** this selector targets the type of element and if often used when an element needs to be styled in a specific way throughout a website.

**class** - this selector targets the any element of specific class. classes can cover different elements types across a web page. This selector is defined with a prefixed `.` to the name of the class. 

**id -** id is a very specific selector that you can only use on a singular element in the html file. The id selector is prefixed with a `#`. 

**Properties**

Properties are type of styles that will be applied to the element. They are contained within the brackets that come after the selector. It is terminated with a semi colon. 

```css
p { color: }
<!-- `p` is the selector, `color` is the property.
```

**Values**

Values are the behaviours of specific properties within the selector. They dictate the appearance and style of property. They are terminated with a semi colon `:` Both properties and values are indented within the curly brackets of the selector. 

### Referencing A Style Sheet in a HTML File

A style sheet needs to be included in a `<link>` element within the `<head>` of the html file. Within the self closing `<link>` tag, if should make reference the the relative css file using the syntax `href="file.name` as well as identify the relationship between the html and css file using `rel="stylesheet"` .  The end product should look something like this:

```html
<head>
  <link rel="stylesheet" href="file.name"> 
<head>
```