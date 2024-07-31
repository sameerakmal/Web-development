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
* Aranging the elements of HTML in a hierarchial way to present on a webpage is called __"DOM"__.
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
* We can make content [sticky](http://127.0.0.1:3000/HTML%20items/src/data-list/Sticky.html) on a webpage using CSS property.
```css
dt{
    position : sticky;
    top : 0;
}
```
### [box-shadow : ](http://127.0.0.1:5500/HTML%20items/src/data-list/box-shadow.html)
* In CSS we can set shadow to any container by using box-shadow box shadow will have 4 values.
```css
{
    box-shadow : horizontal vertical blur color;
}
```
* The unit of horizontal vertical blur is pixels.
## Heading elements :
* Heading elements are mainly used to define headings and to describe a <u>topic</u> in a webpage.
* Heading element default bheaviour is :
    1. display : block; 
    2. font-weight : bold;
    3. font-size : varies from heading to heading;
### Interview questions :

#### 1. Why to use heading element for heading?
#### 2. Why we have to use heading elements for giving heading, can't we configure using HTML text styles and CSS styles?
#### 3. __Can we change the appearance of ```<hn>``` tags?__
* Through CSS we can change the default behaviour
```css
h1{
    font-size : 50px;
    font-weight : lighter;
    color : blue;
}
```
#### 4. Can we remove the default style defined for heading?
* Yes, it can be made possible with the help of CSS inheritance.
```css
h3{
    font-weight : unset;
    display : unset;
    font-size : unset;
}
```
## Working with paragraphs :
### ```<p>``` : 
1. To present the content in the form of paragraph, we use ```<p>``` element.
2. It supports "align" attribute, which can set text left, center, right or justified.
3. Paragraphs will have a line break before and after.
## Blockquotes :
1. It is used to present the summary of the content on a webpage. 
2. Blockquote is similar to paragraph but have left and right indentation for text.
3. It is defined by using ```<blockquote>``` element.
### Interview questions :
#### 1. How to set the first-line indent for paragraph or blockquote?
* Using CSS attribute called ```text-indent : ; ```
```css
blockquote{
    text-indent : 50px;
}
```
#### 2. How to set line space, word space, character space in a paragpraph?
* Using CSS attribute called ```line-height : ;```
```css
blockquote{
    line-height : 30px;
    word-spacing : 7px;
    letter-spacing : 3px;
}
```
#### 3. How to set a DropCap?
* By using the following style we can set DropCrap. : 
    * Access the first letter using the class: first-letter.
    * After Acessing the firstletter apply fonts [size, weight, family].
    * Apply css float as left.

## Difference between display : grid vs column of CSS attribute.
* display : grid would dsiplay the content column wise in the given frame width(column ratio).
* Columns : This attribute would take number of columns as input and display the content in <u>(continuous manner)</u>.

# Text formatting in HTML : 
### Font element :
* We can change the text formatting using font.
* font :: we can change the face(family), size, and color.
#### Syntax :
```css
<font face = " "  size = " " color = " " > Your text </font>
face : font family
size : 1 to 7 leve[increasing order]
color : It represents color name and color code.
```
| Design team | Review team |
| :-----------: | :-----------: |
|```<b>``` | ```<strong>``` |
|```<i>``` | ```<em>``` |
|```<u>``` | ```<ins>``` |
|```<strike>``` | ```<del>``` |

### Interview Questions :
#### 1. What are web safe fonts?
* These fonts are such fonts which would be available in every machine and it can't be deleted. 
* Eg : Sans-serif, monospace, serif.

## Ordered and unordered list
* Order list will add auto numbering for a list of options, which can update automatically when you add or delete items.
* Order list is defined by using ```<ol>``` element.
* Items in list are defined by using ```<li>```.

#### Syntax :
```html
<ol>
    <li> Item-1 </li>
    <li> Item-2 </li>
</ol>
```
#### Note :
* Default number will be given for items.

#### Type :
* It specifies the numbering type, which can be :
1. a
2. A
3. i
4. I
5. 1 (default)

#### start[number] :
* It defines the numbering level to start with.

### Nested list :
* Nesting of list elements.
#### Bad code :
```html
<ol>
    <li>Frontend</li>
    <ol type = "a">
        <li>HTML</li>
        <li>CSS</li>
    </ol>
    <li>Backend</li>
    <ol type = "a">
        <li>MongoDB</li>
        <li>NodeJS</li>
    </ol>
</ol>
```
#### Output : 
<ol>
    <li>Frontend</li>
    <ol type = "a">
        <li>HTML</li>
        <li>CSS</li>
    </ol>
    <li>Backend</li>
    <ol type = "a">
        <li>MongoDB</li>
        <li>NodeJS</li>
    </ol>
</ol>

#### Clean code :
```html
<ol>
    <li>Frontend
        <ol type = "a">
            <li>HTML</li>
            <li>CSS</li>
        </ol>
    </li>
    <li>Backend
        <ol type = "a">
            <li>MongoDB</li>
            <li>NodeJS</li>
    </li>
    </ol>
</ol>
```
#### Output :
<ol>
    <li>Frontend
        <ol type = "a">
            <li>HTML</li>
            <li>CSS</li>
        </ol>
    </li>
    <li>Backend
        <ol type = "a">
            <li>MongoDB</li>
            <li>NodeJS</li>
    </li>
    </ol>
</ol>

### Note : Don't use the bad code even if the output is same.

### Interview Questions :
#### Q1. How to remove numbering in order list?
* It is possible to remove numbering of ordered list element through a CSS attribute called ```list-style : "none"```
#### Q2. How to create a scrollable list?
1. Keep a border
2. Keep a proper width and height as per the content area.
3. using an CSS attribute called "overflow : hidden|scroll|auto"
#### Q3. How to display list items inline?
#### Q4. How to display ```<li>``` in column wise?
##### Grid : 
```css
ol{
display : grid;
grid-template-columns : 6fr 6fr;
}
```
* O/P :
* A.--------B.
* C.--------D.
* E.--------

# Unordered List
- It is used to define bulleted list.
- Bulleted list comprises of symbol instead of numbering.
- Unordered list is defined by using ```<ul>```
- List items are defined by using ```<li>```
- The attribute “type” defines the symbol type,which can be
	- disc
	- circle
	- square

```html
<body>
	<ul type="square">
		<li>Web Sever</li>
		<li>Web Site</li>
		<li>Web Page</li>
	</ul>
</body>
```
#### How to set Custom bullets?
* Ans. we can do by using list-style-image attribute of css.

#### To display the content in fixed style we can use the following attributes of css in "ul"

```css
ul{
    list-style: none;
    position: fixed;
    right: 20px;
    bottom: 10px;
    width: 5px;	
    background-color: white;
    padding: 5px;
}
```
## Pagenation: 
* It refers to process of displaying records by splitting them into <u>pages</u>.

```html
<ul>
    <li><span>&laquo;</span></li>
    <li><span>1</span></li>
    <li><span>2</span></li>
    <li class="disabled"><span>3</span></li>
    <li><span>4</span></li>
    <li><span>5</span></li>
    <li><span>...</span></li>
    <li><span>&raquo;</span></li>
</ul>
```
```css
body{
    display: flex;
    justify-content: center;
    align-items: end;
    height: 500px;
    }
ul{
    list-style: none;
    display: flex;
    }
li{
    margin-right: 10px;
    border : 1px solid black;
    width : 25px;
    padding: 5px;
    text-align: center;
    border-radius: 15px;
    background-color: lightcyan;
    }
```
# Images in HTML
* To use the images in your website you should keep license in mind. So, you need to check images -> tools -> usage rights -> creative common license.
```html
<body>
    <figure>
        <img src = "public/images/iphone.jpg" alt = "can't display" title = "iphone" height = "100" width = "100" border = "3" align = "left">
        <figcaption>Iphone</figcaption>
    </figure>
</body>
```
## Different types of images
| Abbreivation | File format | MIMEType | FileExtension |
| :-----------: | :-----------: | :-----------: | :-----------: | 
|APNG | Animated portable NetworkGraphics | image/apng | .apng |
|BMP | Bitmap file | image/bmp | .bmp |
|GIF | Graphics Interchange Format | image/gif | .gif |
|ICO | Microsoft icon | image/x-icon| .ico, .cur |
|JPEG | JointPhotographic Expert Group | image/jpeg | .jpg, .jpeg, .jfif, .pjeg, .pjp |
|PNG |PortableNetworkGraphics | image/png | .png |
| SVG   | ScalarVectorGraphics   | image/svg+xml | .svg          |
| TIFF  | TaggedImage FileFormat  | image/tiff    | .tiff,.tif    |
| WebP  | WebPicturFormat         | image/webp    | .webp         |


### What is MIME?
* MIME stands for <b>"Multipurpose internet mail extension".</b>
* Server upon sending the information to the browser, it will also send what type of information is being sent.
* To inform the type of information, we go for MIME type.

### Different types of images and their purpose
| Image type | Purpose|
| :-----------: | :-----------: | 
| PNG | 1. High resolution(More space) <br> 2.suitable for downloads |
| JPG | 1. Compressed image format(less space) <br> 2. good for presentation |
|GIF| 1. Low resolution <br> 2. Used for animations |
|SVG | 1. Not pixel based <br> 2. High zoom quality <br> <b>Eg :</b> Google maps, Bootstrap icons.
|Webp | If we try to save an image, it saves the entire image. Image alone can't be captured.| 

### Embedding an image in webpage :
```html
<img src="" alt = "" width = "" height = "" title = "">
``` 

