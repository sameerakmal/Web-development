## Client server architecture:
* Client is a computer which is capable of sending request to other computers present in internet.
* We say client as a computer but in reality browser software is termed as a client.

![alt text](client_server.png)
## Server:
* It is a computer which has the capability to provide output to any number of clients.
* Normally, a server computer woud be referred as high configuration computer.
* Inside the server computer we install a server software called web server.
* Eg : Tomcat, wildfly, glassfish.

![alt text](engine.png)
### Note:
* Installing nodejs wil promote a build tool through which we can automate the process of taking third party libraries from different websites to our projects with the help of a command called "npm".

## HTML:
* On a browser to display the content as per our requirement we need to __markup__ our content.
* To markup the content on the browser we need a language called __html__(hyper text markup language).

### HTML PARSING:
![HTML Parsing](HTML_parsing.png)

### Evolution of HTML language
* __GML__ : Generic makrup language.
* __SGML__ : Standard Generic makrup language.
* Tim Burner Lee introduced a new markup language called as HTML which is a subset of SGML.
* Initially, HTML language was a open source language.
* HTML was introduced as communicating language to web by Tim Burner Lee.
* HTML language is maintained by a community called __WHATWG__.
* HTML 4 version didn't gave importance for SEO and responsive design. 
* In HTML 5 different __semantics__ were introduced to give importance for SEO and response design.
* SEO refers to search engine optimization.
* Whenever we type some content on a browser which needs to be searched. Google search engine uses SEO technique(robo)
* BOT names : web spiders, web crawlers, bot etc...

### Categories of HTML element : 
1. Normal element Eg. bold tag
2. Void element Eg. img tag
3. RC(Rich context) data elements. 
Eg : 
```html
<textarea>
    <p> Hello pw'ian </p>
</textarea>
```
* Output :   <textarea>
        <p> Hello pw'ian </p>
    </textarea>
4. Raw text element
Eg :  1. Temperature 25C 4500/- 2. Temperature 25&deg;C &#8377;4500/-
5. Foreign element : importing someone's code. Eg : SVG, Mathl

### HTML Structure : 
* Araanging the elements of HTML in a hierarchial way to present on a webpage is called __"DOM"__.
```html
<html>
    <!--Document scope-->
    <head>

    </head>
    <body>
    
    </body>
</html>
```
* The content presented in the head section is mainly used for SEO and responsive design.
* The elements which can be written inside head section are :
```html
<title>
<link>
<meta>
<style>
<script>
```

![alt text](html_structure.png)

```html
<!DOCTYPE html>
```
* It is a indication to a browser engine that in the body section we use elements of HTML 5.
```html
<html lang = "en-IN">
```
* It is an indication to the browser that the output should be feasible to the end user in particular format. 
## Body section
### Attributes of body tag :
1. bgcolor : This attribute is used to set background color for body section.
2. text : This attribute is used to set a different color value for the content to be presented.
```html
<body bgcolor = "black" text = "white">
--
</body>
```
* To control elements on a webpage after the presentation we go for __CSS(styling language)__.
#### Note
* We can control images only through css attributes. 
* These attributes are defined in a ```<style>``` manner.
* CSS attributes for background are :
```css
background-repeat : repeat|no-repeat|repeat-x|repeat-y|
background-size : contain|cover|auto|width and height in pixels|
background-positon : top|center|right|left|
background-attachment : fixed|scroll|
```
### HTML 5 new semantics(elements) :
1. Header
2. Section
3. Nav
4. Main
5. Article
6. Figure
7. Figcaption
8. Dialog
9. Aside
10. Div
11. Span 
![alt text](semantics.png)

#### Note:
* The ```<span>``` tag is much like the ```<div>``` element, but ```<div>``` is a block level element and ```<span>``` is an inline element.
![alt text](basic_dom.png)

#### DOM : 
* To align the content in column-wise using CSS. We have an option called __display:flex__.
* We can control the attribute of font through CSS using font-family,font-style,font-size,font-weight.
* For a span element, width property can't be applied directly. To see the effect we use a attribute called __display:inline-block__.
![alt text](shopper_dom.png)

#### Note:
* Default screen width is 1200px, so max no of columns in a page is 12.

## Different types of CSS Selctor:
### Selecting child and sibling in CSS:
```
parent child{  --> child selector

}
Element A + Element B { --> Adjacent building

}
Element A ~ Element B { --> All elements are specifc

}
```
* For any image to be blurred and if the content has to be presented on a blurred image we go for an attribute called background-color : rgba.
* "a" stands for alpha, the range of a is 0 to 1.More the value,lesser the blur.

### Amazon:

[Amazon footer](http://127.0.0.1:3000/Footers/src/amazon_footer.html)
#### Amazon footer DOM:
![Amazon footer dom](Amazon_footer_dom.png)

### Flipkart:
[Flipkart footer](http://127.0.0.1:3000/Footers/src/flipkart_footer.html)
#### Flipkart footer DOM:
![Flipkart footer DOM](Flipkart_footer_dom.png)
### To display any content to the center:
1. Keep all the contents in one container.
2. 
```html
<body>
    <div>
        //your content here
    </div>
</body>
```
3. body is the container here which would display the contents center with attributes.
```css
body{
    dsiplay:flex;
    justify-content:center;
    align-items : center;
    height:100vh;
}
```
4. Note : 
    1. justify-content : center;(horizantal)
    2. align-items : center;(vertical)
 
### Fig and figcaption
* Fig caption element is used by search engine to load the image as a search result for the end user.
```html
<figcaption>
    <div>
        <!-- Place image -->
    </div>
</figcaption>
```   
#### Elements designed for coding platforms:
1. ```<code>``` : To indicate the presentation content is for programming.
2. ```<var>``` : To indicate the browser engine that it is a variable.
3. ```<samp>``` : To indicate the description about the program.
4. ```<pre>``` : It is used to preserve the white spaces in particular container.
5. ```&nbsp;``` : It is used to mark the spaces set by user at any element.
#### HTML basic entities and semantics for body
1. Line break ```<br>``` : 
    * Browser ignores the line breaks given in edition.
2. FAQ : What is the diffference between ```<br>``` and ```</br>```?
    * There is no such element called ```</br>```.
    * Always use ```<br>```. It is a self closing tag.

#### Small text and large text :
1. ```<small> small text</small>``` : It sets letter small size.
2. ```<large> large text</large>``` : It sets letter large size.

### Details and summary
```html
<body>
    <details>
        <summary></summary>
        <!-- content to be placed here-->
    </details>
</body>
```
* It is used to display the content in detail only when required.
* It allows to expand and collapse your content.
* It saves the screen space.

### Data list with terms and definitons :
#### Syntax :
```html
<dl>
    <dt>Term</dt>
    <dd>Definition</dd>
    <dt>Term</dt>
    <dd>Definition</dd>
</dl>
```
#### Note :
1. ```<dt>``` and ```<dd>``` will have some default alignment, so it is easy for presentation.
2. ```<dl>``` has the capability to display in columns using grid(dt --> one column and dd --> one column).

#### Note :
* We can make content sticky on a webpage using CSS property.
```css
dt{
    position : sticky;
    top : 0;
}
```
### box-shadow :
* In CSS we can set shadow to any container by using box-shadow box shadow will have 4 values.
```css
{
    box-shadow : horizontal vertical blur color;
}
```
* The unit of horizontal vertical blur is pixels.